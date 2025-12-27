# Ex.07 Design of Interactive Image Gallery
## Date:27-12-2025

## AIM:
To design a web application for an inteactive image gallery for a minimum five images with next and previous buttons.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM:

```
<html>
<head>
<title>Animal Image Gallery</title>
<link rel="stylesheet" href="gal.css">
</head>
<body>

<header>Animal Gallery</header>

<div class="container">
    <div class="gallery-box">
        <img id="galleryImage" src="animal1.jpg" alt="Animal Image">
        <p class="caption" id="caption">Lion</p>

        <div class="buttons">
            <button onclick="prev()">Previous</button>
            <button onclick="next()">Next</button>
        </div>
    </div>
</div>

<footer>
Designed by Divesh (25018935) &copy; 
</footer>

<script>
let gallery = [
    "lion.png",
    "ele.png",
    "gir.png",
    "panda.png"
];

let captions = [
    "Lion",
    "Elephant",
    "Giraffe",
    "Panda"
];

let index = 0;

function next(){
    index++;
    if(index >= gallery.length){
        index = 0;
    }
    document.getElementById("galleryImage").src = gallery[index];
    document.getElementById("caption").innerText = captions[index];
}

function prev(){
    index--;
    if(index < 0){
        index = gallery.length - 1;
    }
    document.getElementById("galleryImage").src = gallery[index];
    document.getElementById("caption").innerText = captions[index];
}
</script>

</body>
</html>
```


## OUTPUT:
![alt text](<Screenshot (35).png>)

![alt text](<Screenshot (36).png>)

![alt text](<Screenshot (37).png>)

![alt text](<Screenshot (38).png>)

![alt text](<Screenshot (39).png>)

## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
