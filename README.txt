FixedScroll
===========

A plugin to fix an element to the screen while scrolling.

Background
==========

Initial code from: http://jqueryfordesigners.com/fixed-floating-elements/

Plugin Information
==================

Modified the above code to work as a plugin.  Options have been added to 
allow the user to:

1. add padding to the top of the element being fixed
2. set an element that the fixed item cannot scroll past

Note: This does not work in IE6.

Usage
=====

Best to be called from the window load function so as to take into 
account any images that are loaded in the document.  Below is an example:

$(window).load(function(){
	$("#element").fixedscroll({
					padding: 20,
					boundary: '#element2'
	});
});

This "works for me."(tm)  Please feel free to clone this package and send
me merge requests.