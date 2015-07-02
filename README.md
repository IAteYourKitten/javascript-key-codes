# Javascript Keys
An implementation of javascript keycodes to use in your project

### Installation

Simply include javascript-key-codes.js in your page, and then pass e.which as an argument to the get_key() function.  Check out the [demo](http://server.pointybracket.net/js-keys/test).

The get_key() function will return a human-readable key. In the following example we can say "if key == 'enter'" and then do something if the user pressed the enter key.

#### Basic Example

    $(document).ready(function(){
	      $(document).on('keyup', function(e){
		        var key = get_key(e.which);
  		
		        $('#result').html(key);
		
		        if(key == 'enter'){
			          alert('You pressed enter');
		        }

		        return false;
	     });
    });
