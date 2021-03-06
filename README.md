#jQPad#
####By Adrian Cooney####

jQPad is an iPad web development framework by Adrian Cooney. jQPad follows the existing interface patterns of iOS make creating complex AJAX powered website in minutes (although effort is encouraged).

#FAQ#
* __Where can I download jQPad?__

 	jQPad is hosted on Google Code for now. [Here's a direct link](http://code.google.com/p/jqpad/) though this is the old version.

* __Can I contribute to jQPad?__

	Of course you can! All help is appreciated whether it be a plugin, theme or help with all the internal functionality. Please give me a quick email to [jqpadframework@gmail.com](mailto:jqpadframework@gmail.com "jqpadframework@gmail.com").
	
* __Can I suggest a feature?__

	Yes! All suggestions are greatly appreciated. Drop an email to [jqpadframework@gmail.com](mailto:jqpadframework@gmail.com "jqpadframework@gmail.com") with your suggestions. If you could, please be a detailed.
	
* __Is this the only way to access the jQPad documentation?__

	Unfortunately, yes for the time being anyway. jQPad will be powered by aDocs in time when the first official build is released.
	
#Documentation#

##Overview##
###Understanding how jQPad works###
jQPad has two viewports, one on the left for navigation and one on the right for content. The whole content system is based on AJAX calls to retrieve content from the 'content/' directory, unlike many of it's counterparts, which store all their content on the one page. (In future versions, there will be this option.)

##Package.json##
This is where all the jQPad's required information is stored i.e Site name, author information, menu bar

##Theming##
###Elements and their classes###
Please take a peek in `docs/theming.html` for the elements and their equivalent class/id/tag.

##API##
###Plugin Development###
Creating plugins for jQPad is simple, we first have to extend the jQPad object then attach the plugin to an event, whether that be simply for it to be called when the DOM has loaded or when a specific element is clicked/tapped. The plugin API contains only two functions, `attachEvent()` and `attachResource()`. More will be added in future releases.

####__attachEvent( name, function )__####
__name__ -- The name of the event to be triggered.  
__function__ -- The function to be executed when the event is triggered.
