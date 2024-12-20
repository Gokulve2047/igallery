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
    <meta name="description" content="An interactive gallery with images that open in a new tab.">
    <meta name="author" content="GOKUL V E">
    <title>Interactive Image Gallery</title>
    <style>
        /* General reset for margin and padding */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        /* Body styling */
        body {
            font-family: Arial, sans-serif;
            display: flex;
            flex-direction: column;
            align-items: center;
            margin: 0;
            background-size: cover;
            background-image: url("bg.jpg");
            background-position: center;
            background-repeat: no-repeat;
            background-attachment: fixed;
        }

        /* Title styling */
        h1 {
            margin-top: 20px;
            color: rgb(10, 10, 10);
            font-size: 2rem;
            font-style: italic;
            text-align: center;
        }

        /* Gallery container */
        .Gallery {
            display: flex;
            gap: 25px;
            max-width: 1000px;
            margin-top: 50px;
            justify-content: center;
            flex-wrap: wrap;
            padding: 20px;
            transition: all 0.3s ease;
        }

        /* Individual image styling */
        .Gallery img {
            cursor: pointer;
            transition: transform 0.3s ease-in-out, opacity 0.3s ease;
            border-radius: 10px;
            border: 3px solid transparent;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }

        /* Hover effects for images */
        .Gallery img:hover {
            transform: scale(1.1);
            opacity: 0.8;
            border-color: #00aaff;
            box-shadow: 0 8px 12px rgba(0, 0, 0, 0.2);
        }

        /* Footer styling */
        footer {
            bottom: 2%;
            position: fixed;
            width: 100%;
            background-image: url("https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSm18eBadaqCzW5XTKA-c434AR5co6NgyoT9w&s");
            text-align: center;
            font-family: Arial, sans-serif;
            color: rgb(232, 33, 33);
            left: 0%;
            background-size: cover;
            padding: 20px;
            font-size: 18px;
            text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.5);
        }

        /* Responsive design adjustments */
        @media (max-width: 768px) {
            h1 {
                font-size: 1.5rem;
            }

            .Gallery {
                gap: 15px;
                margin-top: 30px;
            }

            .Gallery img {
                width: 150px;
                height: 150px;
            }
        }

        @media (max-width: 480px) {
            .Gallery img {
                width: 100px;
                height: 100px;
            }

            footer {
                font-size: 16px;
                padding: 10px;
            }
        }

        /* Scrollbar styling */
        ::-webkit-scrollbar {
            width: 12px;
        }

        ::-webkit-scrollbar-thumb {
            background-color: #00aaff;
            border-radius: 6px;
        }

        ::-webkit-scrollbar-track {
            background: #f1f1f1;
        }
    </style>
</head>
<body>

    <h1>Interactive Image Gallery</h1>

    <div class="Gallery">
        <img src="Screenshot 2024-12-17 141628.png" alt="Gallery Image 1" width="200" height="200" onclick="openImage(this.src)">
        <img src="Screenshot 2024-12-17 141643.png" alt="Gallery Image 2" width="200" height="200" onclick="openImage(this.src)">
        <img src="Screenshot 2024-12-17 141655.png" alt="Gallery Image 3" width="200" height="200" onclick="openImage(this.src)">
        <img src="Screenshot 2024-12-17 204545.png" alt="Gallery Image 4" width="200" height="200" onclick="openImage(this.src)">
        <img src="Screenshot 2024-12-17 143546.png" alt="Gallery Image 5" width="200" height="200" onclick="openImage(this.src)">
        <img src="Screenshot 2024-12-17 204645.png" alt="Gallery Image 6" width="200" height="200" onclick="openImage(this.src)">
        <img src="Screenshot 2024-12-17 205124.png" alt="Gallery Image 7" width="200" height="200" onclick="openImage(this.src)">
    </div>

    <script>
        // Open image in a new tab when clicked
        function openImage(src) {
            window.open(src, "_blank");
        }
    </script>

    <footer>
        Designed & Developed by GOKUL V E
    </footer>

</body>
</html>
>

```
## OUTPUT:
![alt text](<Screenshot 2024-12-20 092112.png>)


## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
