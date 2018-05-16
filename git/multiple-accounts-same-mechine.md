Using multiple github or bitbucket accounts (personal and work) in a single machine using ssh keys. (Since these services won't
allow same ssh key to be used in diffrent accounts.)

To acomplish this we need to do 3 things:

- Create two ssh keys against work and personal in your system
- Change the ssh config to use diffrent keys (accounts) for diffrent hosts
- Change the repository level configuration to push to approriate remote. 


### Changing SSH config

You can tell ssh service to use diffrent configuration and ssh keys for diffrent hosts. You can do this as below.

First create a config file in `.ssh` directory
 
          touch ~/.ssh/config
          
Add configuration as below

        #Default GitHub
        Host github.com
          HostName github.com
          User git
          IdentityFile ~/.ssh/id_rsa
        Host bitbucket-<org_name>
          HostName bitbucket.org
          User git
          IdentityFile ~/.ssh/id_rsa_<org_key>
          
### Change repository level configuration

You can set email and username for each repository. You can use 

        git config user.name git config user.email
        
Do note that this setting won't affect the git global configuration. Which can be checked passing `--global` 
flag to above command

Now whenever you have to clone from you org, just replace `bitbucket.org` in clone url to `bitbucket-<org_name>`

          git@bitbucket-<org_name>:<org_name>/<repo-name>.git
