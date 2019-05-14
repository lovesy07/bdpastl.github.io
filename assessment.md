# HSCC Assessment 2019

This assessment is intended to help determine which students will be competing in the 2019 High School Coding Competition in Atlanta, GA.



## Matching (1pt each)

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



## Short Answer (2.5 pts each)

1. What does CSS stand for?
2. What does HTML stand for?



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

