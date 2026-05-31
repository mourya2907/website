# Ex.06 Restaurant Website

# AIM:
To develop a static Restaurant website to display the food items and services provided by them.

# DESIGN STEPS:
## Step 1:
Requirement collection.

## Step 2:
Creating the layout using HTML and CSS.

## Step 3:
Updating the sample content.

## Step 4:
Choose the appropriate style and color scheme.

## Step 5:
Validate the layout in various browsers.

## Step 6:
Validate the HTML code.

## Step 7:
Publish the website in the given URL.

# PROGRAM:
~~~
home.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>VEG RESTAURANT</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: sans-serif;
      color: black;
      background-color:white;
    }
    .banner {
      background-image: url("C:/Users/B.NAVASRI/Downloads/background.jpg");
      background-size: cover;
      background-position: center;
      background-repeat: no-repeat;
      text-align: center;
      color: white;
      padding: 120px 20px;
      position: relative;
    }

    .banner::before {
      content: "";
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background-color: rgba(0, 0, 0, 0.4);
      z-index: 0;
    }

    .banner h1, .banner p {
      position: relative;
      z-index: 1;
    }

    .banner h1 {
      font-size: 3em;
      margin-bottom: 10px;
    }

    .banner p {
      font-size: 1.2em;
    }

    .sections {
      display: flex;
      justify-content: space-around;
      flex-wrap: wrap;
      padding: 60px 20px;
      gap: 30px;
    }

    .card {
      background-color: white;
      border-radius: 8px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      width: 300px;
      text-align: center;
      padding: 20px;
      transition: transform 0.3s ease;
    }

    .card:hover {
      transform: scale(1.05);
    }

    .card img {
      width: 100%;
      border-radius: 6px;
    }

    .card h2 {
      margin: 15px 0 10px;
      font-size: 1.4em;
    }

    .card a {
      display: inline-block;
      margin-top: 10px;
      padding: 10px 15px;
      background-color: orangered;
      color: white;
      text-decoration: none;
      border-radius: 4px;
    }

    .card a:hover {
      background-color: orangered;
    }
  </style>
</head>
<body>

  <header class="banner">
    <h1>FOOD HUB</h1>
    <p>FLAT 30% OFF ON WEEKENDS</p>
  </header>

  <section class="sections">
    <div class="card">
      <h2>OUR MENU CARD</h2>
      <img src="C:/Users/B.NAVASRI/Downloads/menu.jpeg" alt="Menu">
      <p>Discover the authentic taste of India with our vibrant, spice-rich menu crafted to delight every palate.</p>
      <a href="menu.html">View Menu</a>
    </div>

    <div class="card">
      <h2>BOOK TABLE NOW</h2>
      <img src="C:/Users/B.NAVASRI/Downloads/plate.webp" alt="Book Table">
      <p>Reserve your seat now and let us treat you to an unforgettable dining experience filled with authentic flavors and warm hospitality.</p>
      <a href="book.html">Book Table Now</a>
    </div>


      <div class="card">
      <h2>ADMINISTRATION DETAILS</h2>
      <img src="c:\Users\B.NAVASRI\Downloads\administer.jpg" alt="administration details">
      <p>Hotel administration is the process of managing hotel operations to ensure smooth service, guest satisfaction, and profitability.</p>
      <a href="administer.html">CLICK HERE</a>
    </div>

    <div class="card">
      <h2>OPENING HOURS</h2>
      <img src="C:/Users/B.NAVASRI/Downloads/hotel.webp" alt="Opening Hours">
      <p>Weekdays: 9.00 am to 9.00 pm</p>
      <p>Weekends: 10.00 am to 5.00 pm</p>
      <a href="contact.html">CONTACT US</a>
    </div>

  </section>

</body>
</html>

menu.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Menu Card</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', sans-serif;
            height: 100vh;
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            align-items: flex-start;
            padding-top: 60px;
            color: white;
            position: relative;
            overflow: hidden;
        }
        body::before {
            content: "";
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-image: url('C:/Users/B.NAVASRI/Downloads/background.jpg');
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
            filter: darken(2px) brightness(0.6);
            z-index: -1;
        }

        .menu-card {
            background-color: rgba(0, 0, 0, 0.7);
            border-radius: 10px;
            padding: 20px;
            margin: 20px;
            width: 320px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.4);
        }

        .menu-card h1 {
            text-align: center;
            color:pink;
            margin-bottom: 20px;
            font-size: 28px;
            text-transform: uppercase;
        }

        .menu-item {
            display: flex;
            align-items: center;
            justify-content: space-between;
            margin-bottom: 15px;
            padding: 10px;
            border-bottom: 1px dashed pink;
        }

        .menu-item img {
            width: 60px;
            height: 60px;
            object-fit: cover;
            border-radius: 8px;
            margin-right: 15px;
        }

        .item-details {
            flex-grow: 1;
        }

        .item-name {
            font-size: 18px;
            color: white;
        }

        .item-price {
            font-weight: bold;
            color:white;
        }
    </style>
