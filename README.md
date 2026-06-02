# Ex.05 Book Front Cover Page Design
## Date:

## AIM:
To design a book front cover page using HTML and CSS.

## DESIGN STEPS:

### Step 1:
Create a Django Admin project.

### Step 2:
Create an app in the Django interface.

### Step 3:
Create a folder named 'static' in the app folder.

### Step 4:
Create a new HTML file in the static folder.

### Step 5:
Write the HTML code with relevant CSS properties.

### Step 6:
Choose the appropriate style and color scheme.

### Step 7:
Insert the images in their appropriate places.

### Step 8:
Publish the website in the LocalHost.

## PROGRAM:
index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>About the Book</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

<div class="container">

    <h1>About the Book</h1>

    <div class="line"></div>

    <p class="description">
        This book introduces the fundamentals of Web Application
        Development using HTML, CSS, JavaScript and Django.
        It provides students with practical knowledge for
        building modern websites and web applications.
    </p>

    <div class="quote">
        "Learning never exhausts the mind."
    </div>

    <div class="author-card">

        <img src="photo.jpeg" alt="Author">

        <div class="author-info">
            <h3>Muhammad Irfan M</h3>
            <p>B.E. Computer Science and Engineering</p>
            <p>Saveetha Engineering College</p>
        </div>

    </div>

    <div class="publisher">

        <div>
            <h3>SEC Publications</h3>
            <p>Chennai, Tamil Nadu</p>
        </div>

        <div class="price">
            ₹399
        </div>

    </div>

</div>

</body>
</html>
```
style.css
```
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, sans-serif;
}

body{
    background:#e6f2ff;
    display:flex;
    justify-content:center;
    align-items:center;
    height:100vh;
}

.container{
    width:500px;
    height:700px;

    background-image:url("bg.jpg");
    background-size:cover;
    background-position:center;

    border:5px solid #003366;
    padding:25px;

    position:relative;
}

.container::before{
    content:"";
    position:absolute;
    inset:0;
    background:rgba(255,255,255,0.85);
}

.container *{
    position:relative;
    z-index:1;
}

h1{
    text-align:center;
    color:#003366;
}

.line{
    width:100%;
    height:2px;
    background:#003366;
    margin:10px 0 20px;
}

.description{
    text-align:justify;
    line-height:1.8;
    margin-bottom:25px;
}

.quote{
    background:#d9ecff;
    border-left:5px solid #003366;
    padding:15px;
    font-style:italic;
    margin-bottom:25px;
}

.author-card{
    display:flex;
    gap:15px;
    align-items:center;

    border:2px solid #003366;
    padding:15px;
    background:white;

    margin-bottom:40px;
}

.author-card img{
    width:100px;
    height:120px;
    object-fit:cover;
    border:2px solid #003366;
}

.author-info h3{
    color:#003366;
    margin-bottom:8px;
}

.publisher{
    border:2px solid #003366;
    background:white;

    display:flex;
    justify-content:space-between;
    align-items:center;

    padding:15px;

    position:absolute;
    bottom:25px;
    left:25px;
    right:25px;
}

.price{
    font-size:24px;
    font-weight:bold;
    color:#003366;
}
```



## OUTPUT:
<img width="1914" height="1019" alt="Screenshot 2026-06-02 111601" src="https://github.com/user-attachments/assets/9799ce0c-75a2-45b8-bd6f-ddb6d72e6ca4" />



## RESULT:
The program for designing book front cover page using HTML and CSS is completed successfully.
