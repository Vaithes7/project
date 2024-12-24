# Project Responsive Web Design using Bootstrap
# Date: 7.12.2024
# AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.

# DESIGN STEPS:
## Step 1:
Clone the repository from GitHub.

## Step 2:
Create Django Admin project.

## Step 3:
Create a New App under the Django Admin project.

## Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

## Step 5:
Create a HTML file and include the needed Bootstrap components.

## Step 6:
Publish the website in the LocalHost.

# PROGRAM :

Home
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>InspireSphere</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        body {
            background-color: #ffffff;
            font-family: 'Arial', sans-serif;
        }
        .navbar-brand {
            font-weight: bold;
            color: #35e1ff !important;
        }
        .custom-btn {
            background-color:#35e1ff;
            color: white;
        }
        .custom-btn:hover {
            background-color: #050302;
        }
        .project-card img {
            border-radius: 15px;
        }
        .card-title {
            font-size: 1.3rem;
            font-weight: 700;
        }
        footer {
            background-color: black ;
            color: #ffffff;
        }
    </style>
</head>
<body>
    <nav class="navbar navbar-expand-lg navbar-light bg-white shadow-sm">
        <div class="container">
            <a class="navbar-brand" href="#">InspireSphere</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item">
                        <a class="nav-link" href="#">Explore</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Opportunities</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link btn custom-btn btn-sm text-white ms-2" href="sign.html">Sign In</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link btn custom-btn btn-sm text-white ms-2" href="login.html">Login</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
    <div class="container mt-5">
        <div class="text-center">
            <h1 class="mb-4">Unleash Creativity Across the Globe</h1>
            <p class="lead text-muted">Discover exceptional designs, showcase your talents, and connect with a community of visionaries.</p>
            <a href="#" class="btn custom-btn btn-lg">Start Exploring</a>
        </div>
    </div>

    <div class="container my-5">
        <h2 class="text-center mb-4">Featured Inspirations</h2>
        <div class="row">
            <div class="col-md-4 mb-4">
                <div class="card project-card shadow-sm">
                    <img src="c:\Users\admin\Downloads\App...png" class="card-img-top" alt="Project 1">
                    <div class="card-body">
                        <h5 class="card-title">Innovative App Design</h5>
                        <p class="card-text text-muted">A groundbreaking concept redefining user experiences.</p>
                    </div>
                </div>
            </div>
            <div class="col-md-4 mb-4">
                <div class="card project-card shadow-sm">
                    <img src="c:\Users\admin\Downloads\CR.avif" class="card-img-top" alt="Project 2">
                    <div class="card-body">
                        <h5 class="card-title">Artistic Illustration</h5>
                        <p class="card-text text-muted">A vivid illustration that tells a captivating story.</p>
                    </div>
                </div>
            </div>
            <div class="col-md-4 mb-4">
                <div class="card project-card shadow-sm">
                    <img src="c:\Users\admin\Downloads\display-logos-brand-called-brand-brand_1191871-97720.jpg" class="card-img-top" alt="Project 3">
                    <div class="card-body">
                        <h5 class="card-title">Futuristic Branding</h5>
                        <p class="card-text text-muted">A branding concept ahead of its time.</p>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <div class="container my-5 text-center">
        <h2 class="mb-4">Ready to Showcase Your Work?</h2>
        <p class="lead text-muted">Join a thriving community of creators and let the world see your brilliance.</p>
        <a href="#" class="btn custom-btn btn-lg">Join InspireSphere</a>
    </div>

    <footer class="py-4">
        <div class="container text-center">
            <p class="mb-0">&copy; 2024 InspireSphere. Empowering Creativity Everywhere.</p>
        </div>
    </footer>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```

Login Page

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login - InspireSphere</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        body {
            background-color:#59f4ff;
            font-family: 'Arial', sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        .login-container {
            max-width: 400px;
            padding: 2rem;
            background: white;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        .custom-btn {
            background-color: #59f4ff;
            color: white;
        }
        .custom-btn:hover {
            background-color: #ffffff;
        }
    </style>
</head>
<body>
    <div class="login-container">
        <h2 class="text-center mb-4">Login to InspireSphere</h2>
        <form>
            <div class="mb-3">
                <label for="email" class="form-label">Email address</label>
                <input type="email" class="form-control" id="email" placeholder="Enter your email">
            </div>
            <div class="mb-3">
                <label for="password" class="form-label">Password</label>
                <input type="password" class="form-control" id="password" placeholder="Enter your password">
            </div>
            <div class="mb-3 form-check">
                <input type="checkbox" class="form-check-input" id="rememberMe">
                <label class="form-check-label" for="rememberMe">Remember me</label>
            </div>
            <button type="submit" class="btn custom-btn w-100">Login</button>
        </form>
        <p class="text-center mt-3">
            <a href="#">Forgot Password?</a>
        </p>
        <p class="text-center">
            Don't have an account? <a href="sign.html">Sign up</a>
        </p>
    </div>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```
Sign In Page

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sign Up - InspireSphere</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        body {
            background-color: #59f4ff;
            font-family: 'Arial', sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        .signup-container {
            max-width: 400px;
            padding: 2rem;
            background: white;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        .custom-btn {
            background-color: #6be6ff;
            color: white;
        }
        .custom-btn:hover {
            background-color: #ffffff;
        }
    </style>
</head>
<body>
    <div class="signup-container">
        <h2 class="text-center mb-4">Sign Up for InspireSphere</h2>
        <form>
            <div class="mb-3">
                <label for="fullName" class="form-label">Full Name</label>
                <input type="text" class="form-control" id="fullName" placeholder="Enter your full name">
            </div>
            <div class="mb-3">
                <label for="email" class="form-label">Email address</label>
                <input type="email" class="form-control" id="email" placeholder="Enter your email">
            </div>
            <div class="mb-3">
                <label for="password" class="form-label">Password</label>
                <input type="password" class="form-control" id="password" placeholder="Create a password">
            </div>
            <div class="mb-3">
                <label for="confirmPassword" class="form-label">Confirm Password</label>
                <input type="password" class="form-control" id="confirmPassword" placeholder="Confirm your password">
            </div>
            <button type="submit" class="btn custom-btn w-100">Sign Up</button>
        </form>
        <p class="text-center mt-3">
            Already have an account? <a href="login.html">Login</a>
        </p>
    </div>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```


# OUTPUT:

Home 
![screencapture-file-C-Users-admin-Desktop-HTML-dibble-html-2024-12-24-23_53_03](https://github.com/user-attachments/assets/5131ad24-8e93-4be1-9780-05deecb7fae9)

Login Page

![Screenshot 2024-12-24 235356](https://github.com/user-attachments/assets/c1f04ac6-6d79-4840-a645-5afe647cc49c)

Sign In Page


![Screenshot 2024-12-24 235335](https://github.com/user-attachments/assets/a5312fbf-8f6e-4fff-a16f-1d95f9d3da86)



# RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
