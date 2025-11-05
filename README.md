# Ex.07 Restuarant Website
## Date:5.11.2025

## AIM:
To develop a static Resturant website to display the menu and services provided by the resturant.

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
    <title>Native Kitchen - Home</title>
    <link href="https://fonts.googleapis.com/css?family=Montserrat:700,400&display=swap" rel="stylesheet">
    <style>
        body {
            margin: 0;
            font-family: 'Montserrat', Arial, sans-serif;
            background: #dfd764;
            color: #232323;
        }
        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 28px 60px;
            background: #f5f5ef;
        }
        .logo {
            display: flex;
            align-items: center;
            font-size: 2.1rem;
            font-weight: 700;
        }
        .logo-img {
            height: 50px;
            width: 50px;
            border-radius: 50%;
            object-fit: cover;
            margin-right: 16px;
            border: 2px solid #ffe8b2;
        }
        nav {
            display: flex;
            gap: 38px;
        }
        nav a {
            text-decoration: none;
            color: #232323;
            font-weight: 500;
            font-size: 1.1rem;
            position: relative;
        }
        nav a.active, nav a:hover {
            color: #658635;
        }
        .hero {
            display: flex;
            align-items: center;
            gap: 60px;
            padding: 64px 10vw;
        }
        .hero-img {
            display: flex;
            align-items: center;
            justify-content: center;
        }
        .hero-img img {
            width: 450px;
            height: auto;
            border-radius: 22px;
            border: 3px solid #f0c152;
            box-shadow: 0 4px 30px rgba(101, 134, 53, 0.09);
        }
        .hero-content {
            max-width: 370px;
        }
        .hero-content h1 {
            font-size: 2.2rem;
            margin-bottom: 10px;
            font-weight: 700;
        }
        .hero-content p {
            font-size: 1.2rem;
            color: #444;
        }
        @media (max-width: 900px) {
            .hero {
                flex-direction: column;
                gap: 32px;
                padding: 32px 5vw;
            }
            .hero-img img {
                width: 80vw;
                max-width: 420px;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="logo">
            <img src="C:\Users\admin\OneDrive\Desktop\sem 3\web\exp7\softweb\generated-image (4).png" alt="Native Kitchen Logo" class="logo-img">
            Native Kitchen
        </div>
        <nav>
            <a href="index.html" class="active">HOME</a>
            <a href="about.html">ABOUT</a>
            <a href="menu.html">MENU</a>
        </nav>

    </header>

    <section class="hero">
        <div class="hero-content">
            <h1>Taste the Tradition</h1>
            <p>where every dish tells a story</p>
        </div>
        <div class="hero-img">
            <img src="C:\Users\admin\OneDrive\Desktop\sem 3\web\exp7\softweb\generated-image.png" alt="Hero Image">
        </div>
    </section>
</body>
</html>

menu.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Native Kitchen - Menu</title>
    <link href="https://fonts.googleapis.com/css?family=Montserrat:700,400&display=swap" rel="stylesheet">
    <style>
        body {
            margin: 0;
            font-family: 'Montserrat', Arial, sans-serif;
            background: #dfd764;
            color: #232323;
        }
        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 28px 60px;
            background: #f5f5ef;
        }
        .logo {
            display: flex;
            align-items: center;
            font-size: 2.1rem;
            font-weight: 700;
        }
        .logo-img {
            height: 50px;
            width: 50px;
            border-radius: 50%;
            object-fit: cover;
            margin-right: 16px;
            border: 2px solid #ffe8b2;
        }
        nav {
            display: flex;
            gap: 38px;
        }
        nav a {
            text-decoration: none;
            color: #232323;
            font-weight: 500;
            font-size: 1.1rem;
            position: relative;
        }
        nav a.active, nav a:hover {
            color: #658635;
        }
        main {
            max-width: 740px;
            margin: 50px auto;
            background: #f9faf2;
            padding: 36px 40px;
            border-radius: 20px;
            box-shadow: 0 4px 30px rgba(101, 134, 53, 0.06);
        }
        h1 {
            font-size: 2.4rem;
            color: #3f5429;
            text-align: center;
            margin-bottom: 36px;
            font-weight: 700;
        }
        .menu-section {
            margin-bottom: 34px;
        }
        .menu-section h2 {
            color: #658635;
            font-size: 1.5rem;
            margin-bottom: 14px;
            font-weight: 700;
        }
        .menu-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 14px 0;
            border-bottom: 1px dotted #c2c27b;
        }
        .menu-item:last-child {
            border-bottom: none;
        }
        .dish-name {
            font-size: 1.15rem;
            font-weight: 600;
        }
        .dish-price {
            font-size: 1rem;
            color: #735a01;
            font-weight: 500;
        }
        .dish-desc {
            font-size: 0.98rem;
            color: #444;
            margin-top: 2px;
        }
        @media (max-width: 900px) {
            main {
                margin: 24px 6vw;
                padding: 24px 12px;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="logo">
            <img src="C:\Users\admin\OneDrive\Desktop\sem 3\web\exp7\softweb\generated-image (4).png" alt="Native Kitchen Logo" class="logo-img">
            Native Kitchen
        </div>
        <nav>
            <a href="index.html">HOME</a>
            <a href="about.html">ABOUT</a>
            <a href="menu.html" class="active">MENU</a>
        </nav>
    </header>

    <main>
        <h1>Our Specials</h1>
        
        <section class="menu-section">
            <h2>Starters</h2>
            <div class="menu-item">
                <div>
                    <span class="dish-name">Idli Sambar</span>
                    <div class="dish-desc">Soft rice cakes served with aromatic lentil stew.</div>
                </div>
                <span class="dish-price">₹60</span>
            </div>
            <div class="menu-item">
                <div>
                    <span class="dish-name">Medu Vada</span>
                    <div class="dish-desc">Crispy lentil doughnuts paired with coconut chutney.</div>
                </div>
                <span class="dish-price">₹70</span>
            </div>
        </section>
        
        <section class="menu-section">
            <h2>Main Course</h2>
            <div class="menu-item">
                <div>
                    <span class="dish-name">Dosa</span>
                    <div class="dish-desc">Golden South Indian crepes, choice of filling.</div>
                </div>
                <span class="dish-price">₹90</span>
            </div>
            <div class="menu-item">
                <div>
                    <span class="dish-name">Bisi Bele Bath</span>
                    <div class="dish-desc">Traditional Karnataka rice-lentil dish with vegetables.</div>
                </div>
                <span class="dish-price">₹110</span>
            </div>
        </section>
        
        <section class="menu-section">
            <h2>Desserts</h2>
            <div class="menu-item">
                <div>
                    <span class="dish-name">Payasam</span>
                    <div class="dish-desc">Sweet milk pudding with vermicelli and cardamom.</div>
                </div>
                <span class="dish-price">₹60</span>
            </div>
            <div class="menu-item">
                <div>
                    <span class="dish-name">Mysore Pak</span>
                    <div class="dish-desc">Rich gram flour and ghee fudge from Mysore.</div>
                </div>
                <span class="dish-price">₹50</span>
            </div>
        </section>
    </main>
</body>
</html>

about.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Native Kitchen - About</title>
    <link href="https://fonts.googleapis.com/css?family=Montserrat:700,400&display=swap" rel="stylesheet">
    <style>
        body {
            margin: 0;
            font-family: 'Montserrat', Arial, sans-serif;
            background: #e8eed3;
            color: #232323;
        }
        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 28px 60px;
            background: #f5f5ef;
        }
        .logo {
            display: flex;
            align-items: center;
            font-size: 2.1rem;
            font-weight: 700;
        }
        .logo-img {
            height: 50px;
            width: 50px;
            border-radius: 50%;
            object-fit: cover;
            margin-right: 16px;
            border: 2px solid #ffe8b2;
        }
        nav {
            display: flex;
            gap: 38px;
        }
        nav a {
            text-decoration: none;
            color: #232323;
            font-weight: 500;
            font-size: 1.1rem;
            position: relative;
        }
        nav a.active, nav a:hover {
            color: #658635;
        }
        .hero-top {
            position: relative;
            height: 260px;
            width: 100%;
            background: linear-gradient(120deg, #708d5a 55%, #373734 100%);
            color: #fff;
            display: flex;
            align-items: flex-end;
            padding-left: 80px;
            padding-bottom: 70px;
            font-size: 2.2rem;
            font-weight: 700;
            letter-spacing: 2px;
        }
        .content-section {
            display: flex;
            align-items: flex-start;
            gap: 40px;
            background: #fbfaea;
            padding: 60px 6vw;
            border-radius: 0 0 38px 38px;
            margin-top: -30px;
            box-shadow: 0 0 50px rgba(140,155,103,0.09);
        }
        .content-img {
            flex: 1 1 320px;
            max-width: 390px;
            display: flex;
            justify-content: center;
            align-items: center;
        }
        .content-img img {
            width: 100%;
            max-width: 370px;
            height: auto;
        }
        .content-txt {
            flex: 2 1 400px;
            padding-top: 16px;
        }
        .content-txt h2 {
            font-size: 2.1rem;
            color: #545440;
            font-weight: 700;
            margin-bottom: 26px;
        }
        .content-txt p {
            font-size: 1.13rem;
            color: #232323;
            margin-bottom: 16px;
            line-height: 1.7;
        }
        @media (max-width: 920px) {
            .content-section {
                flex-direction: column;
                align-items: center;
                gap: 24px;
                padding: 20px 2vw;
            }
            .hero-top {
                padding-left: 24px;
                font-size: 1.7rem;
                padding-bottom: 32px;
                height: 140px;
            }
            .content-txt {
                padding-top: 0;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="logo">
            <img src="C:\Users\admin\OneDrive\Desktop\sem 3\web\exp7\softweb\generated-image (4).png" alt="Native Kitchen Logo" class="logo-img">
            Native Kitchen
        </div>
        <nav>
            <a href="index.html">HOME</a>
            <a href="about.html" class="active">ABOUT</a>
            <a href="menu.html">MENU</a>
        </nav>
    </header>
    <section class="hero-top">
        ABOUT
    </section>
    <section class="content-section">
        <div class="content-img">
            <!-- Use tree/ambience/food illustration here.
                 Below, use your actual image filename, e.g., image.jpg. -->
            <img src="C:\Users\admin\OneDrive\Pictures\Screenshots\Screenshot 2025-11-05 161450.png" alt="Restaurant Ambience / Tree Graphic">
        </div>
        <div class="content-txt">
            <h2>Discover Our Journey</h2>
            <p>Immerse yourself in an extraordinary fine dining experience at Native Kitchen, where high-quality culinary excellence meets Authentic South Indian Vegetarian Cuisine. Our meticulously crafted traditional dishes are served in a luxurious ambience designed to transport you back in time, evoking a sense of nostalgia and delight.</p>
            <p>Native Kitchen is the brainchild of a group of passionate individuals, united by their love for exceptional food and the desire to create a restaurant unlike any other. Join us and savor the unique blend of tradition and innovation that defines our cuisine, offering you a dining experience that is truly unparalleled.</p>
        </div>
    </section>
</body>
</html>

```

## OUTPUT:

![alt text](<Screenshot 2025-11-05 162002.png>)

![alt text](<Screenshot 2025-11-05 162015.png>)

![alt text](<Screenshot 2025-11-05 162028.png>)

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
