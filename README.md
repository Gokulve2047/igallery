# Ex.08 Design of Interactive Image Gallery
## Date:17:12:2024

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
            body {
                font-family: Arial, sans-serif; /* Changed to generic font */
                display: flex;
                flex-direction: column;
                align-items: center;
                margin: 0;
                background-color: black; /* Changed to black */
                color: #1a8ccf;
            }

            h1 {
                margin-top: 20px;
                color: rgb(21, 122, 231);
                font-size: xx-large;
                font-style: italic;
                text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5);
            }

            .Gallery {
                display: flex;
                flex-wrap: wrap; /* Allows the gallery to adjust dynamically */
                gap: 20px;
                max-width: 800px;
                margin-top: 50px;
                justify-content: center;
            }

            .Gallery img {
                width: 200px;
                height: 200px;
                border: 3px solid #d1bf20;
                border-radius: 10px;
                box-shadow: 0 4px 8px rgba(230, 6, 6, 0.834);
                cursor: pointer;
                transition: transform 0.3s ease, box-shadow 0.3s ease;
            }

            .Gallery img:hover {
                transform: scale(1.1); /* Zoom effect */
                box-shadow: 0 6px 12px rgba(218, 12, 12, 0.4);
            }

            footer {
                position: fixed;
                bottom: 0;
                width: 100%;
                background-color: rgb(11, 11, 11); /* Changed to black */
                text-align: center;
                color: aliceblue;
                padding: 10px 20px;
                font-family: Arial, sans-serif;
                font-size: 16px;
                text-shadow: 1px 1px 2px rgb(244, 242, 242);
            }

            footer span {
                font-weight: bold;
            }
        </style>
    </head>
    <body>
        <h1>Interactive Image Gallery</h1>
        <div class="Gallery">
            <img src="Screenshot 2024-12-17 141628.png" onclick="openImage(this.src)">
            <img src="Screenshot 2024-12-17 141643.png" alt="Image 2" onclick="openImage(this.src)">
            <img src="Screenshot 2024-12-17 141655.png" alt="Image 3" onclick="openImage(this.src)">
            <img src="Screenshot 2024-12-17 141711.png" alt="Image 5" onclick="openImage(this.src)">
            <img src="Screenshot 2024-12-17 143546.png" alt="Image 4" onclick="openImage(this.src)">
            <img src="Screenshot 2024-12-17 204645.png" alt="Image 6" onclick="openImage(this.src)">
            <img src="Screenshot 2024-12-17 205124.png" alt="Image 7" onclick="openImage(this.src)">
        </div>

        <script>
            function openImage(src) {
                window.open(src, "_blank");
            }
        </script>

        <footer>
            Designed & Developed by <span>GOKUL V E</span>
        </footer>
    </body>
</html>
```

## OUTPUT:
![alt text](<goku/igallery/static/Screenshot 2024-12-17 205455.png>)

## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
