### Відображення повідомлення alert за допомогою JavaScript

void webAlert(string $msg[, $url]);

**$msg** - повідомлення, показане в alert.
**$url** - залежно від значення визначає дію, яка йде після alert. 

Значення починається з 'javascript:'.
Якщо далі вказати код, він виконається, а якщо далі вказати адресу, відбудеться редирект, а якщо далі порожньо - нічого.

***

#### Приклад.

	$modx->webAlert('Hello!');
	//Виведе alert с повідомленням «Hello!».

	$modx->webAlert('Hello!','http://modx.im');
	//Виведе alert с повідомленням «Hello!», далі відбудеться редирект на http://modx.im.

Також зверніть увагу на regClientScript(), sendAlert().
