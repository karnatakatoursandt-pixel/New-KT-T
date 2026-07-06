<!DOCTYPE html>
<html lang="en">
<head>

<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Karnataka Tours and Travels</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css"/>

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Poppins',sans-serif;
scroll-behavior:smooth;
}

body{
background:#f5f7fb;
overflow-x:hidden;
}

/* NAVBAR */

header{
width:100%;
height:100vh;
background:
linear-gradient(rgba(0,0,0,0.65),rgba(0,0,0,0.65)),
url('https://images.unsplash.com/photo-1501785888041-af3ef285b470?q=80&w=1600&auto=format&fit=crop');
background-size:cover;
background-position:center;
position:relative;
}

.navbar{
width:100%;
padding:18px 8%;
display:flex;
justify-content:space-between;
align-items:center;
position:fixed;
top:0;
left:0;
background:rgba(0,0,0,0.45);
backdrop-filter:blur(8px);
z-index:999;
}

.logo-container{
display:flex;
align-items:center;
gap:12px;
}

.logo-container img{
width:70px;
height:70px;
object-fit:contain;
border-radius:50%;
background:white;
padding:5px;
box-shadow:0 5px 15px rgba(0,0,0,0.2);
}

.logo-text h2{
color:white;
font-size:26px;
font-weight:800;
line-height:1;
}

.logo-text span{
color:#ff9800;
font-size:18px;
font-weight:600;
}

.nav-links{
display:flex;
gap:25px;
}

.nav-links a{
text-decoration:none;
color:white;
font-weight:500;
transition:0.3s;
}

.nav-links a:hover{
color:#ff9800;
}

/* HERO */

.hero{
width:100%;
height:100vh;
display:flex;
justify-content:center;
align-items:center;
text-align:center;
padding:0 10%;
}

.hero-content h1{
font-size:72px;
font-weight:800;
color:white;
line-height:1.2;
}

.hero-content h1 span{
color:#ff9800;
}

.hero-content p{
font-size:22px;
color:#eee;
margin-top:20px;
}

.hero-buttons{
margin-top:40px;
display:flex;
justify-content:center;
gap:20px;
flex-wrap:wrap;
}

.btn{
padding:16px 35px;
border-radius:50px;
font-size:18px;
font-weight:600;
text-decoration:none;
transition:0.4s;
}

.btn-primary{
background:#ff9800;
color:white;
}

.btn-primary:hover{
background:white;
color:black;
}

.btn-outline{
border:2px solid white;
color:white;
}

.btn-outline:hover{
background:white;
color:black;
}

/* COMMON */

section{
padding:100px 8%;
}

.section-title{
text-align:center;
margin-bottom:60px;
}

.section-title h2{
font-size:48px;
color:#0b1c39;
font-weight:800;
}

.section-title p{
margin-top:10px;
color:#666;
}

/* SERVICES */

.services-grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
gap:30px;
}

.service-card{
background:white;
padding:40px 30px;
border-radius:20px;
text-align:center;
box-shadow:0 10px 30px rgba(0,0,0,0.08);
transition:0.4s;
}

.service-card:hover{
transform:translateY(-10px);
}

.service-icon{
font-size:55px;
color:#ff9800;
margin-bottom:20px;
}

.service-card h3{
font-size:24px;
margin-bottom:15px;
color:#0b1c39;
}

.service-card p{
line-height:1.8;
color:#666;
}

/* VEHICLES */

.vehicles{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
gap:30px;
}

.vehicle-card{
background:white;
border-radius:20px;
overflow:hidden;
box-shadow:0 10px 30px rgba(0,0,0,0.08);
transition:0.4s;
}

.vehicle-card:hover{
transform:translateY(-10px);
}

.vehicle-card img{
width:100%;
height:220px;
object-fit:cover;
}

.vehicle-content{
padding:25px;
}

.vehicle-content h3{
margin-bottom:10px;
color:#0b1c39;
}

.vehicle-content p{
color:#666;
}

/* REVIEWS */

.reviews{
background:#0b1c39;
}

.reviews .section-title h2,
.reviews .section-title p{
color:white;
}

.review-grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
gap:30px;
}

.review-card{
background:white;
padding:35px;
border-radius:20px;
}

.review-card .stars{
font-size:22px;
margin-bottom:20px;
}

.review-card p{
line-height:1.8;
margin-bottom:15px;
color:#555;
}

.review-card h4{
color:#0b1c39;
}

/* AREAS */

.area-grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
gap:25px;
}

.area-box{
background:#0b1c39;
color:white;
padding:25px;
border-radius:15px;
text-align:center;
font-size:20px;
font-weight:600;
transition:0.4s;
}

.area-box:hover{
background:#ff9800;
}

