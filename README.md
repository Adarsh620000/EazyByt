# EazyByt
A language learning platform..
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Language Learning Platform</title>
    <link rel="stylesheet" href="css/styles.css">
</head>
<body>
    <header>
        <h1>APNI SANSKRITI</h1>
        <H2>APNA BHARAT</H2>
        <nav>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Courses</a></li>
                <li><a href="#">Dashboard</a></li>
                <li><a href="#">Profile</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="course-list">
            <h2>Available Courses</h2>
            <div class="course">
                <h3>BASICS HINDI</h3>
                <p>COURSE PRICE:-28000</p>
                <button>Enroll</button>
            </div>
            <div class="course">
                <h3>ADVANCED HINDI</h3>
                <p>COURSE PRICE:-50000</p>
                <button>Enroll</button>
            </div>
            <div class="course">
                <h3>BASICS SANSKRIT</h3>
                <p>COURSE PRICE:-75000</p>
                <button>Enroll</button>
            </div>
            <div class="course">
                <h3>ADVANCED SANSKRIT</h3>
                <p>COURSE PRICE:-100000</p>
                <button>Enroll</button>
            </div>
        </section>
    </main>

    <footer>
        <p>&copy; 2024 Language Learning Platform</p>
    </footer>

    <script src="js/scripts.js"></script>
</body>
</html>



/* General Styles */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

header {
    background-color: #4CAF50;
    color: white;
    padding: 1em;
    text-align: center;
}

nav ul {
    list-style-type: none;
    padding: 0;
    DISPLAY: inline;
}

nav ul li {
    display: inline;
    margin: 0 10px;
}

nav ul li a {
    color: white;
    text-decoration: none;
}

main {
    padding: 2em;
}

.course {
    border: 1px solid #ddd;
    margin: 1em 0;
    padding: 1em;
    border-radius: 8px;
}

button {
    background-color: #4CAF50;
    color: white;
    border: none;
    padding: 10px 20px;
    border-radius: 5px;
    cursor: pointer;
}

button:hover {
    background-color: #45a049;
}

footer {
    background-color: #f1f1f1;
    text-align: center;
    padding: 1em;
    position: fixed;
    width: 100%;
    bottom: 0;
}

/* Responsive Design */
@media (max-width: 600px) {
    nav ul li {
        display: block;
        text-align: center;
        margin: 10px 0;
    }
}



document.addEventListener("DOMContentLoaded", function() {
    const enrollButtons = document.querySelectorAll("button");

    enrollButtons.forEach(button => {
        button.addEventListener("click", function() {
            alert("Enrolled in course!");
        });
    });
});
