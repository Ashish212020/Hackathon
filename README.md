# Hackathon
->html code
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hackathon</title>
    <link rel="stylesheet" href="style.css">
    
<body>
    <div class="image-container">
        <div class="overlay-box">
            <div class="subdivision">
                <h2>Counting</h2>
                <p>Patient </p>
            </div>
            <div class="subdivision">
                <h2>Counting</h2>
                <p> Hospital</p>
            </div>
            <div class="subdivision">
                <h2>Counting</h2>
                <p>Treatment</p>
            </div>
        </div>
        <div class="navbar">
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Services</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
            <div class="search-container">
                <input type="text" class="search-input" placeholder="Search...">
                <button class="search-button">Search</button>
            </div>
        </div>
    </div>
   <div class="container">

   </div>
</body>
</html>
-> css
.image-container {
    position: relative;
    background-image: url('images/1c.jpg'); /* Replaceim 'your-image.jpg' with the actual image file path */
    background-size: cover;
    height: 400px; /* Adjust the height as needed */
    text-align: center;
    color: white;
    border-radius:10px ;
}
.overlay-box {
    background-color: rgba(0, 0, 0, 0.7); /* Semi-transparent background color for the box */
    position: absolute;
    top: 50px; /* Adjust the top position as needed */
    left: 0;
    right: 0;
    margin: 0 auto; /* Center the box horizontally */
    padding: 20px;
    max-width: 800px; /* Adjust the maximum width as needed */
    border-radius: 5px;
    display: flex; /* Use flexbox for horizontal layout */
    justify-content: space-between; /* Space items evenly within the box */
    margin-top: 180px;
}

.subdivision {
    flex: 1; /* Distribute available space equally among the subdivisions */
    text-align: center;
    margin: 0 10px; /* Add some spacing between subdivisions */
}

/* Style the navigation bar */
.navbar {
    background-color: rgba(0, 0, 0, 0.7); /* Add a semi-transparent background to make text more readable */
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px 20px;
    border-radius: 25px;
    margin-left: 40px;
    margin-right: 40px;
    margin-top: 25px;
    
}
@media (max-width: 768px) {
    .overlay-box {
        top: 10px; /* Adjust the top position for smaller screens */
        padding: 10px;
        flex-direction: column; /* Stack subdivisions vertically on smaller screens */
    }
    
    .subdivision {
        margin: 10px 0; /* Add vertical spacing between subdivisions */
    }
}

.navbar ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    overflow: hidden;
    display: flex; /* Display the navigation links as a flex container */
    
}

.navbar li {
    margin-right: 15px; /* Add some space between navigation items */
}

.navbar li:last-child {
    margin-right: 0; /* Remove margin from the last navigation item */
}

.navbar li a {
    color: white;
    text-decoration: none;
}

.navbar li a:hover {
    background-color: rgba(255, 255, 255, 0.3); /* Change the background color on hover */
    color: black;
}

/* Style the search input */
.search-container {
    display: flex;
    align-items: center;
}

.search-input {
    border: none;
    padding: 8px;
    margin-right: 10px;
    border-radius: 4px;
}

.search-button {
    background-color: #007bff;
    color: white;
    border: none;
    border-radius: 4px;
    padding: 8px 12px;
    cursor: pointer;
}
@media (max-width: 768px) {
    .navbar {
        flex-direction: column;
    }

    .navbar li {
        margin-right: 0;
        margin-bottom: 10px;
        text-align: center;
    }

    .search-container {
        flex-direction: column;
    }

    .search-input {
        margin-right: 0;
    }
}
