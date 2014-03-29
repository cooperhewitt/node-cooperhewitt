node-cooperhewitt
=================

A little node module to call into the [cooperhewitt api](http://collection.cooperhewitt.org/api)



    var cooperhewitt = require('./index')
    
    var api_token = '';
    
    var method = 'cooperhewitt.objects.getRandom';
    var args = {'access_token': api_token};
      
    
    cooperhewitt.call(method, args, function(rsp){
    
	    console.log(rsp);
    
    });