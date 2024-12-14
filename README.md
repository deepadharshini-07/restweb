# Ex.07 Restaurant Website
## Date:13:12:2024

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
```
index.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>FORK IT ALL</title>
    <link rel="stylesheet" href="trial.css">
</head>
<body>
    <header class="banner">
        <h1>Welcome to FORK IT ALL </h1>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="trial2.html">Menu</a></li>
                <li><a href="trial 3.html">Administration</a></li>
                <li><a href="trial4.html">Contact Us</a></li>
            </ul>
        </nav>
    </header>

    <section class="intro">
        <h2>Your Cravings Our Creations</h2>
        <p>More than a restaurant, it's an experience of taste and ambiance.</p>
    </section>

    <footer>
        <p>© 2024 DEEPADHARSHINI T</p>
    </footer>
</body>
</html>

trial.css
/* General Reset */
body {
    margin: 0;
    padding: 0;
    font-family: Arial, sans-serif;
    line-height: 1.6;
    color: #333;
    background-image: url('Background.png'); /* Replace with your image file path */
    background-size: cover; /* Ensures the image covers the entire screen */
    background-position: center; /* Centers the image */
    background-attachment: fixed; /* Makes the background fixed on scroll */
    background-repeat: no-repeat; /* Prevents repeating of the image */
}

/* Header Styling */
header.banner {
    background-color: #222;
    color: white;
    padding: 20px 10px;
    text-align: center;
}

header.banner h1 {
    margin: 0;
    font-size: 2.5em;
    letter-spacing: 2px;
}

header.banner nav ul {
    list-style: none;
    padding: 0;
    margin: 10px 0 0;
    display: flex;
    justify-content: center;
    gap: 20px;
}

header.banner nav ul li {
    display: inline;
}

header.banner nav ul li a {
    text-decoration: none;
    color: white;
    font-size: 1.2em;
    transition: color 0.3s;
}

header.banner nav ul li a:hover {
    color: #ff6347;
}

/* Intro Section */
section.intro {
    padding: 40px 20px;
    text-align: center;
    background-color: #fff;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    margin: 20px;
    border-radius: 10px;
}

section.intro h2 {
    font-size: 2em;
    color: #222;
    margin-bottom: 10px;
}

section.intro p {
    font-size: 1.1em;
    color: #555;
    margin: 0;
}

/* Footer Styling */
footer {
    text-align: center;
    padding: 10px 0;
    background-color: #222;
    color: white;
    position: relative;
    bottom: 0;
    width: 100%;
}

footer p {
    margin: 0;
    font-size: 0.9em;
}

/* Responsive Design */
@media (max-width: 768px) {
    header.banner nav ul {
        flex-direction: column;
        gap: 10px;
    }

    section.intro {
        margin: 10px;
    }
}

trial2.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Menu</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background-color: #f9f9f9;
            color: #333;
        }

        header.banner {
            background-color: #222;
            color: white;
            padding: 20px;
            text-align: center;
        }

        header.banner h1 {
            margin: 0;
        }

        header.banner nav ul {
            list-style: none;
            padding: 0;
            margin: 10px 0 0;
            display: flex;
            justify-content: center;
            gap: 20px;
        }

        header.banner nav ul li {
            display: inline;
        }

        header.banner nav ul li a {
            text-decoration: none;
            color: white;
            font-size: 1.2em;
            transition: color 0.3s;
        }

        header.banner nav ul li a:hover {
            color: #ff6347;
        }

        .menu {
            padding: 20px;
            text-align: center;
        }

        .menu h2 {
            font-size: 2em;
            color: #222;
            margin-bottom: 20px;
        }

        .menu-items {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            padding: 0;
        }

        .item {
            background: white;
            border-radius: 10px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            text-align: center;
            padding: 15px;
        }

        .item img {
            max-width: 100%;
            height: auto;
            border-bottom: 2px solid #f4f4f4;
        }

        .item h3 {
            font-size: 1.5em;
            margin: 10px 0;
        }

        .item p {
            font-size: 1.2em;
            color: #555;
        }

        footer {
            background-color: #222;
            color: white;
            text-align: center;
            padding: 10px 0;
            position: relative;
            bottom: 0;
            width: 100%;
        }

        footer p {
            margin: 0;
            font-size: 0.9em;
        }
    </style>
</head>
<body>
    <header class="banner">
        <h1>Menu</h1>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="trial2.html">Menu</a></li>
                <li><a href="trial 3.html">Administration</a></li>
                <li><a href="trial4.html">Contact Us</a></li>
            </ul>
        </nav>
    </header>

    <section class="menu">
        <h2>Our Delicious Menu</h2>
        <div class="menu-items">
            <div class="item">
                <img src="Margherita Pizza.png" alt="Margherita Pizza">
                <h3>Margherita Pizza</h3>
                <p>Rs. 250</p>
            </div>

            <div class="item">
                <img src="Veggie Burger.png" alt="Veggie Burger">
                <h3>Veggie Burger</h3>
                <p>Rs. 240</p>
            </div>

            <div class="item">
                <img src="Caesar Salad.png" alt="Caesar Salad">
                <h3>Caesar Salad</h3>
                <p>Rs. 300</p>
            </div>

            <div class="item">
                <img src="Spaghetti Carbonara.png" alt="Spaghetti Carbonara">
                <h3>Spaghetti Carbonara</h3>
                <p>Rs. 400</p>
            </div>

            <div class="item">
                <img src="Sushi Platter.png" alt="Sushi Platter">
                <h3>Sushi Platter</h3>
                <p>Rs. 850</p>
            </div>

            <div class="item">
                <img src="Chicken Tacos.png" alt="Chicken Tacos">
                <h3>Chicken Tacos</h3>
                <p>Rs. 250</p>
            </div>

            <div class="item">
                <img src="Grilled Salmon.png" alt="Grilled Salmon">
                <h3>Grilled Salmon</h3>
                <p>Rs. 1150</p>
            </div>

            <div class="item">
                <img src="Steak with Vegetables.png" alt="Steak with Vegetables">
                <h3>Steak with Vegetables</h3>
                <p>Rs. 1250</p>
            </div>

            <div class="item">
                <img src="Chocolate Cake.png" alt="Chocolate Cake">
                <h3>Chocolate Cake</h3>
                <p>Rs. 390</p>
            </div>

            <div class="item">
                <img src="Strawberry Cheesecake.png" alt="Strawberry Cheesecake">
                <h3>Strawberry Cheesecake</h3>
                <p>Rs. 500</p>
            </div>

            <div class="item">
                <img src="Mango Smoothie.png" alt="Mango Smoothie">
                <h3>Mango Smoothie</h3>
                <p>Rs. 150</p>
            </div>

            <div class="item">
                <img src="Cappuccino.png" alt="Cappuccino">
                <h3>Cappuccino</h3>
                <p>Rs. 200</p>
            </div>
        </div>
    </section>

    <footer>
        <p>&copy; 2024 Deepadharshini T</p>
    </footer>
</body>
</html>
trial 3.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Administration</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
        }

        .banner {
            background-color: #4CAF50;
            color: white;
            padding: 20px 0;
            text-align: center;
        }

        .banner h1 {
            margin: 0;
            font-size: 2.5em;
        }

        nav ul {
            list-style: none;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            background-color: #333;
        }

        nav ul li {
            margin: 0;
        }

        nav ul li a {
            display: block;
            padding: 10px 20px;
            text-decoration: none;
            color: white;
        }

        nav ul li a:hover {
            background-color: #4CAF50;
        }

        .team {
            padding: 40px 20px;
            text-align: center;
        }

        .team h2 {
            margin-bottom: 20px;
            font-size: 2em;
            color: #4CAF50;
        }

        .team-members {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
        }

        .member {
            background: white;
            border: 1px solid #ddd;
            border-radius: 10px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            width: 200px;
            padding: 20px;
            text-align: center;
        }

        .member img {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            object-fit: cover;
            margin-bottom: 15px;
        }

        .member h3, .member h4, .member h5, .member h6 {
            margin: 10px 0 5px;
            font-size: 1.2em;
            color: #333;
        }

        .member p {
            margin: 0;
            font-size: 0.9em;
            color: #666;
        }

        footer {
            text-align: center;
            background-color: #333;
            color: white;
            padding: 10px 0;
            margin-top: 40px;
        }
    </style>
</head>
<body>
    <header class="banner"> 
        <h1>Our Team</h1>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="trial2.html">Menu</a></li>
                <li><a href="trial 3.html">Administration</a></li>
                <li><a href="trial4.html">Contact Us</a></li>
            </ul>
        </nav>
    </header>

    <section class="team">
        <h2>Meet Our Team</h2>
        <div class="team-members">
            <div class="member">
                <img src="person 1.png" alt="Deepadharshini T">
                <h3>Deepadharshini T</h3>
                <p>Owner</p>
            </div>
            <div class="member">
                <img src="person 2.png" alt="Vijay">
                <h3>Vijay</h3>
                <p>Management Team</p>
            </div>
            <div class="member">
                <img src="person 3.png" alt="Mahi">
                <h3>Mahi</h3>
                <p>Management Team</p>
            </div>
            <div class="member">
                <img src="person 4.png" alt="Siva">
                <h3>Siva</h3>
                <p>Senior Chef</p>
            </div>
            <div class="member">
                <img src="person 5.png" alt="Virat">
                <h3>Virat</h3>
                <p>Chef</p>
            </div>
            <div class="member">
                <img src="person 6.png" alt="Jadeja">
                <h3>Jadeja</h3>
                <p>Chef</p>
            </div>
        </div>
    </section>

    <footer>
        <p>&copy; 2024 Deepadharshini T</p>
    </footer>
</body>
</html>
trial4.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Us</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
        }

        .banner {
            background-color: #4CAF50;
            color: white;
            padding: 20px 0;
            text-align: center;
        }

        .banner h1 {
            margin: 0;
            font-size: 2.5em;
        }

        nav ul {
            list-style: none;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            background-color: #333;
        }

        nav ul li {
            margin: 0;
        }

        nav ul li a {
            display: block;
            padding: 10px 20px;
            text-decoration: none;
            color: white;
        }

        nav ul li a:hover {
            background-color: #4CAF50;
        }

        .contact {
            padding: 40px 20px;
            text-align: center;
        }

        .contact h2 {
            margin-bottom: 20px;
            font-size: 2em;
            color: #4CAF50;
        }

        .contact p {
            font-size: 1.2em;
            margin: 10px 0;
            color: #555;
        }

        footer {
            text-align: center;
            background-color: #333;
            color: white;
            padding: 10px 0;
            margin-top: 40px;
        }
    </style>
</head>
<body>
    <header class="banner">
        <h1>Contact Us</h1>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="trial2.html">Menu</a></li>
                <li><a href="trial 3.html">Administration</a></li>
                <li><a href="trial4.html">Contact Us</a></li>
            </ul>
        </nav>
    </header>

    <section class="contact">
        <h2>Get in Touch</h2>
        <p><strong>Address:</strong> No.1, Washington Colony, Chrompet, Chennai-28</p>
        <p><strong>Phone:</strong> 9876543210</p>
        <p><strong>Email:</strong> forkitall@restaurant.com</p>
    </section>

    <footer>
        <p>&copy; 2024 Deepadharshini T</p>
    </footer>
</body>
</html>
```

## OUTPUT:
![alt text](<Screenshot 2024-12-13 185521.png>)

![alt text](<Screenshot 2024-12-13 185535.png>)

![alt text](<Screenshot 2024-12-13 185551.png>)

![alt text](<Screenshot 2024-12-13 185603.png>)


![alt text](<Screenshot 2024-12-13 185615.png>)

![alt text](<Screenshot 2024-12-13 185630.png>)



## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
