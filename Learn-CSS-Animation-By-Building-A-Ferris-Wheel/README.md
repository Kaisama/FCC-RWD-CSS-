# freeCodeCamp_ferrisWheel
 In this course, you'll build a Ferris wheel. You'll learn how to use CSS to animate elements, transform them, and adjust their speed.

```html
<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <title>Ferris Wheel</title>
    <link rel="stylesheet" href="./styles.css" />
  </head>
  <body>
    
  </body>
</html>
```

```html
  <body>
    <div class="wheel">
      <span class="line"></span>
      <span class="line"></span>
      <span class="line"></span>
      <span class="line"></span>
      <span class="line"></span>
      <span class="line"></span>
      <div class="cabin"></div>
      <div class="cabin"></div>
      <div class="cabin"></div>
      <div class="cabin"></div>
      <div class="cabin"></div>
      <div class="cabin"></div>
    </div>
  </body>
```

```css
.wheel {
  border: 2px solid black;
  border-radius: 50%;
  margin-left: 50px;
}
```

```css
.wheel {
  border: 2px solid black;
  border-radius: 50%;
  margin-left: 50px;
  position: absolute;
  height: 55vw;
  width: 55vw;
}
```

```css
.wheel {
  border: 2px solid black;
  border-radius: 50%;
  margin-left: 50px;
  position: absolute;
  height: 55vw;
  width: 55vw;
  max-height: 500px;
  max-width: 500px;
}
```

```css
.line {
  background-color: black;
  width: 50%;
  height: 2px;
}
```

```css
.line {
  background-color: black;
  width: 50%;
  height: 2px;
  position: absolute;
  left: 50%;
  top: 50%;
}
```

```css
.line {
  background-color: black;
  width: 50%;
  height: 2px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform-origin: 0% 0%;
}
```

```css
.line:nth-of-type(2) {
  transform: rotate(60deg);
}
```

```css
.line:nth-of-type(3) {
  transform: rotate(120deg);
}

.line:nth-of-type(4) {
  transform: rotate(180deg);
}

.line:nth-of-type(5) {
  transform: rotate(240deg);
}

.line:nth-of-type(6) {
  transform: rotate(300deg);
}
```

```css
.cabin {
  background-color: red;
  width: 20%;
  height: 20%;
}
```

```css
.cabin {
  background-color: red;
  width: 20%;
  height: 20%;
  position: absolute;
  border: 2px solid;
}
```

```css
.cabin {
  background-color: red;
  width: 20%;
  height: 20%;
  position: absolute;
  border: 2px solid;
  transform-origin: 50% 0%;
}
```

```css
.cabin:nth-of-type(1) {
  right: -8.5%;
  top: 50%;
}
```

```css
.cabin:nth-of-type(2) {
  right: 17%;
  top: 93.5%;
}

.cabin:nth-of-type(3) {
  right: 67%;
  top: 93.5%;
}

.cabin:nth-of-type(4) {
  left: -8.5%;
  top: 50%;
}

.cabin:nth-of-type(5) {
  left: 17%;
  top: 7%;
}

.cabin:nth-of-type(6) {
  right: 17%;
  top: 7%;
}
```

```css
@keyframes wheel {
  
}
```

```css
@keyframes wheel {
  0% {
    
  }
}
```

```css
@keyframes wheel {
   0% {
     transform: rotate(0deg);
   }
}
```

```css
@keyframes wheel {
   0% {
     transform: rotate(0deg);
   }

   100% {
     transform: rotate(360deg);
   }
}
```

```css
.wheel {
  border: 2px solid black;
  border-radius: 50%;
  margin-left: 50px;
  position: absolute;
  height: 55vw;
  width: 55vw;
  max-width: 500px;
  max-height: 500px;
  animation-name: wheel;
  animation-duration: 10s;
}
```

```css
.wheel {
  border: 2px solid black;
  border-radius: 50%;
  margin-left: 50px;
  position: absolute;
  height: 55vw;
  width: 55vw;
  max-width: 500px;
  max-height: 500px;
  animation-name: wheel;
  animation-duration: 10s;
  animation-iteration-count: infinite;
  animation-timing-function: linear;
}
```

```css
@keyframes cabins {
   0% {
     transform: rotate(0deg);
   }

   100% {
     transform: rotate(-360deg);
   }
}
```

```css
.cabin {
  background-color: red;
  width: 20%;
  height: 20%;
  position: absolute;
  border: 2px solid;
  transform-origin: 50% 0%;
  animation: cabins 10s linear infinite;  
}
```

```css
.cabin {
  background-color: red;
  width: 20%;
  height: 20%;
  position: absolute;
  border: 2px solid;
  transform-origin: 50% 0%;
  animation: cabins 10s ease-in-out infinite;
}
```

```css
@keyframes cabins {
  0% {
    transform: rotate(0deg);
    background-color: yellow;
  }

  100% {
    transform: rotate(-360deg);
  }
}
```

```css
@keyframes cabins {
  0% {
    transform: rotate(0deg);
    background-color: yellow;
  }

  50% {
    background-color: purple;
  }

  100% {
    transform: rotate(-360deg);
  }
}
```

```css
@keyframes cabins {
  0% {
    transform: rotate(0deg);
  }

  50% {
    background-color: purple;
  }

  100% {
    transform: rotate(-360deg);
  }
}
```

```css
@keyframes cabins {
  0% {
    transform: rotate(0deg);
  }

  25%{
    background-color: yellow;
  }

  50% {
    background-color: purple;
  }

  100% {
    transform: rotate(-360deg);
  }
}
```

```css
@keyframes cabins {
  0% {
    transform: rotate(0deg);
  }

  25% {
    background-color: yellow;
  }

  50% {
    background-color: purple;
  }

  75% {
    background-color: yellow;
  }
  
  100% {
    transform: rotate(-360deg);
  }
}
```