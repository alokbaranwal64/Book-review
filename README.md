# Book-review
#This code is dedicated to website which provide to you Book review.

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Book Review</title>
<style>
    body {
        margin: 0;
        font-family: Arial, sans-serif;
        background-color: #000;
        color: white;
        animation: fadeIn 1.5s ease-in-out;
    }
    @keyframes fadeIn {
        from { opacity: 0; }
        to { opacity: 1; }
    }
    header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 15px 30px;
        background-color: #111;
        position: sticky;
        top: 0;
        z-index: 1000;
    }
    nav a {
        color: white;
        margin: 0 15px;
        text-decoration: none;
        transition: color 0.3s;
    }
    nav a:hover {
        color: #ff9800;
    }
    .clock {
        font-size: 1rem;
        color: #ff9800;
    }
    main {
        padding: 30px;
    }
    .book-feature {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
        gap: 20px;
    }
    .book-card {
        background: #111;
        padding: 20px;
        border-radius: 8px;
        box-shadow: 0 0 10px rgba(255,255,255,0.1);
        transition: transform 0.3s ease;
    }
    .book-card:hover {
        transform: scale(1.05);
    }
    footer {
        text-align: center;
        padding: 20px;
        background-color: #111;
        margin-top: 20px;
    }
    .social-links a {
        margin: 0 10px;
        color: #ff9800;
        text-decoration: none;
    }
</style>
</head>
<body>
<header>
 
</header>

<main>
    <h1>Featured Book Reviews</h1>
    <div class="book-feature">
        <div class="book-card">
            <h3>Book Title 1</h3>
            <p>A short review about the book. Lorem ipsum dolor sit amet...</p>
        </div>
        <div class="book-card">
            <h3>Book Title 2</h3>
            <p>Another review. Lorem ipsum dolor sit amet...</p>
        </div>
        <div class="book-card">
            <h3>Book Title 3</h3>
            <p>Interesting book review here...</p>
        </div>
    </div>
</main>

<footer>
    <div class="social-links">
        <a href="#">Facebook</a>
        <a href="#">Twitter</a>
        <a href="#">Instagram</a>
    </div>
    <p>&copy; 2025 Book Review</p>
</footer>

<script>
    function updateClock() {
        const now = new Date();
        const hours = String(now.getHours()).padStart(2, '0');
        const minutes = String(now.getMinutes()).padStart(2, '0');
        const seconds = String(now.getSeconds()).padStart(2, '0');
        document.getElementById('clock').textContent = `${hours}:${minutes}:${seconds}`;
    }
    setInterval(updateClock, 1000);
    updateClock();
</script>
</body>
</html>
