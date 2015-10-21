# Web Useful Resources
web programming useful resources link

berikut adalah link yang penting :<br/>
# CSS / Font Graphics
Web Icon-Fonts Graphics :<br/>
1. <a href="http://glyphicons.com/" target="_blank">Glyphicons Icons</a><br/>
2. <a href="https://fortawesome.github.io/Font-Awesome/icons/" target="_blank">Font-Awesome Icons</a><br/>

# Javascript / Client Side
Javascript Modules :<br/>
1. <a href="http://wenzhixin.net.cn/p/multiple-select/docs/" target="_blank">Multiple Select</a><br/>
Info ajax<br/>
```javascript
  $.ajax(
        url 		: 'functions_link.php',
		type 		: 'POST',
		data 		: JSON.stringify(getDataFunctions()),
		success		: function(response) {resultData(response)},
		error		: function(e) {onError(e);},
		dataType 	: 'json',
		contentType : 'application/json'
	});
```
Info ajax File Upload<br/>
```javascript
  $.ajaxFileUpload({
		url 			: 'functions_link.php',
		type 			: 'POST',
		secureuri      	: false,
		fileElementId	: 'temporary_image',
		data			: JSON.stringify(data),
		success			: function(response) {resultUpload(response);},
		error			: function(e) {onError(e);},
		dataType 		: 'json'
	});
```
# Server Side PHP Framework
PHP Framework :<br/>
1. <a href="https://github.com/ivantcholakov/starter-public-edition-3" target="_blank">Code-Igniter 3</a><br/>

# Web Programming Tutorials
1. <a href="http://www.w3schools.com/" target="_blank">w3schools</a><br/>
2. <a href="http://www.javatpoint.com/" target="_blank">Java Web Services Tutorial 1</a><br/>
3. <a href="http://docs.oracle.com/javaee/6/tutorial/doc/gijti.html" target="_blank">Oracle Introduction to Web Services - Java EE 6</a><br/> 
