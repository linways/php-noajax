# NoAjax

A JavaScript library which helps to call the PHP server methods directly from the browser.

**Usage**
```
noajax.call(name, [arg1, arg2...], [callback])
```
`name` [string] : Name of the server side method.  
`arg1, arg2, ...` : Optional method arguments  
`callback` [function]: Optional callback, which is called asynchronously with the error and result after the method is complete  

**Example**  
```
    noajax.call("addTwoNumbers", 2, 4, function(err, res){
        if(err)
            console.log("Error: " + err.message);
        if(res)
            console.log("Result: " + res);
    });
```

## Build
To Build the project you need to install grunt-cli   
`npm install -g grunt-cli`  

```
 npm install
 grunt
```

## Tests
To run the tests

```
 cd PHPTestMethods
 php -S localhost:8000
```

Then open `test/testRunner.html` in a browser to run the tests.