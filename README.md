node-cooperhewitt
=================

A little node module to call into the [cooperhewitt api](http://collection.cooperhewitt.org/api)

You can get a API TOKEN pretty easily [right here](https://collection.cooperhewitt.org/api/oauth2/authenticate/like-magic/).

To install it, just do this:

    $ npm install node-cooperhewitt

And then in your project somewhere, do something like this:

    var cooperhewitt = require('node-cooperhewitt')
    
    var api_token = '<YOUR API TOKEN>';
    
    var method = 'cooperhewitt.objects.getRandom';
    var args = {'access_token': api_token};
          
    cooperhewitt.call(method, args, function(rsp){   
	    console.log(rsp);  
    });