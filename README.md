<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
        <title>School Website</title>
        <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
        <style>
            body, html {
                height: 100%;
                margin: 0;
                padding: 0;
                font-family: Arial, sans-serif;
                background: linear-gradient(to right, #1e3c72, #2a5298);
                background-attachment: fixed;
                background-size: cover;
                color: white;
                overflow-x: hidden;
                overflow-y: auto;
            }
            ::-webkit-scrollbar {
                width: 10px;
            }
            ::-webkit-scrollbar-track {
                background: #1e3c72;
            }
            ::-webkit-scrollbar-thumb {
                background: #2a5298;
                border-radius: 5px;
            }
    
            header {
                background: linear-gradient(to right, #0066cc, #99ccff);
                color: white;
                padding: 15px;
                text-align: center;
                font-size: 24px;
                width: 100%;
            }
            .navbar {
                border: 4px solid grey;
                border-radius: 15px;
                padding: 10px;
            }
            .navbar-brand, .nav-link {
                color: black !important;
            }
            .navbar-nav .nav-link {
                background-color: grey;
                color: black;
                border-radius: 30px;
                padding: 10px 20px;
                margin: 5px;
                transition: background-color 0.3s, transform 0.2s;
            }
    
            .navbar-nav .nav-link:hover {
                background-color: #666666;
                transform: scale(1.1);
            }
    
            .main-content {
                flex-grow: 1;
                display: flex;
                justify-content: center;
                align-items: center;
                width: 100%;
                padding: 20px;
            }
    
            .container, .form-container {
                background: linear-gradient(to top, #f1f1f1, #ffffff);
                width: 100%;
                max-width: 1200px;
                box-shadow: 0px 0px 10px gray;
                border-radius: 5px;
                padding: 20px;
                text-align: center;
            }
    
            footer {
    background-color: #0066cc;
    color: white;
    padding: 20px;
    text-align: center;
    width: 100vw; /* Full viewport width */
    position: relative; /* Ensures it stays within normal flow */
    left: 0;
}

footer .container {
    max-width: 1200px; /* Limits content width */
    margin: 0 auto; /* Centers the content inside the footer */
}

    
            table {
                width: 100%;
                border-collapse: collapse;
                margin-top: 20px;
            }
    
            table, th, td {
                border: 1px solid black;
            }
    
            th, td {
                padding: 10px;
                text-align: center;
            }
    
            h1 {
                background-color: cadetblue;
                text-align: center;
                margin: 0;
                padding: 20px;
                width: 100%;
            }
    
            .gallery-container {
                overflow-x: auto;
                white-space: nowrap;
                padding: 20px;
                background-color: #f8f9fa;
            }
    
            .gallery-container img {
                width: 200px;
                height: 150px;
                margin-right: 10px;
                border-radius: 10px;
                object-fit: cover;
            }
    
            .card {
                transition: all 0.3s ease-in-out;
            }
    
            .card:hover {
                transform: scale(1.02);
                box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.2);
            }
    
            .fade-toggle {
                display: none;
            }
    
            /* Custom scrollbar styling */
            .gallery-container::-webkit-scrollbar {
                height: 8px;
            }
    
            .gallery-container::-webkit-scrollbar-track {
                background: #333;
            }
    
            .gallery-container::-webkit-scrollbar-thumb {
                background: #0066cc;
                border-radius: 5px;
            }
    
            .gallery-container::-webkit-scrollbar-thumb:hover {
                background: #0066cc;
            }
    
            ::placeholder {
                color: #6c757d;
                opacity: 1;
            }
    
            .form-control {
                background-color: #f8f9fa;
                border: 1px solid #ced4da;
            }
    
            /* Media Queries for Responsiveness */
            @media (max-width: 768px) {
                header {
                    font-size: 18px;
                    padding: 10px;
                }
    
                .navbar-nav .nav-link {
                    padding: 8px 15px;
                }
    
                .main-content {
                    padding: 10px;
                }
    
                .container, .form-container {
                    width: 100%;
                    padding: 15px;
                }
    
                footer {
                    padding: 10px;
                }
    
                table, th, td {
                    font-size: 12px;
                }
            }
    
            @media (max-width: 576px) {
                header {
                    font-size: 16px;
                }
    
                .navbar-nav .nav-link {
                    font-size: 12px;
                    padding: 5px 10px;
                }
    
                .gallery-container img {
                    width: 150px;
                    height: 120px;
                }
    
                .main-content {
                    flex-direction: column;
                    align-items: flex-start;
                }
            }
            @keyframes blink {
        50% { opacity: 0; }
    }

    .blink {
        animation: blink 1s infinite;
        font-weight: bold;
    }

    .present {
        color: green;
    }

    .absent {
        color: red;
    }
    
        </style>
    </head>
    
<body class="container py-5">
    <header>
        KIPINI HIGH SCHOOL
    </header>
    
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
        <div class="container">
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav">
                    <!-- Departments Dropdown -->
                    <li class="nav-item dropdown">
                        <a class="nav-link dropdown-toggle" href="#" id="departmentsDropdown" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                            Departments
                        </a>
                        <ul class="dropdown-menu" aria-labelledby="departmentsDropdown">
                            <li><a class="dropdown-item" href="#">Science</a></li>
                            <li><a class="dropdown-item" href="#">Mathematics</a></li>
                            <li><a class="dropdown-item" href="#">Humanities</a></li>
                            <li><a class="dropdown-item" href="#">Languages</a></li>
                            <li><a class="dropdown-item" href="#">Games</a></li>
                            <li><a class="dropdown-item" href="#">Guidance & Counselling</a></li>
                            <li><a class="dropdown-item" href="#">Technicals</a></li>
                        </ul>
                    </li>
                    <!-- Events Dropdown -->
                    <li class="nav-item dropdown">
                        <a class="nav-link dropdown-toggle" href="#" id="eventsDropdown" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                            Events
                        </a>
                        <ul class="dropdown-menu" aria-labelledby="eventsDropdown">
                            <li><a class="dropdown-item" href="#">Opening</a></li>
                            <li><a class="dropdown-item" href="#">Form 4 Clinic</a></li>
                            <li><a class="dropdown-item" href="#">Form 3 Clinic</a></li>
                            <li><a class="dropdown-item" href="#">Form 2 Clinic</a></li>
                            <li><a class="dropdown-item" href="#">Kipini Open Tournament</a></li>
                            <li><a class="dropdown-item" href="#">CAT 1</a></li>
                            <li><a class="dropdown-item" href="#">CAT 2</a></li>
                            <li><a class="dropdown-item" href="#">Half-Term</a></li>
                            <li><a class="dropdown-item" href="#">EXAMS</a></li>
                            <li><a class="dropdown-item" href="#">Closing</a></li>
                        </ul>
                    </li>
                    <!-- Gallery Dropdown -->
                    <li class="nav-item dropdown">
                        <a class="nav-link dropdown-toggle" href="#" id="galleryDropdown" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                            Gallery
                        </a>
                        <ul class="dropdown-menu" aria-labelledby="galleryDropdown">
                            <li><a class="dropdown-item" href="#">Photos</a></li>
                            <li><a class="dropdown-item" href="#">Videos</a></li>
                        </ul>
                    </li>
                    <!-- About Dropdown -->
                    <li class="nav-item dropdown">
                        <a class="nav-link dropdown-toggle" href="#" id="aboutDropdown" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                            About
                        </a>
                        <ul class="dropdown-menu" aria-labelledby="aboutDropdown">
                            <li><a class="dropdown-item" href="#">Contact</a></li>
                            <li><a class="dropdown-item" href="#">Email</a></li>
                        </ul>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
    <!-- Include Bootstrap JavaScript -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
    <div class="container mt-5">
        <h2 class="text-center">Search for Students, Teachers, or Events</h2>
        <form action="search_results.php" method="GET" class="d-flex justify-content-center">
          <div class="form-group mr-2">
            <input type="text" name="query" class="form-control" placeholder="Enter name, event, etc." required>
          </div>
          <button type="submit" class="btn btn-primary">Search</button>
        </form>
      </div>
      <!-- Bootstrap JS, Popper.js, and jQuery -->
      <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
      <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.9.1/dist/umd/popper.min.js"></script>
      <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>

      
<div class="container mt-5">
    <div class="row justify-content-between align-items-center">
        
        <!-- Parent's Portal - Left -->
        <div class="col-md-3">
            <div class="card shadow-lg">
                <div class="card-header bg-primary text-white text-center">
                    <h5>Parent's Portal</h5>
                </div>
                <div class="card-body">
                    <form action="parent_login.php" method="POST">
                        <div class="mb-2">
                            <label for="parentUsername" class="form-label">Username</label>
                            <input type="text" class="form-control" id="parentUsername" name="username" required>
                        </div>
                        <div class="mb-2">
                            <label for="parentPassword" class="form-label">Password</label>
                            <input type="password" class="form-control" id="parentPassword" name="password" required>
                        </div>
                        <div class="d-grid">
                            <button type="submit" class="btn btn-primary">Login</button>
                        </div>
                    </form>
                </div>
            </div>
        </div>
        <!-- Welcome Message - Center -->
        <div class="col-md-5 text-center">
            <h2 style="color: black; font-style: italic;">Welcome to Our School</h2>
            <p style="color: black; font-style: italic;">
                Providing quality education and a bright future for our students.
            </p>
        </div>
        <!-- Principal's Portal - Right -->
        <div class="col-md-3">
            <div class="card shadow-lg">
                <div class="card-header bg-dark text-white text-center">
                    <h5>Principal's Portal</h5>
                </div>
                <div class="card-body">
                    <form action="principal_login.php" method="POST">
                        <div class="mb-2">
                            <label for="username" class="form-label">Username</label>
                            <input type="text" class="form-control form-control-sm" id="username" name="username" required>
                        </div>
                        <div class="mb-2">
                            <label for="password" class="form-label">Password</label>
                            <input type="password" class="form-control form-control-sm" id="password" name="password" required>
                        </div>
                        <div class="d-grid">
                            <button type="submit" class="btn btn-dark btn-sm">Login</button>
                        </div>
                    </form>
                </div>
            </div>
        </div>

    </div>
</div>
    <div class="container mt-4">
        <h2 class="text-center mb-3">Image Gallery</h2>
        <div class="gallery-container d-flex">
            <img src="C:\Users\student\Pictures\Benja phot.jpg" alt="Image 1">
            <img src="https://via.placeholder.com/200x150" alt="Image 2">
            <img src="https://via.placeholder.com/200x150" alt="Image 3">
            <img src="https://via.placeholder.com/200x150" alt="Image 4">
            <img src="https://via.placeholder.com/200x150" alt="Image 5">
            <img src="https://via.placeholder.com/200x150" alt="Image 6">
            <img src="https://via.placeholder.com/200x150" alt="Image 7">
            <img src="https://via.placeholder.com/200x150" alt="Image 8">
            <img src="https://via.placeholder.com/200x150" alt="Image 9">
            <img src="https://via.placeholder.com/200x150" alt="Image 10">
            <img src="https://via.placeholder.com/200x150" alt="Image 11">
            <img src="https://via.placeholder.com/200x150" alt="Image 12">
            <img src="https://via.placeholder.com/200x150" alt="Image 13">
            <img src="https://via.placeholder.com/200x150" alt="Image 14">
            <img src="https://via.placeholder.com/200x150" alt="Image 15">
            <img src="https://via.placeholder.com/200x150" alt="Image 16">
            <img src="https://via.placeholder.com/200x150" alt="Image 17">
            <img src="https://via.placeholder.com/200x150" alt="Image 18">
            <img src="https://via.placeholder.com/200x150" alt="Image 19">
            <img src="https://via.placeholder.com/200x150" alt="Image 20">
        </div>
    </div>
    <div class="row g-4">
        <div class="col-md-6">
            <div class="card p-4">
                <h3 class="text-center">Online Homework Portal</h3>
                <input type="text" class="form-control mb-2" placeholder="Student Name">
                <input type="file" class="form-control mb-2">
                <button class="btn btn-primary w-100">Submit Homework</button>
            </div>
        </div>
        <div class="col-md-6">
            <div class="card p-4">
                <h3 class="text-center">Exam Results Portal</h3>
                <input type="text" class="form-control mb-2" placeholder="Student ID">
                <button class="btn btn-success w-100">Check Results</button>
            </div>
        </div>
    </div>
    <div class="row g-4 mt-4">
        <div class="col-md-6">
            <div class="card p-4">
                <h3 class="text-center">School Timetable</h3>
                <button class="btn btn-info w-100 mb-2" onclick="toggleTimetable('form2NTimetable')">Form 2 North Timetable</button>
                <div id="form2NTimetable" class="fade-toggle">
                    <table class="table table-bordered table-striped">
                        <thead class="table-dark">
                            <tr>
                                <th>Time/Day</th><th>Monday</th><th>Tuesday</th><th>Wednesday</th><th>Thursday</th><th>Friday</th><th>Saturday</th><th>Sunday</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr>
                                <td>8:00 - 9:00</td><td>Math</td><td>English</td><td>History</td><td>Chemistry</td><td>Physics</td><td>Biology</td><td>CRE/IRE</td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </div>
        </div>
        <div class="col-md-6">
            <div class="card p-4">
                <h3 class="text-center">Online Fee Payment</h3>
                <input type="text" class="form-control mb-2" placeholder="Student ID">
                <select class="form-select mb-2">
                    <option value="credit">Credit Card</option>
                    <option value="mobile">Mobile Money</option>
                </select>
                <button class="btn btn-danger w-100">Pay Now</button>
            </div>
        </div>
    </div>
    <div class="container-fluid mt-4">
        <div class="d-flex justify-content-between">
            <!-- Class Teacher Login (Left) -->
            <div class="col-md-5">
                <div class="card p-4">
                    <h3 class="text-center">Class Teacher Login</h3>
                    <form action="class_teacher_login.php" method="POST">
                        <div class="mb-2">
                            <label for="teacherUsername" class="form-label">Username</label>
                            <input type="text" class="form-control" id="teacherUsername" name="username" required>
                        </div>
                        <div class="mb-2">
                            <label for="teacherPassword" class="form-label">Password</label>
                            <input type="password" class="form-control" id="teacherPassword" name="password" required>
                        </div>
                        <button type="submit" class="btn btn-dark w-100">Login</button>
                    </form>
                </div>
            </div>
            <!-- Attendance List (Right) -->
            <div class="col-md-5">
                <div class="card p-4">
                    <h3 class="text-center">Attendance List</h3>
                    <table class="table table-striped">
                        <thead>
                            <tr>
                                <th>Student Name</th>
                                <th>Status</th>
                            </tr>
                        </thead>
                        <tbody id="attendanceList"></tbody>
                    </table>
                </div>
            </div>
            
            <script>
                function markAttendance() {
                    let name = document.getElementById("studentName").value;
                    let status = document.getElementById("attendance").value;
                    
                    if (!name.trim()) {
                        alert("Please enter a student name.");
                        return;
                    }
            
                    let table = document.getElementById("attendanceList");
                    let newRow = table.insertRow();
            
                    newRow.insertCell(0).textContent = name;
                    let statusCell = newRow.insertCell(1);
                    statusCell.textContent = status;
            
                    // Add blinking and color classes
                    if (status.toLowerCase() === "present") {
                        statusCell.classList.add("blink", "present");
                    } else if (status.toLowerCase() === "absent") {
                        statusCell.classList.add("blink", "absent");
                    }
            
                    document.getElementById("studentName").value = "";
                }
            </script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
    <footer class="text-dark pt-4">
        <div class="container-fluid">
            <div class="row">
                <!-- Quick Links -->
                <div class="col-md-3">
                    <h5>Quick Links</h5>
                    <ul class="list-unstyled">
                        <li><a href="#" class="text-dark">Home</a></li>
                        <li><a href="#" class="text-dark">Departments</a></li>
                        <li><a href="#" class="text-dark">Gallery</a></li>
                        <li><a href="#" class="text-dark">About</a></li>
                        <li><a href="#" class="text-dark">Events</a></li>
                        <li><a href="#" class="text-dark">Downloads</a></li>
                        <li><a href="#" class="text-dark">Blog</a></li>
                        <li><a href="#" class="text-dark">Contact Us</a></li>
                    </ul>
                </div>
    
                <!-- Related Links -->
                <div class="col-md-3">
                    <h5>Related Links</h5>
                    <ul class="list-unstyled">
                        <li><a href="#" class="text-dark">Teachers</a></li>
                        <li><a href="#" class="text-dark">Supporting staffs</a></li>
                        <li><a href="#" class="text-dark">School Library</a></li>
                        <li><a href="#" class="text-dark">Prefects' body</a></li>
                        <li><a href="#" class="text-dark">Assemblies</a></li>
                    </ul>
                </div>
    
                <!-- Newsletter -->
                <div class="col-md-3">
                    <h5>Newsletter</h5>
                    <p>Download our quarterly briefs below</p>
                    <a href="#" class="btn btn-outline-dark btn-sm">Download</a>
                </div>
    
                <!-- Social Media -->
                <div class="col-md-3">
                    <h5>Get Us On Social Media</h5>
                    <div class="social-media">
                        <a href="https://facebook.com/kipinihighschool" target="_blank"><img src="https://img.icons8.com/ios-filled/50/ffffff/facebook.png" alt="Facebook" width="30" height="30"></a>
                        <a href="https://twitter.com/kipinihighschool" target="_blank"><img src="https://img.icons8.com/ios-filled/50/ffffff/twitter.png" alt="Twitter" width="30" height="30"></a>
                        <a href="https://instagram.com/kipinihighschool" target="_blank"><img src="https://img.icons8.com/ios-filled/50/ffffff/instagram.png" alt="Instagram" width="30" height="30"></a>
                        <a href="https://linkedin.com/school/kipinihighschool" target="_blank"><img src="https://img.icons8.com/ios-filled/50/ffffff/linkedin.png" alt="LinkedIn" width="30" height="30"></a>
                    </div>
                </div>
            </div>
    
            <hr class="bg-dark">

<footer>
    <div class="container">
        <div class="text-center pb-3">
            <p class="mb-0">&copy; 2025 KIPINI HIGH SCHOOL. All rights reserved.</p>
            <p>Contact +254703465552</p>
        </div>
    </div>
</footer>

<!-- Include Font Awesome for social media icons -->
<script src="https://kit.fontawesome.com/YOUR_KIT_CODE.js" crossorigin="anonymous"></script>

    
</body>
</html>




