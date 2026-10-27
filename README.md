<!DOCTYPE html>
<html lang="tl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Glamsanity Haven Private Villa - Book Now</title>
<style>
{margin:0;padding:0;box-sizing:border-box;font-family:Arial,sans-serif}
body{background:#f8f8f8;color:#222}
header{position:fixed;top:0;width:100%;background:#fff;padding:15px 30px;display:flex;justify-content:space-between;align-items:center;box-shadow:0 2px 10px rgba(0,0,0,.1);z-index:1000}
.logo{font-weight:bold;font-size:18px}
nav a{margin-left:20px;text-decoration:none;color:#222;font-weight:600}
.hero{height:85vh;background:url('https://images.unsplash.com/photo-1571896349842-33c89424de2d') center/cover;display:flex;align-items:center;justify-content:center;text-align:center;color:#fff;padding-top:60px}
.hero-overlay{background:rgba(0,0,0,.45);width:100%;height:100%;display:flex;flex-direction:column;align-items:center;justify-content:center;padding:20px}
.hero h1{font-size:42px;margin-bottom:10px}
.hero p{font-size:18px;margin-bottom:20px}
.btn{background:#0a7a4c;color:#fff;padding:12px 28px;border-radius:30px;text-decoration:none;font-weight:bold;display:inline-block;border:none;cursor:pointer}
section{padding:60px 20px;max-width:1100px;margin:auto}
.grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(250px,1fr));gap:20px;margin-top:20px}
.card{background:#fff;border-radius:15px;overflow:hidden;box-shadow:0 3px 15px rgba(0,0,0,.08)}
.card img{width:100%;height:180px;object-fit:cover}
.card div{padding:15px}
.price{color:#0a7a4c;font-weight:bold;margin-top:5px}
.form-box{background:#fff;padding:30px;border-radius:15px;box-shadow:0 3px 20px rgba(0,0,0,.1)}
.form-box input,.form-box select,.form-box textarea{width:100%;padding:12px;margin:8px 0 15px;border:1px solid #ddd;border-radius:8px}
.form-box label{font-weight:bold;font-size:14px}
footer{background:#111;color:#aaa;text-align:center;padding:30px;margin-top:40px}
</style>
</head>
<body>

<header> 
  <div class="logo">GLAMSANITY HAVEN</div>
  <nav>
    <a href="#rooms">Rooms</a>
    <a href="#amenities">Amenities</a>
    <a href="#book">Book Now</a>
  </nav>
</header>

<div class="hero">
  <div class="hero-overlay">
    <h1>Your Private Escape in Pampanga</h1>
    <p>Exclusive Villa • Private Pool • Up to 20 pax</p>
    <a href="#book" class="btn">Check Availability</a>
  </div>
</div>

<section id="rooms">
  <h2>Rooms & Rates</h2>
  <div class="grid">
    <div class="card">
      <img src="REPLACE-ROOM1.jpg">
      <div>
        <h3>Master Bedroom</h3>
        <p>Good for 4 • With AC & Bathroom</p>
        <p class="price">Included</p>
      </div>
    </div>
    <div class="card">
      <img src="REPLACE-ROOM2.jpg">
      <div>
        <h3>Family Room</h3>
        <p>Good for 6 • Bunk beds</p>
        <p class="price">Included</p>
      </div>
    </div>
  </div>
</section>

<section id="amenities">
  <h2>Amenities</h2>
  <div class="grid">
    <div class="card"><div> Private Pool</div></div>
    <div class="card"><div> Videoke</div></div>
    <div class="card"><div> Griller + Kitchen</div></div>
    <div class="card"><div>️ Parking for 4 cars</div></div>
  </div>
</section>

<section id="book">
  <h2>Reserve Your Date</h2>
  <div class="form-box">
    <label>Check-in Date</label>
    <input type="date" id="checkin">
    <label>Check-out Date</label>
    <input type="date" id="checkout">
    <label>Guests</label>
    <select id="guests">
      <option>1-5 pax</option>
      <option>6-10 pax</option>
      <option>11-20 pax</option>
      <option>21+ pax</option>
    </select>
    <label>Name</label>
    <input type="text" id="name" placeholder="Juan Dela Cruz">
    <label>Facebook / Phone</label>
    <input type="text" id="contact" placeholder="09xx xxx xxxx">
    <label>Message</label>
    <textarea id="msg" placeholder=""></textarea>
    <button class="btn" style="width:100%" onclick="sendBooking()">Send Reservation via Messenger</button>
    <p style="font-size:12px;text-align:center;margin-top:10px;color:#888">No payment yet - we will confirm if date is available</p>
  </div>
</section>

<footer>© 2026 Glamsanity Haven Private Villa | Pampanga</footer>

<script>
function sendBooking(){
  const checkin = document.getElementById('checkin').value;
  const checkout = document.getElementById('checkout').value;
  const guests = document.getElementById('guests').value;
  const name = document.getElementById('name').value;
  const contact = document.getElementById('contact').value;
  const msg = document.getElementById('msg').value;

  if(!checkin || !checkout || !name || !contact){ alert(); return; }

  const text = :%0A%0A📅 Check-in: ${checkin}%0A📅 Check-out: ${checkout}%0A👥 Guests: ${guests}%0A👤 Name: ${name}%0A📱 Contact: ${contact}%0A💬 Message: ${msg};
  
 
  const fbPage = "https://m.me/YOURFBPAGE";
  const waNumber = "639XXXXXXXXX"; 

  /
  window.open(https://wa.me/${waNumber}?text=${text}, '_blank');
}
</script>

</body>
</html>
