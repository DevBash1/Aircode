# Aircode
A Javascript Text Encryptor for encrypting text to spaces.
This is not the normal encryption we are used which encrypts text to text.   
Example

| Encryption Type | Text | Result |
| ------------- | ------------- |  ------------- |
| sha1  | hello world | 2aae6c35c94fcfb415dbe95f408b9ce91ee846ed |
| md5  | hello world | 5eb63bbbe01eeed093cb22bb8f5acdc3 |
| aircode | hello world | 	 		 				  	 	 			 		 	  	 	 		 	 			  	 	 		 	 			  	 	 		 	 	 	 	  	 						  	 	 	 		 	 	 	  	 	 		 	 	 	 	  	 	 	 			 		  	 	 			 			|


As you can see from the example above.   
The result for `aircode` seems empty but it is actually filled with spaces and tabs.
Aircode can encypt text, numbers, symbols, emojis and other text characters to spaces.   

With this,      
You can easily encrypt a file with credencials and make them appear as an empty file.   
A hacker or any attacker who gets access to a file aircoded will think it's just an empty file.

Aircode is meant to be used with other encryption types like `sha1`,`md5`,etc and then the result aircoded into a file which will then appear blank.   

# Usage
Aircode can be installed from npm and has no dependancy,   
It can also be used from the web by adding the js script.

```
npm i -g aircode
```

To use from nodejs.

```javascript
let air = require("aircode");

let str = "hello world";

// Convert String to Aircode
let aircode = air.airencode(str);
console.log(aircode) // 

// Convert Aircode to String
let text = air.deair(aircode);
console.log(text) // hello world
```

To use from terminal,   
Make sure to install globally with command.   
```
npm i -g aircode
```

To airencode a text file run the command   

```
aircode -a input.txt output.txt
```

Then to deair an airencoded file back to it's original form, use the command.   
```
aircode -d output.txt input.txt
```

This will decrypt the airencoded file.
