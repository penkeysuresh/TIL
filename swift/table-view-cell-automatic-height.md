Using auto layout we can design dynamic table view cells. This will save us from a lot of sizing code given, there are multiple screen sizes to take care of recently in iOS. Instead of giving a height in storyboard or in ``heightForRowAtIndexPath`` one can give constarints from top and bottom in storyboard and add below line in the code.

		self.tableView.rowHeight = UITableViewAutomaticDimension
		self.tableView.estimatedRowHeight = 120.0

This will take care of the height of the cells based on the content size and also scale easily in other devises. 