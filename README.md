# Ex.08 Design of Interactive Image Gallery
## Date:
17/12/2024

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
<html>
<head>
    <title>Image Gallery</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }

        .gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .gallery img {
            width: 220px;
            height: 400px;
            margin: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            cursor: pointer;
        }

        .modal {
            display: none;
            position: fixed;
            z-index: 1;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            overflow: auto;
            background-color: rgba(0, 0, 0, 0.5);
        }

        .modal-content {
            background-color:black;
            margin: 15% auto;
            padding: 20px;
            border: 1px solid #888;
            width: 80%;
        }

        .modal-content img {
            width: 100%;
        }

        .close {
            color: #aaa;
            float: right;
            font-size: 28px;
            font-weight: bold;
            cursor: pointer;
        }

        .close:hover,
        .close:focus {
            color: black;
            text-decoration: none;
            cursor: pointer;
        }
        
    </style>
</head>
<body>

    <div class="gallery">
        <img src="sunrise.jpeg" alt="Sunrise" onclick="openModal(this)">
        <img src="sunset.jpeg" alt="Sunset" onclick="openModal(this)">
        <img src="moon.jpeg" alt="Moon" onclick="openModal(this)">
        <img src="crescent.jpeg" alt="crescent" onclick="openModal(this)">
        <img src="tree.jpeg" alt="tree" onclick="openModal(this)">
        </div>

    <div id="myModal" class="modal">
        <div class="modal-content">
            <span class="close">&times;</span>
            <img id="modalImg">
        </div>
    </div>

    <script>
        function openModal(img) {
            var modal = document.getElementById("myModal");
            var modalImg = document.getElementById("modalImg");
            modal.style.display = "block";
            modalImg.src = img.src;
        }

        var span = document.getElementsByClassName("close")[0];
        span.onclick = function() {
            document.getElementById("myModal").style.display = "none";
        }
    </script>
    <footer align="center">
        <h4>Designed And Developed By Hiba Nasreen M</h4>
    </footer>

</body>
</html>
```

## OUTPUT:
![alt text](<Screenshot 2024-12-17 141259.png>)
![alt text](<Screenshot 2024-12-17 142055.png>)
![alt text](<Screenshot 2024-12-17 142108-1.png>)
![alt text](<Screenshot 2024-12-17 142123-1.png>)
![alt text](<Screenshot 2024-12-17 142140-1.png>)
![alt text](<Screenshot 2024-12-17 142154-1.png>)

## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
