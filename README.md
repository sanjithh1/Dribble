# Project: Responsive Web Design

## Date:12/11/24

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
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Professional Bootstrap Website</title>
    <!-- Bootstrap CSS -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <!-- Custom Styles -->
    <style>
        body {
            padding-top: 70px;
        }
        .hero-section {
            background: url('wolf.jpg') no-repeat center center;
            background-size: cover;
            color: white;
            text-align: center;
            padding: 100px 20px;
        }
        .custom-card:hover {
            transform: scale(1.05);
            transition: 0.3s;
        }
    </style>
</head>
<body>
    <!-- Navbar -->
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark fixed-top">
        <div class="container-fluid">
            <a class="navbar-brand" href="#">My Website</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item"><a class="nav-link active" href="#about">About</a></li>
                    <li class="nav-item"><a class="nav-link" href="#services">Services</a></li>
                    <li class="nav-item"><a class="nav-link" href="#portfolio">Portfolio</a></li>
                    <li class="nav-item"><a class="nav-link" href="#contact">Contact</a></li>
                </ul>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="hero-section">
        <div class="container">
            <h1 class="display-4 fw-bold">Wild photography</h1>
            <p class="lead">embrace the endangered animals</p>
            <a href="#about" class="btn btn-primary btn-lg">Learn More</a>

        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-5 bg-light">
        <div class="container">
            <h2 class="text-center mb-5">About Us</h2>
            <div class="row">
                <div class="col-md-6">
                    <img src="500x300.jpg" class="img-fluid rounded" alt="About Us">
                </div>
                <div class="col-md-6">
                    <p class="lead">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin bibendum, libero at facilisis lacinia, erat arcu suscipit est, nec pulvinar erat nunc nec justo.</p>
                    <button class="btn btn-info" data-bs-toggle="tooltip" data-bs-placement="right" title="More Info">Hover for Tooltip</button>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="py-5">
        <div class="container">
            <h2 class="text-center mb-5">Our Services</h2>
            <div class="row g-4">
                <div class="col-md-4">
                    <div class="card custom-card shadow">
                        <div class="card-body">
                            <h5 class="card-title">Web Development</h5>
                            <p class="card-text">Creating responsive and modern websites tailored to your needs.</p>
                            <button class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#serviceModal">Learn More</button>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card custom-card shadow">
                        <div class="card-body">
                            <h5 class="card-title">App Development</h5>
                            <p class="card-text">Innovative mobile apps for iOS and Android platforms.</p>
                            <button class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#serviceModal">Learn More</button>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card custom-card shadow">
                        <div class="card-body">
                            <h5 class="card-title">Digital Marketing</h5>
                            <p class="card-text">Maximize your online presence with our marketing strategies.</p>
                            <button class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#serviceModal">Learn More</button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Modal -->
    <div class="modal fade" id="serviceModal" tabindex="-1" aria-labelledby="serviceModalLabel" aria-hidden="true">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title" id="serviceModalLabel">Service Details</h5>
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                    Here are more details about this service.
                </div>
                <div class="modal-footer">
                    <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
                    <button type="button" class="btn btn-primary">Save changes</button>
                </div>
            </div>
        </div>
    </div>

    <!-- Accordion -->
    <section id="faq" class="py-5 bg-light">
        <div class="container">
            <h2 class="text-center mb-5">FAQs</h2>
            <div class="accordion" id="faqAccordion">
                <div class="accordion-item">
                    <h2 class="accordion-header" id="headingOne">
                        <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
                            What services do you offer?
                        </button>
                    </h2>
                    <div id="collapseOne" class="accordion-collapse collapse show" aria-labelledby="headingOne" data-bs-parent="#faqAccordion">
                        <div class="accordion-body">
                            We offer web development, app development, and digital marketing services.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header" id="headingTwo">
                        <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
                            How can I contact you?
                        </button>
                    </h2>
                    <div id="collapseTwo" class="accordion-collapse collapse" aria-labelledby="headingTwo" data-bs-parent="#faqAccordion">
                        <div class="accordion-body">
                            You can contact us via email, phone, or the contact form below.
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-dark text-white text-center py-3">
        <div class="container">
            <p>© 2024 My Website. All rights reserved.</p>
        </div>
    </footer>

    <!-- Bootstrap JS -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

```
## OUTPUT:
![Screenshot 2024-11-19 092042](https://github.com/user-attachments/assets/9f4cef62-1d32-4b01-833b-6636b2d3837d)
![Screenshot 2024-11-19 092050](https://github.com/user-attachments/assets/b8551a09-7cda-4cd6-8c85-039d6bd8b21c)

## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
