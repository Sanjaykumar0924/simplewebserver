# EX01 Developing a Simple Webserver
## Date:

## AIM:
To develop a simple webserver to serve html pages.

## DESIGN STEPS:
### Step 1: 
HTML content creation.

### Step 2:
Design of webserver workflow.

### Step 3:
Implementation using Python code.

### Step 4:
Serving the HTML pages.

### Step 5:
Testing the webserver.

## PROGRAM:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">
    <style>
    a{
        padding: 10px;text-decoration: none;color: brown;font-weight: bold;  
    }
    i:hover{
        color: grey;
    }
    a:hover{
        color: rgb(11, 54, 87);
    }
    input{
            border-radius: 20px;
            width:240px;
            height: 40px;
           border-image: auto;
           background-image: url(serach\ icon.png),url(cancel\ 1.png); background-size: 20px ;
           background-repeat: no-repeat;background-position: 1%,95%;background-color: antiquewhite;
           text-align: center;

        }
</style>

</head>
<body style="background-image: url(grey.webp);background-size: 100%;background-attachment: fixed; ">
    <div style="display: flex; height: 70px;background-color: antiquewhite;margin-top: 20px;margin-left: 20px;margin-right: 15px;">
        <div style="width: 30%;padding: 20px;">
            <i aria-setsize="20px" class="bi bi-amazon" style="margin: 7px;"></i>
            <i class="bi bi-whatsapp"  style="margin: 7px;"></i>
            <i class="bi bi-facebook" style="margin: 7px;"></i>
            <i class="bi bi-messenger" style="margin: 7px;"></i>
            <i class="bi bi-meta" style="margin: 7px;"></i>
        </div>
        
        <div style="width: 54%;padding-left: 19%;padding-top: 10px;font-style: italic;padding-top: 20px;">
<a  href="home page.html">Alumini</a>
<i class="bi bi-three-dots-vertical"></i>

<a    href="home.html">Events</a>
<i class="bi bi-three-dots-vertical"></i>
<a  href="best.html">cheer</a>
<i class="bi bi-three-dots-vertical"></i>
<a   href="">Log in</a>
<i class="bi bi-three-dots-vertical"></i>
<a  href="">SEC portal</a>
<i class="bi bi-three-dots-vertical"></i>

        </div>
        <div style="width: 18%; padding: 20px;border-radius: 10px;background-color: antiquewhite;">
            <form action="" style="width: 700px;">
                <input  style="border-radius: 15px;height: 30px;text-align: center;" type="text" name="search" placeholder="search">
            </form>
                    </div>
    </div>
    <div style="display: flex;height: 130px;margin-left: 50px; margin-right: 50px;background-color: rgb(250, 250, 250);" >
        <div style="width: 35%;"><img style="height: 125px; padding: 30px;" src="saveetha logo.png" alt=""></div>
        <div style="width: 60%;">
<div style="display: flex;padding: 15px;font-size:19px;padding-top: 30px;">
    <a href="">Home</a>
    <a href="">About</a>
    <a href="">Departments</a>
    <a href="">Life at SEC</a>
    <a href="">Admission</a>
    <a href="">Placements</a>
    <a href="">Research</a>
</div>
    </div>
        <div style="width: 15%;color: white;font-size: 20px;text-align: center;padding-top: 15px;clip-path: polygon(25% 0%,100% 0%,100% 100%,0%  100%);"class="bg-secondary">
       FOR<br>ADMISSION <br>   <i class="bi bi-whatsapp"  style="margin: 7px;"></i>9150184246
        </div>
        
    </div>
    <div style="display: flex; height: 1300px;margin-left: 50px;margin-right: 50px;">
        <div style="padding-top:10px ;margin-bottom: 10px;">
            <div class="card" style="width: 25rem;background-color: rgb(175, 8, 8);">
                <div class="card-body">
                  <h5 class="card-title" style="padding-left: 40px;font-size: 30px;color: white;"> ADMISSION ENQUIRY</h5>
                  <p class="card-text"> <br></p>
                  <a href="#" class="btn btn-primary" style="text-align: center;margin-left: 40px;background-color: white;color: rgb(153, 13, 13);" >APPLY NOW</a>
                </div>
              </div>
              <div class="card" style="width: 25rem;background-color: rgb(175, 8, 8);">
                <div class="card-body">
                  <h5 class="card-title" style="padding-left: 40px;font-size: 30px; color: white;" >CHAT WITH CLASS AMBASADOR</h5>
                  <p class="card-text"><br></p>
                <a href="#" class="btn btn-primary"  style="text-align: center;margin-left: 40px;background-color: white;color: rgb(153, 13, 13);" >KNOW MORE</a>
                </div>
              </div>
              <div class="card" style="width: 25rem;background-color:  rgb(175, 8, 8);">
                <div class="card-body">
                  <h5 class="card-title" style="padding-left: 40px;font-size: 30px;color: white;">BLOGS</h5>
                  <p class="card-text"><br>
                  </p>
                 <a href="#" class="btn btn-primary"  style="text-align: center;margin-left: 40px;background-color: white;color: rgb(153, 13, 13);" >KNOW MORE</a>
                </div>
              </div>
        </div>
        <div style="padding-left: 22px;padding-top: 10px;" >
            <div style="height: 900px" id="carouselExampleSlidesOnly" class="carousel slide" data-bs-ride="carousel">
                <div class="carousel-inner">
                  <div class="carousel-item active">
                    <img src="sav img 1.jpg" class="d-block w-100" alt="...">
                  </div>
                  <div class="carousel-item">
                    <img src="img 4.jpg" class="d-block w-100" alt="...">
                  </div>
                  <div class="carousel-item">
                    <img src="img 2.jpg" class="d-block w-100" alt="...">
                  </div>
                 
                </div>
        </div>
    </div>
   
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz" crossorigin="anonymous"></script>

    </body>
</html>

## OUTPUT:
![alt text](<Screenshot 2024-03-30 133202.png>)

## RESULT:
The program for implementing simple webserver is executed successfully.
