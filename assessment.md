# HSCC Assessment 2019

This assessment is intended to help determine which students will be competing in the 2019 High School Coding Competition in Atlanta, GA.



## Matching (2pt each)

Match the following html elements to their descriptions

```
a. body
b. head
c. a
d. img
e. br
```

1. Contains links to both internal and external web pages _________

2. Can be used to create a new line with out creating a new section _________

3. Contains the content that renders on the page _________

4. Contains titles, styles, and scripts _________

5. Used for putting images on a page _________

   

## True or False (2pts each)

1. A **div** is a block level element  _________
2. A **p** is is a block level element  _________
3. An **h1** element is smaller than an **h2** element  _________
4. A **ul** element is used to create an unordered list  _________
5. Both **ul** and **ol** have **al** elements as children  _________
6. Examples of common html attributes are **class**, **type**, and **id**  _________
7. Padding adds space around an html element whereas margin adds space within an html element  _________
8. The **href** attribute is used within an **a** element  _________
9. The **src** attribute is used within an **img** element  _________
10. An **em** is an inline element  _________



##  Multiple Choice (2.5 pts)

1. Given the code: 

```html
<div id='myID'>
   I am a div!
</div>
<div>
  I am also a div! 
</div>
```



Which of the following css selectors would change the background color of the first div to black (circle one): 

```css
.myID {
  background: 'black';
}
```



```css
div {
  background: 'black';
}
```



```css
#myID {
  background: 'black';
}
```



```css
.myID {
  background: 'blue';
}
```





2. How many columns are in the bootstrap grid system? 

   4 Columns

   6 Columns

   8 Columns 

   12 Columns

   

   

3. Given the code: 

```html
<!doctype html>
<html>
  <head>
    <script>
    		const sayHi = function() {
          alert('HI!')
        }
    </script>
  </head>
  <body>
   
    
    
  </body>
</html>
```



Which of the following buttons will alert the user with a message "HI!"?

```html
<button onPress='sayHi'>  Press me </button>
```



```html
<button onClick='sayHi'>  Press me </button>
```



```html
<button handleClick='sayHi'>  Press me </button>
```



```html
<button onPush='sayBye'>  Press me </button>
```





4. Given the following code: 

```html
<!doctype html>
<html>
  <head>
     <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css" integrity="sha384-HSMxcRTRxnN+Bdg0JdbxYKrThecOKuH5zCYotlSAcp1+c8xmyTe9GYg1l9a69psu" crossorigin="anonymous">
  </head>
  <body>
   	
    <div>  ONE    </div>
    <div>  TWO    </div>
    <div>  THREE  </div>
    
  </body>
</html>
```



What classes would you use to ensure that each div took up the entire page on an extra small screen, but all rendered in the same row on any other screen?



```html
col col-xs-12
```



```html
col col-xs-8 col-md-4
```



```html
col col-xs-6 col-lg-12
```



```html
col col-xs-12 col-sm-4
```







## Short Answer (4 pts each)

1. What does CSS stand for?



2. What does HTML stand for?



3. Given the code, what is the output? 

```javascript
for( var i = 0; i < 6; i++ ){
  console.log('i = ' + i)
}
```















4. Given the code, what would you put into the style section of the html to wrap a border around the div? 

```html
<!doctype html>
<html>
  <head>
    <style>
    
    
    
    
    
    
    </style>
  </head>
  <body>
    <div>
      I am a div! I sure wish I had a border around me.
    </div>
  </body>
</html>
```





5. Given the code, what is the output? 

```javascript
const myFunction = function(parameter) {
	var output = 'Hi ' + paramter
  
 	console.log(output)  
}


myFunction('friend')
```







6. Name any 4 CSS properties:
   1. 
   2. 
   3. 
   4. 





7. What is the output of the following code? 

```javascript
var number = 10

if (number % 2 == 0){
  console.log('HELLO')
} 
else {
  console.log('WORLD')
}

console.log('!!')
```







8. What is the output of the following code? 

```javascript
var array = [7, 3, 9, 10, 13]

console.log('Array at element 0 is ' + array[0])
```







9. What is the output of the following code? 

```javascript
var size = 2
var array = [7, 3, 9, 10, 13]

var counter = 0

while (counter < size){
  array[counter] = counter
  
  counter = counter + 1
}

console.log('Array at element ' + counter + ' is ' + array[counter])
```







10. In the following code, how would you print out favorite food? 

```javascript
var myDetails = {
  name: 'My Name',
  birthday: 'MyBirthday', 
  favoriteFood: 'Pizza', 
}





```









## Code Analysis (10 pts)

###### styles.css

```css
#container {
  display: flex;
  flex-wrap: wrap;
}

.class-one, .class-four {
  width: 100%;
  height: 10vh;
  background: red;
}

.class-two {
  width: 20%;
  height: 80vh;
  background: blue;
}

.class-three {
  width: 80%;
  height: 80vh;
  background: green;
}
```

###### index.html

```html
<!doctype html>
<html>
  <head>
    <link rel="stylesheet" href="./styles.css">

  </head>
  <body>
    <div id="container">
      <div class="class-one">

      </div>
      <div class="class-two">

      </div>
      <div class="class-three">

      </div>
      <div class="class-four">

      </div>
    </div>
  </body>
</html>
```

Draw what the user will see in the box below. Label the areas with their colors.

```
























```