</head>
<body>

    <div class="menu-card">
        <h1>BREAKFAST</h1>
        <div class="menu-item">
            <img src="c:\Users\B.NAVASRI\Downloads\idly.jpeg" alt="Idly">
            <div class="item-details"><div class="item-name">Idly</div></div>
            <div class="item-price">Rs. 50</div>
        </div>

        <div class="menu-item">
            <img src="c:\Users\B.NAVASRI\Downloads\parrota.avif" alt="Parotta">
            <div class="item-details"><div class="item-name">Parotta</div></div>
            <div class="item-price">Rs. 70</div>
        </div>

        <div class="menu-item">
            <img src="c:\Users\B.NAVASRI\Downloads\masala dosa.webp" alt="Masala Dosa">
            <div class="item-details"><div class="item-name">Masala Dosa</div></div>
            <div class="item-price">Rs. 100</div>
        </div>

        <div class="menu-item">
            <img src="c:\Users\B.NAVASRI\Downloads\idiyapam.webp" alt="Idiyappam">
            <div class="item-details"><div class="item-name">Idiyappam</div></div>
            <div class="item-price">Rs. 60</div>
        </div>
    </div>

    <div class="menu-card">
        <h1>LUNCH</h1>
        <div class="menu-item">
            <img src="c:\Users\B.NAVASRI\Downloads\veg briyani.avif" alt="Veg Briyani">
            <div class="item-details"><div class="item-name">Veg Briyani</div></div>
            <div class="item-price">Rs. 150</div>
        </div>

        <div class="menu-item">
            <img src="c:\Users\B.NAVASRI\Downloads\Fried-Rice-11.jpg" alt="Fried Rice">
            <div class="item-details"><div class="item-name">Fried Rice</div></div>
            <div class="item-price">Rs. 160</div>
        </div>

        <div class="menu-item">
            <img src="c:\Users\B.NAVASRI\Downloads\isolated-traditional-indian-thali-meal-free-photo.jpg" alt="Meals">
            <div class="item-details"><div class="item-name">Meals</div></div>
            <div class="item-price">Rs. 200</div>
        </div>

        <div class="menu-item">
            <img src="c:\Users\B.NAVASRI\Downloads\bisi bele bath.jpg" alt="Sambar Rice">
            <div class="item-details"><div class="item-name">Sambar Rice</div></div>
            <div class="item-price">Rs. 150</div>
        </div>
    </div>

    <div class="menu-card">
        <h1>DESSERT</h1>
        <div class="menu-item">
            <img src="c:\Users\B.NAVASRI\Downloads\fruit cake.webp" alt="Fruit Cake">
            <div class="item-details"><div class="item-name">Fruit Cake</div></div>
            <div class="item-price">Rs. 250</div>
        </div>

        <div class="menu-item">
            <img src="c:\Users\B.NAVASRI\Downloads\fruit tart.webp" alt="Fruit Tart">
            <div class="item-details"><div class="item-name">Fruit Tart</div></div>
            <div class="item-price">Rs. 200</div>
        </div>

        <div class="menu-item">
            <img src="c:\Users\B.NAVASRI\Downloads\cheesecake.webp" alt="Cheesecake">
            <div class="item-details"><div class="item-name">Cheesecake</div></div>
            <div class="item-price">Rs. 180</div>
        </div>

        <div class="menu-item">
            <img src="c:\Users\B.NAVASRI\Downloads\chocolate lava cake.webp" alt="Lava Cake">
            <div class="item-details"><div class="item-name">Lava Cake</div></div>
            <div class="item-price">Rs. 280</div>
        </div>
    </div>

</body>
</html>

