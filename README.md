socialSharePrivacy for PrototypeJS
===============================

This is the PrototypeJS version of the jQuery-plugin socialSharePrivacy of the "Heise Zeitschriftenverlags". More information about the original plugin and the options can be found here http://www.heise.de/extras/socialshareprivacy/

How to use
----------

Add a block element, such as div, with the class "socialshareprivacy" to your document, at the position where you want to place your buttons. 

	<div class="socialshareprivacy"></div>

Then call the socialSharePrivacy function, when the page was loaded:

	document.observe("dom:loaded", function() {
		socialSharePrivacy.init({
			'id':'socialshareprivacy' // Element ID
			// ... rest of options
		});
	});

You can also pass options to the plugin (for more details, see http://www.heise.de/extras/socialshareprivacy/ ):
    
	socialSharePrivacy.init({
		'id':'socialshareprivacy', // Element ID
		services : {
			twitter : {
				'status' : 'off'
			},
			gplus : {
				'status' : 'off'
			}
		}
	});