/* CONTACT */

.contact-container{
display:grid;
grid-template-columns:1fr 1fr;
gap:50px;
}

.contact-info{
background:#0b1c39;
padding:40px;
border-radius:20px;
color:white;
}

.contact-info h3{
font-size:34px;
margin-bottom:25px;
}

.contact-info p{
line-height:2;
margin-bottom:20px;
}

.contact-form{
background:white;
padding:40px;
border-radius:20px;
box-shadow:0 10px 30px rgba(0,0,0,0.08);
}

.contact-form form{
display:flex;
flex-direction:column;
gap:20px;
}

.contact-form input,
.contact-form textarea,
.contact-form select{
padding:18px;
border:none;
background:#f5f7fb;
border-radius:10px;
font-size:16px;
outline:none;
}

.contact-form button{
padding:18px;
border:none;
background:#ff9800;
color:white;
font-size:18px;
font-weight:600;
border-radius:10px;
cursor:pointer;
}

/* FOOTER */

footer{
background:#071225;
color:white;
text-align:center;
padding:40px 20px;
}

footer h2{
margin-bottom:15px;
}

/* WHATSAPP */

.whatsapp{
position:fixed;
right:20px;
bottom:20px;
width:65px;
height:65px;
background:#25d366;
border-radius:50%;
display:flex;
justify-content:center;
align-items:center;
color:white;
font-size:32px;
text-decoration:none;
z-index:999;
}

/* MOBILE */

@media(max-width:900px){

.hero-content h1{
font-size:42px;
}

.contact-container{
grid-template-columns:1fr;
}

.nav-links{
display:none;
}

}

</style>

</head>

<body>

<header>

<div class="navbar">

<div class="logo-container">

<img src="logo.png" alt="Karnataka Tours and Travels Logo">

<div class="logo-text">
<h2>Karnataka Tours</h2>
<span>& Travels</span>
</div>

</div>

<div class="nav-links">
<a href="#">Home</a>
<a href="#services">Services</a>
<a href="#vehicles">Vehicles</a>
<a href="#reviews">Reviews</a>
<a href="#contact">Contact</a>
</div>

</div>

<div class="hero">

<div class="hero-content">

<h1>
Explore South India With <span>Karnataka Tours & Travels</span>
</h1>

<p>
One Way Drop • Rental Package • Outstation Trips • City Local Pickup & Drop
</p>

<div class="hero-buttons">

<a href="tel:+918431312571" class="btn btn-primary">
Call Now
</a>

<a href="https://wa.me/918431312571" class="btn btn-outline">
WhatsApp Booking
</a>

</div>

</div>

</div>

</header>

<!-- SERVICES -->

<section id="services">

<div class="section-title">
<h2>Our Services</h2>
<p>Professional travel services across South India</p>
</div>

<div class="services-grid">

<div class="service-card">
<div class="service-icon">
<i class="fa-solid fa-road"></i>
</div>
<h3>One Way Drop</h3>
<p>
Affordable one way taxi service with comfortable vehicles and professional drivers.
</p>
</div>

<div class="service-card">
<div class="service-icon">
<i class="fa-solid fa-car"></i>
</div>
<h3>Rental Package</h3>
<p>
Flexible hourly and daily rental packages for family and business trips.
</p>
</div>

<div class="service-card">
<div class="service-icon">
<i class="fa-solid fa-route"></i>
</div>
<h3>Outstation Trips</h3>
<p>
Reliable outstation travel across Karnataka, Kerala, Goa and South India.
</p>
</div>

<div class="service-card">
<div class="service-icon">
<i class="fa-solid fa-city"></i>
</div>
<h3>City Local</h3>
<p>
Local city pickup and drop service available 24/7.
</p>
</div>

<div class="service-card">
<div class="service-icon">
<i class="fa-solid fa-plane"></i>
</div>
<h3>Airport Pickup & Drop</h3>
<p>
Safe airport transfer service with punctual pickup and drop.
</p>
</div>

<div class="service-card">
<div class="service-icon">
<i class="fa-solid fa-users"></i>
</div>
<h3>Family Tour Packages</h3>
<p>
Luxury family tours with experienced drivers and comfortable vehicles.
</p>
</div>

</div>

</section>

<!-- VEHICLES -->

<section id="vehicles">

<div class="section-title">
<h2>Available Vehicles</h2>
<p>Luxury and comfortable vehicles for every trip</p>
</div>

<div class="vehicles">

<div class="vehicle-card">
<img src="https://imgd.aeplcdn.com/664x374/n/cw/ec/115777/etios-exterior-right-front-three-quarter.jpeg">
<div class="vehicle-content">
<h3>Etios</h3>
<p>Comfortable sedan for city and outstation trips.</p>
</div>
</div>