book.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Restaurant Booking Form</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', sans-serif;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            position: relative;
            color: white;
            overflow: hidden;
        }

        body::before {
            content: "";
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-image: url('C:/Users/B.NAVASRI/Downloads/background.jpg');
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
            filter: darken(3px) brightness(0.6);
            z-index: -1;
        }

        .booking-form {
            background-color: rgba(0, 0, 0, 0.7);
            backdrop-filter: blur(10px);
            border-radius: 15px;
            padding: 40px;
            width: 400px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.4);
        }

        .booking-form h2 {
            text-align: center;
            margin-bottom: 25px;
            font-size: 28px;
            color: white;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .form-group {
            margin-bottom: 15px;
        }

        label {
            display: block;
            font-weight: bold;
            margin-bottom: 6px;
            color: white;
        }

        input, select, textarea {
            width: 100%;
            padding: 10px;
            border: none;
            border-radius: 6px;
            font-size: 16px;
            box-sizing: border-box;
        }

        input:focus, select:focus, textarea:focus {
            outline: none;
            border: 2px solid yellow;
        }

        textarea {
            resize: none;
            height: 80px;
        }

        button {
            width: 100%;
            padding: 12px;
            background-color:yellow;
            border: none;
            border-radius: 6px;
            font-size: 18px;
            font-weight: bold;
            color: #333;
            cursor: pointer;
            transition: 0.3s ease;
        }

        button:hover {
            background-color:yellow;
        }
    </style>
</head>
<body>

    <form class="booking-form">
        <h2>Book Your Table</h2>

        <div class="form-group">
            <label for="name">Full Name:</label>
            <input type="text" id="name" placeholder="Enter your name" required>
        </div>

        <div class="form-group">
            <label for="email">Email Address:</label>
            <input type="email" id="email" placeholder="Enter your email" required>
        </div>

        <div class="form-group">
            <label for="phone">Phone Number:</label>
            <input type="tel" id="phone" placeholder="Enter your phone number" required>
        </div>

        <div class="form-group">
            <label for="guests">Number of Guests:</label>
            <select id="guests" required>
                <option value="">Select</option>
                <option>1</option>
                <option>2</option>
                <option>3–4</option>
                <option>5–6</option>
                <option>7–10</option>
            </select>
        </div>

        <div class="form-group">
            <label for="date">Date:</label>
            <input type="date" id="date" required>
        </div>

        <div class="form-group">
            <label for="time">Time:</label>
            <input type="time" id="time" required>
        </div>

        <div class="form-group">
            <label for="requests">Special Requests:</label>
            <textarea id="requests" placeholder="Any special instructions..."></textarea>
        </div>

        <button type="submit">Book Table</button>
    </form>

</body>
</html>

administer.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ADMINISTRATION</title>
    <style>
        body {

            background-image: url('c:/Users/B.NAVASRI/Downloads/background.jpg');
            background-size: cover;      
            background-position: center; 
            background-repeat: no-repeat;
            background-attachment: fixed; 
            padding: 20px;
            font-family: Arial, sans-serif;
        }

        .grid-container {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
            justify-items: center;
        }

        .image-box {
            border: 2px solid grey;
            border-radius: 10px;
            padding: 10px;
            background-color: rgba(255, 255, 255, 0.8); 
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
            width: 250px;
            text-align: center;
        }

        .image-box img {
            max-width: 100%;
            height: auto;
            border-radius: 5px;
        }
    </style>
</head>
<body>
    <div class="grid-container">
        <div class="image-box"><img src="c:/Users/B.NAVASRI/Downloads/chef1.jpeg"><h1>HEAD CHEF</h1></div>
        <div class="image-box"><img src="c:/Users/B.NAVASRI/Downloads/chef2.jpeg"><h1>HEAD CHEF</h1></div>
        <div class="image-box"><img src="c:/Users/B.NAVASRI/Downloads/chef3.jpeg"><h1>HEAD CHEF</h1></div>
        <div class="image-box"><img src="c:/Users/B.NAVASRI/Downloads/chef4.jpeg"><h1>CHEF</h1></div>
        <div class="image-box"><img src="c:/Users/B.NAVASRI/Downloads/chef5.jpeg"><h1>CHEF</h1></div>
        <div class="image-box"><img src="c:/Users/B.NAVASRI/Downloads/chef 6.webp"><h1>CHEF</h1></div>
    </div>

    
</body>
</html>

contact.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Us - Restaurant</title>
    <style>
        
        html, body {
            height: 100%;
            margin: 0;
            font-family: Arial, sans-serif;
        }

        body {
            background-image: url('c:/Users/B.NAVASRI/Downloads/background.jpg');
            background-size: cover;        
            background-position: center;
            background-repeat: no-repeat;  
            display: flex;
            justify-content: center;       
            align-items: center;          
            padding: 20px;
        }

        .container {
            max-width: 600px;
            background-color: rgba(255, 255, 255, 0.9); 
            padding: 30px;
            border-radius: 10px;
            text-align: center;
        }

        h1 {
            margin-bottom: 20px;
        }

        p {
            font-size: 18px;
            margin: 10px 0;
        }

        a {
            color: blue;
            text-decoration: none;
        }

        a:hover {
            text-decoration: underline;
        }

    </style>
</head>
<body>

    <div class="container">
        <h1>Contact Us</h1>
        <p>Phone: <a href="tel:+911234567890">+91 12345 67890</a></p>
        <p>Email: <a href="mailto:info@restaurant.com">info@restaurant.com</a></p>
        <p>Address: 123 Food Street, City, Country</p>
    </div>

</body>
</html>
~~~
# OUTPUT:
<img width="1917" height="1097" alt="Screenshot 2025-10-04 211310" src="https://github.com/user-attachments/assets/ff4b582d-8add-449d-9c33-9a475a93f9b9" />

<img width="1920" height="1140" alt="Screenshot 2025-10-04 211447" src="https://github.com/user-attachments/assets/a0b65dd5-d56a-49b5-89f9-6441752b963f" />





<img width="1920" height="1136" alt="Screenshot 2025-10-04 211507" src="https://github.com/user-attachments/assets/84bf07e3-2dd7-4587-b993-d234bcb76ac0" />


<img width="1920" height="1133" alt="Screenshot 2025-10-04 211523" src="https://github.com/user-attachments/assets/00602b43-4cd4-408e-ac54-85826e89b2d6" />




<img width="1920" height="1126" alt="Screenshot 2025-10-04 211627" src="https://github.com/user-attachments/assets/8a115cff-a2f1-4821-a370-8e7f673d5f92" />


# RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
