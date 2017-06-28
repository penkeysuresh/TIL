In iOS by default modals are presented as a sheet from the bottom of the screen. From iOS 7 onwards we can completely customize the animation by which transitions happens, whether it be a push onto a navigation controller stack, selecting a different tab, or a plain presentation

We can acomplish this by setting the ``modalPresentationStyle`` to ``UIModalPresentationCustom`` and set your self as the ``transitionDelegate``. After defining the delegate we'll need to implement ``UIViewControllerTransitioningDelegate`` methods. 

For more : http://www.teehanlax.com/blog/custom-uiviewcontroller-transitions/