<div class="vehicle-card">
<img src="https://imgd.aeplcdn.com/664x374/n/cw/ec/45691/dzire-exterior-right-front-three-quarter-3.jpeg">
<div class="vehicle-content">
<h3>Dzire</h3>
<p>Affordable and smooth travel experience.</p>
</div>
</div>

<div class="vehicle-card">
<img src="https://imgd.aeplcdn.com/664x374/n/cw/ec/115755/ertiga-exterior-right-front-three-quarter.jpeg">
<div class="vehicle-content">
<h3>Ertiga</h3>
<p>Spacious family MPV for tours and travel.</p>
</div>
</div>

<div class="vehicle-card">
<img src="https://imgd.aeplcdn.com/664x374/n/cw/ec/51435/innova-crysta-exterior-right-front-three-quarter.jpeg">
<div class="vehicle-content">
<h3>Innova Crysta</h3>
<p>Premium luxury vehicle for comfortable journeys.</p>
</div>
</div>

<div class="vehicle-card">
<img src="https://images.unsplash.com/photo-1544620347-c4fd4a3d5957?q=80&w=1200&auto=format&fit=crop">
<div class="vehicle-content">
<h3>Tempo Traveller</h3>
<p>Perfect for group and family travel packages.</p>
</div>
</div>

<div class="vehicle-card">
<img src="https://images.unsplash.com/photo-1570125909517-53cb21c89ff2?q=80&w=1200&auto=format&fit=crop">
<div class="vehicle-content">
<h3>Mini Bus / 50 Seater Bus</h3>
<p>Best for large group tours and events.</p>
</div>
</div>

</div>

</section>

<!-- REVIEWS -->

<section class="reviews" id="reviews">

<div class="section-title">
<h2>Customer Reviews</h2>
<p>Trusted by happy customers across South India</p>
</div>

<div class="review-grid">

<div class="review-card">
<div class="stars">⭐⭐⭐⭐⭐</div>
<p>
Excellent service and clean vehicle. Driver was very professional and friendly.
</p>
<h4>— Ravi Kumar</h4>
</div>

<div class="review-card">
<div class="stars">⭐⭐⭐⭐⭐</div>
<p>
Very comfortable family trip to Kerala and Coorg. Highly recommended.
</p>
<h4>— Priya Sharma</h4>
</div>

<div class="review-card">
<div class="stars">⭐⭐⭐⭐⭐</div>
<p>
Affordable pricing and excellent support throughout our journey.
</p>
<h4>— Imran Khan</h4>
</div>

</div>

</section>

<!-- SERVICE AREAS -->

<section>

<div class="section-title">
<h2>Service Areas</h2>
<p>We provide travel services across South India</p>
</div>

<div class="area-grid">

<div class="area-box">Karnataka</div>
<div class="area-box">Andhra Pradesh</div>
<div class="area-box">Telangana</div>
<div class="area-box">Tamil Nadu</div>
<div class="area-box">Kerala</div>
<div class="area-box">Puducherry</div>
<div class="area-box">Goa</div>

</div>

</section>

<!-- CONTACT -->

<section id="contact">

<div class="section-title">
<h2>Book Your Journey</h2>
<p>Contact Karnataka Tours & Travels today</p>
</div>

<div class="contact-container">

<div class="contact-info">

<h3>Karnataka Tours & Travels</h3>

<p>
📞 +91 8431312571 <br>
📞 +91 7026220040
</p>

<p>
📧 karnatakatoursandt@gmail.com
</p>

<p>
✔ One Way Drop <br>
✔ Rental Package <br>
✔ Outstation Trips <br>
✔ City Local Pickup & Drop
</p>

</div>

<div class="contact-form">

<form>

<input type="text" placeholder="Your Name" required>

<input type="tel" placeholder="Mobile Number" required>

<select>
<option>Select Vehicle</option>
<option>Etios</option>
<option>Dzire</option>
<option>Ertiga</option>
<option>Innova</option>
<option>Innova Crysta</option>
<option>Tempo Traveller</option>
<option>Mini Bus</option>
<option>50 Seater Bus</option>
</select>

<textarea rows="6" placeholder="Enter Trip Details"></textarea>

<button type="submit">
Send Enquiry
</button>

</form>

</div>

</div>

</section>

<footer>

<h2>Karnataka Tours & Travels</h2>

<p>
Safe Journey • Happy Journey
</p>

<p>
📞 +91 8431312571 | +91 7026220040
</p>

<p>
📧 karnatakatoursandt@gmail.com
</p>

</footer>

<a href="https://wa.me/918431312571" class="whatsapp">
<i class="fa-brands fa-whatsapp"></i>
</a>

</body>
</html>
