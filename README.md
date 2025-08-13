# Ex02 Commercial Website
## Date:13.8.2025

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
```
       <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Online Website</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: plum;
        }
        header {
            background-color: #333;
            color:pink;
            padding: 20px;
            text-align: center;
        }
        nav {
            display: flex;
            justify-content: center;
            background-color: #444;
            padding: 10px;
        }
        nav a {
            color:pink;
            text-decoration: none;
            margin: 0 15px;
            padding: 10px 15px;
        }
        nav a:hover {
            background-color: #555;
            border-radius: 5px;
        }
        .hero {
            display: flex;
            align-items: center;
            justify-content: center;
            background: url('realestate-hero.jpg') no-repeat center center/cover;
            height: 400px;
            color: pink;
            text-align: center;
        }
        .hero h1 {
            font-size: 3rem;
            background: rgba(0, 0, 0, 0.5);
            padding: 20px;
        }
        .properties {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            padding: 20px;
            gap: 20px;
        }
        .property {
            border: 1px solid #ddd;
            border-radius: 5px;
            overflow: hidden;
            width: 300px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }
        .property img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }
        .property-details {
            padding: 15px;
        }
        .property-details h3 {
            margin: 0 0 10px;
        }
        .property-details p {
            margin: 0 0 15px;
            color: #555;
        }
        .property-details a {
            text-decoration: none;
            color:brown;
            background-color: peachpuff;
            padding: 10px 15px;
            border-radius: 5px;
        }
        .property-details a:hover {
            background-color: #0056b3;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 20px;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <header>
        <h1>My Commercial Website</h1>
    </header>
    <nav>
        <a href="#home">Home</a>
        <a href="#properties">Properties</a>
        <a href="#about">About Us</a>
        <a href="#contact">Contact</a>
    </nav>
    <section id="home" class="home">
        <div style="text-align: center; padding: 50px;">
            <h2>Empowering Your Business with Smart Solutions </h2>
            <p>We deliver innovative products and services that help you grow, thrive, and stay ahead of the competition.</p>
            <a href="#properties" style="text-decoration: none; color: white; background-color: #007BFF; padding: 10px 20px; border-radius: 5px;">Browse Properties</a>
        </div>
    </section>
    <section class="hero">
        <h1>Explore Your Choice</h1>
    </section>
    <section id="properties" class="properties">
        <div class="property">
            <img src="C:\Users\admin\Downloads\image 1.webp" >
            <div class="property-details">
                <h3>Branded cloths </h3>
                <p>RS 8,200</p>
                <a href="#">View Details</a>
            </div>
        </div>
        <div class="property">
            <img src="C:\Users\admin\Downloads\image 2.webp" >
            <div class="property-details">
                <h3>Modern Shoes</h3>
                <p>RS 2000</p>
                <a href="#">View Details</a>
            </div>
        </div>
        <div class="property">
            <img src="C:\Users\admin\Downloads\image 3.webp">
            <div class="property-details">
                <h3>Smart Watches</h3>
                <p>RS 4500</p>
                <a href="#">View Details</a>
            </div>
        </div>
    </section>
    <section id="about" class="about" style="background-color: #f9f9f9; padding: 50px;">
        <div style="max-width: 800px; margin: auto; text-align: center;">
            <h2>About Us</h2>
            <p>At My Commercial Website, we specialize in providing high-quality [products/services] tailored to meet the unique needs of businesses and individuals. With a commitment to excellence and a passion for innovation, we help our clients achieve their goals through reliable, scalable, and cost-effective solutions.</p>
            
        </div>
    </section>
    <section id="contact" class="contact" style="padding: 50px;">
        <div style="max-width: 600px; margin: auto; text-align: center;">
            <h2>Contact Us</h2>
            <p>Have questions or need assistance? We're here to help!</p>
            <p>Email: <a href="mailto:info@dreamhomes.com">mywebsite@gmail.com</a></p>
            <p>Phone: <a href="tel:+1234567890">+91 2356789100</a></p>
            <p>Address: 123 Innovation Street,Sector 45, Tech Park, chennai</p>
            <form style="margin-top: 20px;">
                <input type="text" placeholder="Your Name" style="width: 100%; padding: 10px; margin-bottom: 10px; border: 1px solid #ddd; border-radius: 5px;">
                <input type="email" placeholder="Your Email" style="width: 100%; padding: 10px; margin-bottom: 10px; border: 1px solid #ddd; border-radius: 5px;">
                <textarea placeholder="Your Message" style="width: 100%; padding: 10px; margin-bottom: 10px; border: 1px solid #ddd; border-radius: 5px;"></textarea>
                <button type="submit" style="background-color: #007BFF; color: white; padding: 10px 20px; border: none; border-radius: 5px;">Send Message</button>
            </form>
        </div>
    </section>
    <footer>
        <p>&copy; 2023 Dream Homes Real Estate. All rights reserved.</p>
    </footer>
</body>
</html>
```

## OUTPUT
![image](https://github.com/user-attachments/assets/1ddc3628-7512-40ad-a6d3-98f2c6802b23)
![Screenshot 2025-05-20 140616](https://github.com/user-attachments/assets/1211f6ae-db7c-4887-86f7-282a7f4b825b)
![Screenshot 2025-05-20 141008](https://github.com/user-attachments/assets/13b3b5b6-2706-4f23-9c7c-ebcedcf105e1)


## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
