<video src="" controls></video>
 <video src="" controls autoplay></video>

<!-- if you want a text to remain fixed on top of a page. Use position(fixed)-->
position: fixed;
top: 0;
margin: 0;
width: 100%;
text-align: center;


<!-- if you want a text to remain fixed but still move the text around i.e position anywhere. Use position(relative) -->
position: relative;
top: 10 px;
left: 100px;


# CSS BACKGROUND
background: rgba(255, 255, 255, 0.6);     - Background will look transparent in way 
body {
  background-size: cover;
}       - For image to to cover the size of the screen and remain fixed even when spliting that tab


background: linear-gradient(to right,blue, violet);       - Color will be both blue-violet with blue on the left and violet on the right hence it means it showcases  # background: linear-gradient (Direction, From, To);

background: linear-gradient(200deg,blue, violet);     - Color will change with a pattern of blue-violet



# TRANSITIONS
img {
 <!-- Transition supports the transform code in the img:hover, You can adjust the time in ms in which the image transforms -->
  transition: all 1500ms ease;
  opacity: 1;
  color: blue;
  display block 

}

img:hover {
<!-- Scale transforms the image by increasing it whenever you hover on it -->
<!-- Translate moves the image all across the screen when you hover on it  -->
  transform: scale(2) rotate(620deg) translate(200px, 400px);
  opacity: 0.7;
  color: red;
}




<!-- Why the Parent Div matters for your CSS
When you set your CSS like this:

The Parent (.one, .two, etc.) sets the boundary: You told the .one div to be width: 8%. This means that specific "box" on your screen is quite small.

The Child (img) fills that boundary: By setting img { width: 100%; }, you aren't telling the image to be 100% of the whole screen; you are telling it to be 100% of its parent.

The Result: The image shrinks down until it perfectly fits inside that 8% wide box you created. -->



# GRIDS

img {
  width: 300px;
}

.image-gallery {
  display: grid;
  <!-- Creates 2 Columns, each 300px to fit the width of the image in this case,,, you can aslo use 'grid-template-columns: repeat(2, 300px);' -->
  grid-template-columns: 300px 300px;
  <!-- gap leaves a space between the images in this case -->
  gap: 20px;
}

2. 
.container {
   <!-- Creates 4 rows, each exactly 150px tall -->
  display: grid;
  grid-template-rows: repeat(4, 150px);
}

.container {
  <!-- If you want three rows with specific heights, use three values in grid-template-rows -->
  display: grid;
  grid-template-rows: 100px 300px 100px;
}


# HTML Class Manipulation
<!-- // Selecting by Tag Name -->
const heading = document.querySelector("h1");

<!-- // Selecting by Class (use a dot) -->
const firstImage = document.querySelector(".one");

<!-- // Selecting by ID (use a hashtag) -->
const mainTitle = document.querySelector("#header-title");


2. 
const box = document.querySelector(".one");
<!-- // This replaces whatever was in the div with a new heading -->
box.innerHTML = "<h2>New Title</h2>";

<!-- .classList (The Styling/State)
This is an object that lets you manage the CSS classes attached to the element. It doesn't change the text inside; it changes the "tags" or "labels" the element has so that your CSS can style it differently.

Used for: Adding animations, hiding/showing elements, or changing colors based on a click.
Common Methods: .add(), .remove(), and .toggle() e.g; -->
const box = document.querySelector(".one");
<!-- // This adds the "active" class from your CSS to the box -->
<!-- An "active class" is just a CSS class that you create to represent a change in state—like when a button is clicked, a menu is open, or a photo is selected etc (it is like an "ON" switch to change something) hence the change is permanent until the page is refreshed. -->
box.classList.add("active");













ul/li.shecodes*10

                <input type="file">
                 <input type="text">
                 <input type="number">
                <input type="email">
                <input type="date">
                <input type="password">
               <input type="datetime-local">

# replace()
let city = "Montreal";
city = city.replace("e", "é"); =   // "Montréal"

# Given a variable country set to "Guinea Bissau", replace the space by a "-"
country = country.replace(/ /g, "-")


# trim
let city = " Montreal  ";
city = city.trim(); // "Montreal"

# toUpperCase()
let city = "Montreal";
city = city.toUpperCase(); // "MONTREAL"

# string concentration
let firstName = "Julie";
let lastName = "Johnson";
let fullName = firstName + " " + lastName; // "Julie Johnson"

//or
let fullName = `${firstName} ${lastName}`;

# round, floor , ceil, min, random
Math.round(4.7) // 5
Math.floor(4.7) // 4
Math.ceil(4.7) // 5
Math.min(2, 5, 1) // 1
Math.random(); // 0.47231881595639025    # generates a pseudo-random floating-point number that is greater than or equal to 0 and strictly less than 1

# Arrays and loops
# while loop
  let times = 0;
  while (times < 10) {
  console.log(times);
  times = times + 1;
    }
# forEach loop
  let fruits = ['apples', 'oranges', 'bananas'];
   fruits.forEach(function(fruit) {
  alert("I have " + fruit + " in my shopping bag");
  });

// or 
   function buyFruit(fruit){
    alert (fruit);
   }
     let fruits = ['apples', 'oranges', 'bananas'];
     fruits.forEach(buyFruit);

# for loop
    for (let i = 0; i < 10; i++) {
    console.log("i is " + i);
    }

    const myList = ["apples", "bananas", "oranges", "mangoes", "strawberry"]
    for (let i = 0; i < myList.length; i++) {
    alert("I have " + myList[i] + " in my shopping bag");
    }

# pop & shift
pop() - removes last item in an array
shift()- removes 1st item in an array
  e.g fruits.shift()   // removes apples from the list above for fruits
# push & unshift
push - adds an element to the end of an array
   e.g fruits.push("guava")   // will add guava at the end of the list
unshift - adds ana elememt at the beginning of an array# CSS-Background
