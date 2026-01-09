## Ex. 08 Diesign of Interacitve Image Gallery  
## Date:

## AIM:
To design a web application for an inteactive image gallery with minimum five images.

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

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Image Gallery</title> 
<style> 
         .gallery-container  
{ 
            position: relative; 
            max-width: 600px; 
            margin: auto; 
            background: white; 
            padding: 10px; 
            border-radius: 10px; 
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.2); 
         } 
         .gallery-image  
{ 
            width: 100%; 
            height: 600px; 
            object-fit: cover; 
            border-radius: 10px; 
         } 
         .caption  
{ 
            margin-top: 10px; 
            font-size: 18px; 
         } 
         .gallery-buttons  
{ 
            display: flex; 
            justify-content: space-between; 
            margin-top: 15px; 
         } 
         button  
{ 
            padding: 10px 20px; 
            cursor: pointer; 
            border: none; 
            border-radius: 5px; 
            background-color: #007BFF; 
            color: white; 
            transition: 0.3s; 
         } 
     </style> 
</head>  
<body> 
<div class="gallery-container"> 
<img id="galleryImage" class="gallery-image" src="sundar.png" height="50%" width="40%"> 
<div id="caption" class="caption">Caption for Image 1</div> 
<div class="gallery-buttons"> 
<button onclick="prevImage()">Previous</button> 
<button onclick="nextImage()">Next</button> 
</div> 
</div> 
<script> 
const images = [ 
{ src: "sundar.png", caption: "Sundar Pichai is the CEO of both Google and its parent company, Alphabet Inc. " }, 
{ src: "Ratan.png", caption: "Ratan Tata is the former chairman of Tata Sons, known for expanding the Tata Group globally and his philanthropy in India." }, 
{ src: "Bill.png", caption: "Bill Gates is the co-founder of Microsoft" }, 
{ src: "elon.png", caption: "Elon Musk is the CEO of Tesla and SpaceX" } 
]; 
let currentIndex = 0; 
function updateGallery( )  
{ 
document.getElementById("galleryImage").src = images[currentIndex].src; 
document.getElementById("caption").textContent = images[currentIndex].caption; 
} 
function nextImage( )  
{ 
currentIndex = (currentIndex + 1) % images.length; 
updateGallery( ); 
} 
function prevImage( )  
{ 
currentIndex = (currentIndex - 1 + images.length) % images.length; 
updateGallery( ); 
} 
</script> 
</body>
</html>
```

## OUTPUT:


<img width="1893" height="1029" alt="ig1" src="https://github.com/user-attachments/assets/63aa3b69-228c-47d6-ae09-049084a629e6" />
<img width="1913" height="1029" alt="ig2" src="https://github.com/user-attachments/assets/24bf840e-fa31-417a-a121-6f968604c4b2" />
<img width="1915" height="1018" alt="ig3" src="https://github.com/user-attachments/assets/4f76ca2b-7462-442c-a478-07a3c2462c75" />
<img width="1910" height="1030" alt="ig4" src="https://github.com/user-attachments/assets/2eb32af6-9bc2-4430-aca5-7ab40060a15a" />










## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
