# Project Responsive Web Design using Bootstrap
## Date:

## AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.


## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

### Step 5:
Create a HTML file and include the needed Bootstrap components.

### Step 6:
Publish the website in the LocalHost.

## PROGRAM :
'''
index.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
    <title>Dribbble Clone</title>

    <!-- Google Font for Pacifico -->
    <link href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap" rel="stylesheet"/>

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css"/>

    <!-- Custom CSS -->
    <link rel="stylesheet" href="styles.css"/>

    <!-- Meta Description -->
    <meta name="description" content="Dribbble-inspired gallery showcasing design and fashion products."/>
</head>
<body>
    <!-- Navigation Bar -->
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
        <a class="navbar-brand" href="#">Dribbble</a>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav"
            aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav ml-auto">
                <li class="nav-item"><a class="nav-link" href="#">Look Up</a></li>
                <li class="nav-item"><a class="nav-link" href="#">Designers</a></li>
                <li class="nav-item"><a class="nav-link" href="#">Teams</a></li>
                <li class="nav-item"><a class="nav-link" href="#">Hub</a></li>
                <li class="nav-item"><a class="nav-link" href="#">Hiring</a></li>
                <li class="nav-item"><a class="btn btn-primary" href="#">Sign Up</a></li>
            </ul>
        </div>
    </nav>

    <!-- Header Section -->
    <div class="container mt-4">
        <div class="text-center mb-4 header-section">
            <h3>Your Next Favorite Look Awaits.</h3>
            <p class="lead">Curated styles and exclusive picks from top brands.</p>
        </div>

        <!-- Gallery Section -->
        <div class="row gallery-section">
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="images/jeans.jpg" class="card-img-top gallery-img" alt="Levis Denim"/>
                    <div class="card-body text-center">
                        <p class="card-title">DENIM</p>
                        <small class="text-muted">Calvin Klein</small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="images/sketchers.jpg" class="card-img-top gallery-img" alt="Puma Sneakers"/>
                    <div class="card-body text-center">
                        <p class="card-title">SNEAKERS</p>
                        <small class="text-muted">Sketchers</small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="images/mochi.webp" class="card-img-top gallery-img" alt="Woodland Shoes"/>
                    <div class="card-body text-center">
                        <p class="card-title">SHOES</p>
                        <small class="text-muted">Mochi</small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="images/versace.jpg" class="card-img-top gallery-img" alt="Zara Heels"/>
                    <div class="card-body text-center">
                        <p class="card-title">HEELS</p>
                        <small class="text-muted">Versace</small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="images/armani.jpg" class="card-img-top gallery-img" alt="Swatch Watch"/>
                    <div class="card-body text-center">
                        <p class="card-title">WATCH</p>
                        <small class="text-muted">Armani Exchange</small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="images/nike.jpg" class="card-img-top gallery-img" alt="Nike Sneakers"/>
                    <div class="card-body text-center">
                        <p class="card-title">SNEAKERS</p>
                        <small class="text-muted">NIKE</small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="images/saint.jpg" class="card-img-top gallery-img" alt="Macys Heels"/>
                    <div class="card-body text-center">
                        <p class="card-title">HEELS</p>
                        <small class="text-muted">Saint Laurent</small>
                    </div>
                </div>
            </div>
            <div class="col-md-3 col-sm-6 mb-4">
                <div class="card shadow gallery-item">
                    <img src="images/burberry.jpg" class="card-img-top gallery-img" alt="Perfume Bottle"/>
                    <div class="card-body text-center">
                        <p class="card-title">PERFUMES</p>
                        <small class="text-muted">Burberry</small>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Footer -->
    <footer class="bg-dark text-white text-center py-3">
        <p>© Dribbble. All rights reserved.</p>
    </footer>

    <!-- Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.5.1.min.js"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.bundle.min.js"></script>
</body>
</html>


styles.css

body {
    font-family: 'Pacifico', cursive;
    margin: 0;
    padding: 0;
    background-color: #bcd4d4;
    color: #2c3e50;
}

.navbar {
    background-color: #00695c;
    box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.1);
}

.navbar-brand, .navbar-nav .nav-link {
    color: #ffffff !important;
}

.navbar-nav {
    flex-direction: row;
}

.navbar-nav .nav-link {
    padding: 0 15px;
}

.nav-item .btn-primary {
    background-color: #ff7043;
    border-color: #ff7043;
}

.nav-item .btn-primary:hover {
    background-color: #d84315;
    border-color: #d84315;
}

.header-section h3 {
    font-weight: bold;
    color: #00695c;
}

.header-section p {
    font-size: 1.2em;
    color: #37474f;
}

.gallery-container {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
    gap: 20px;
    padding: 20px;
}

.card {
    background-color: #ffffff;
    border: 1px solid #cfd8dc;
    border-radius: 10px;
    box-shadow: 0px 6px 12px rgba(0, 0, 0, 0.08);
    overflow: hidden;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 0;
    margin-bottom: 20px;
    max-width: 100%;
}

.card:hover {
    transform: translateY(-5px);
    box-shadow: 0px 10px 20px rgba(0, 0, 0, 0.15);
}

.gallery-img {
    width: 100%;
    height: 180px;
    object-fit: cover;
    display: block;
    border-radius: 10px 10px 0 0;
    margin: 0;
}

.card:hover .gallery-img {
    transform: scale(1.05);
    box-shadow: 0px 8px 15px rgba(0, 0, 0, 0.25);
}

.card-title {
    font-weight: bold;
    font-size: 1.1rem;
    color: #00695c;
    text-align: center;
    margin-top: 15px;
}

.card-body {
    padding: 20px;
    text-align: center;
    flex-grow: 1;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

footer {
    background-color: #00695c;
    color: #ffffff;
    text-align: center;
    padding: 25px;
    font-size: 0.9em;
    margin-top: 40px;
    box-shadow: 0px -2px 5px rgba(0, 0, 0, 0.1);
}

/* Responsive Design */
@media (max-width: 768px) {
    .navbar-nav {
        flex-direction: column;
        text-align: center;
        padding: 10px 0;
    }

    .gallery-section {
        margin-top: 20px;
    }

    .card-body {
        padding: 10px;
    }
}

@media (max-width: 480px) {
    .header-section h3 {
        font-size: 1.5em;
    }

    .header-section p {
        font-size: 1em;
    }
}

'''

## OUTPUT:
![alt text](<Screenshot 2025-05-29 085904.png>)
![alt text](<Screenshot 2025-05-29 085918.png>)

## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
