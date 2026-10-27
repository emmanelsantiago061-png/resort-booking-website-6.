<!DOCTYPE html>
<html lang="en">
<head>
    <title>Resort Booking</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header>
        <h1>Paradise Resort</h1>
        <nav>
            <a href="index.html">Home</a>
            <a href="#rooms">Rooms</a>
            <a href="#booking">Book Now</a>
        </nav>
    </header>

    <section>
        <h2>Welcome to Paradise Resort</h2>
        <p>Book your perfect vacation today!</p>
        <button onclick="location.href='#booking'">
            Book Now
        </button>
    </section>

    <section id="rooms">
        <h2>Our Rooms</h2>
        <p>Standard Room - ₱2,500</p>
        <p>Deluxe Room - ₱4,000</p>
        <p>Family Room - ₱6,000</p>
    </section>

    <section id="booking">
        <h2>Reservation</h2>
        <form>
            <input type="text" placeholder="Full Name" required>
            <input type="email" placeholder="Email" required>
            <input type="date" required>
            <button type="submit">Submit Booking</button>
        </form>
    </section>

</body>
</html>
