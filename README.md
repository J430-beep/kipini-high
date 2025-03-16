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
               background-color: palegreen;
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
                background: linear-gradient(to right, hwb(253 0% 20%), hwb(249 7% 7%));
                color: white;
                padding: 15px;
                text-align: center;
                font-size: 24px;
                width: 100%;
            }
            .navbar {
                border: 4px solid hsl(253, 83%, 47%);
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
                background-color: hsl(246, 89%, 45%);
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
                background-color: hsl(241, 87%, 44%);
                color: white;
                padding: 20px;
                text-align: center;
                width: 100%;
            }
    
            footer a {
                transition: color 0.3s ease;
            }
    
            footer a:hover {
                color: #007bff;
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
            .gallery {
    display: flex;
    flex-direction: row; /* Arrange videos in a row */
    gap: 10px; /* Space between videos */
    overflow-x: auto; /* Enables horizontal scrolling if needed */
    white-space: nowrap; /* Prevents wrapping */
}

.gallery-item video {
    width: 250px; /* Adjust width as needed */
    height: auto;
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
                .main-content {
                    flex-direction: column;
                    align-items: flex-start;
                }
            }


            .cardd-containerr {
    display: flex;
    justify-content: space-around; /* Distributes items evenly */
    align-items: center; /* Aligns items in a single line */
    flex-wrap: nowrap; /* Prevents wrapping to a new line */
    gap: 20px; /* Adds spacing between cards */
    overflow-x: auto; /* Enables horizontal scrolling if necessary */
    padding: 10px;
}

.cardd {
    text-align: center;
    background-color: white;
}

.cardd img {
    width: 120px; /* Adjust the size for a perfect circle */
    height: 120px;
    border-radius: 50%; /* Makes the image circular */
    object-fit: cover; /* Ensures the image fits properly */
    display:block;
    margin: 0 auto; /* Centers the image */
    border: 3px solid #007bff; /* Optional: Adds a border */
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
        <h2 class="text-center" style="color: black;">Search for Students, Teachers, or Events</h2>
<form action="search_results.php" method="GET" class="d-flex justify-content-center" style="color: black;">
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

    <div class="row mt-4">
        <div class="col-md-12">
            <h1 class="text-center bg-info text-white p-3 rounded-3 shadow">SCHOOL'S HISTORY</h1>
            <button class="btn btn-secondary w-100 mb-3 rounded-pill shadow-sm" onclick="toggleHistory()">Show History</button>
                <div id="history" class="p-4 border rounded-4 bg-light shadow-lg" style="display: none; color: black; font-style: italic;">
                <p>
                    Kipini High School, established in 1986, was founded by a group of visionary educators and community leaders with the mission of providing quality education to the local community. Located in the heart of Kipini, the school began with just a few classrooms and a handful of students. The founders were driven by the belief that education is the key to unlocking opportunities and empowering the youth of the region to achieve their fullest potential.
                </p>
                <p>
                    In its early years, Kipini High School faced many challenges, from limited resources to a lack of infrastructure. However, the strong sense of community support and the dedication of the staff ensured that the school persevered. The local community contributed generously to building classrooms, providing educational materials, and supporting the school’s growth. Over the years, the school’s physical infrastructure expanded, and it became a well-known institution in the region.
                </p>
                <p>
                    The school initially offered a broad range of subjects, including traditional subjects like Mathematics, English, and Sciences, but soon began to integrate more modern disciplines such as ICT and foreign languages. This shift was in response to the growing demand for a more diverse curriculum that would prepare students for an increasingly globalized world. The curriculum was designed to foster both academic excellence and holistic development, emphasizing the importance of character building alongside academic achievements.
                </p>
                <p>
                    Kipini High School’s commitment to excellence in education has been reflected in its consistently strong performance in national exams. Year after year, the school’s students have excelled, particularly in subjects like Mathematics, English, and Science. The school has produced numerous top performers who have gone on to achieve great success in higher education and professional careers.
                </p>
                <p>
                    Beyond academics, the school places great emphasis on extracurricular activities. Kipini High School is known for its active sports programs, including football, basketball, and athletics. The school has won several regional and national awards in various sports, showcasing the talents of its students. Additionally, cultural events, debates, and drama performances are regularly held, providing students with opportunities to showcase their talents in the arts.
                </p>
                <p>
                    The school is also home to a vibrant leadership program. Students are encouraged to take on leadership roles through student councils, clubs, and peer mentorship programs. These opportunities help develop essential life skills such as communication, teamwork, and problem-solving, which are invaluable in both academic and personal development. Leadership is seen as an integral part of the school’s mission to produce well-rounded individuals who will make positive contributions to society.
                </p>
                <p>
                    One of the school’s core values is community service. Students are regularly involved in local community projects, such as environmental conservation, charity events, and educational outreach programs. This helps foster a sense of social responsibility and encourages students to think beyond themselves. It also strengthens the school’s connection with the local community, which continues to play a vital role in its success.
                </p>
                <p>
                    Technology has become a key part of Kipini High School’s educational approach. The school is equipped with modern computer labs, and students are taught to use technology not only for academic purposes but also to enhance their creativity and problem-solving abilities. With the rise of online learning, the school has embraced digital platforms for remote learning and online assignments, ensuring that students remain engaged and supported even during times of disruption.
                </p>
                <p>
                    In the years ahead, Kipini High School continues to expand its facilities and curriculum to meet the evolving needs of its students. New programs, such as coding, robotics, and entrepreneurship, are being introduced to equip students with skills relevant to the modern job market. The school remains committed to its mission of providing an excellent education and creating a nurturing environment where students can grow into responsible, capable citizens.
                </p>
                <p>
                    As Kipini High School looks to the future, it does so with confidence. The foundation laid by its founders, combined with the tireless efforts of its staff and students, ensures that the school will remain a beacon of educational excellence for years to come. With a continued focus on academic achievement, extracurricular involvement, community service, and leadership development, Kipini High School is poised to remain a key player in shaping the future of its students and the community at large.
                </p>
            </div>
        </div>
    </div>
    <script>
        function toggleHistory() {
            var historyDiv = document.getElementById("history");
            if (historyDiv.style.display === "none") {
                historyDiv.style.display = "block";
            } else {
                historyDiv.style.display = "none";
            }
        }
    </script>


<h2 style="color: black;">School Administrators</h2>

<div class="cardd-containerr">
    <div class="cardd">
        <img src="c:\Users\student\Desktop\principal2.jpg" alt="Person 1">
        <div class="containerr">
            <h4><b>Principal</b></h4>
            <p style="color: black;">Principal</p><p style="color: black;">Mr.Amin Swaleh</p>
        </div>
    </div>

    <div class="cardd">
        <img src="c:\Users\student\Desktop\Deputy2.jpg" alt="Person 2">
        <div class="containerr">
            <h4><b>Deputy Principal</b></h4>
            <p style="color: black;">D.Principal</p><p style="color: black;">Mr.Hassan Rashid</p>
        </div>
    </div>

    <div class="cardd">
        <img src="c:\Users\student\Desktop\Kamau1.jpg" alt="Event 1">
        <div class="containerr">
            <h4><b>Senior Teacher</b></h4>
            <p style="color: black;">Senior Teacher</p><p style="color: black;">Mr.Kamau Caleb</p>
        </div>
    </div>

    <div class="cardd">
        <img src="c:\Users\student\Desktop\Abuga1.jpg" alt="Event 2">
        <div class="containerr">
            <h4><b>Sports Day</b></h4>
            <p style="color: black;">Dean Of Studies</p><p style="color: black;">Mr.Abuga Joseph</p>
        </div>
    </div>

    <div class="cardd">
        <img src="c:\Users\student\Desktop\boarding master 2.jpg" alt="Online Classes">
        <div class="containerr">
            <h4><b>Online Learning</b></h4>
            <p style="color: black;">Boarding Master</p><p style="color: black;">Mr.Benjamin Murimi</p>
        </div>
    </div>
</div>
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
            <img src="C:\Users\student\Desktop\software.jpg" alt="Image 1">
            <img src="C:\Users\student\Desktop\software2.jpg" alt="Image 2">
            <img src="C:\Users\student\Desktop\website 2.jpg" alt="Image 3">
            <img src="C:\Users\student\Desktop\website image 4.jpg" alt="Image 4">
            <img src="C:\Users\student\Desktop\website image 5.jpg" alt="Image 5">
            <img src="C:\Users\student\Desktop\website image 6.jpg" alt="Image 6">
            <img src="C:\Users\student\Pictures\2024 PASSPORTS\NUMBERED PASSPORTS\.trashed-1739523251-2766.jpg" alt="Image 7">
            <img src="C:\Users\student\Pictures\2024 PASSPORTS\NUMBERED PASSPORTS\.trashed-1739523251-2810.jpg" alt="Image 8">
            <img src="C:\Users\student\Pictures\2024 PASSPORTS\NUMBERED PASSPORTS\.trashed-1739523247-2701.jpg" alt="Image 9">
            <img src="C:\Users\student\Pictures\2024 PASSPORTS\NUMBERED PASSPORTS\.trashed-1739523221-2716.jpg" alt="Image 10">
            <img src="C:\Users\student\Pictures\2024 PASSPORTS\NUMBERED PASSPORTS\.trashed-1739523232-2768.jpg" alt="Image 11">
            <img src="C:\Users\student\Pictures\2024 PASSPORTS\NUMBERED PASSPORTS\.trashed-1739523248-2676.jpg" alt="Image 12">
            <img src="C:\Users\student\Pictures\2024 PASSPORTS\NUMBERED PASSPORTS\.trashed-1739523235-2686.jpg" alt="Image 13">
            <img src="C:\Users\student\Pictures\2024 PASSPORTS\NUMBERED PASSPORTS\.trashed-1739523222-2531.jpg" alt="Image 14">
            <img src="C:\Users\student\Pictures\2024 PASSPORTS\NUMBERED PASSPORTS\.trashed-1739523241-2708.jpg" alt="Image 15">
            <img src="C:\Users\student\Pictures\2024 PASSPORTS\NUMBERED PASSPORTS\.trashed-1739523223-2724.jpg" alt="Image 16">
            <img src="C:\Users\student\Pictures\2024 PASSPORTS\NUMBERED PASSPORTS\.trashed-1739523233-2677.jpg" alt="Image 17">
            <img src="C:\Users\student\Pictures\2024 PASSPORTS\NUMBERED PASSPORTS\.trashed-1739523240-2790.jpg" alt="Image 18">
            <img src="C:\Users\student\Pictures\2024 PASSPORTS\NUMBERED PASSPORTS\.trashed-1739523240-2812.jpg" alt="Image 19">
    </div> 
    <div class="gallery">
        <div class="gallery-item">
            <video controls>
                <source src="C:\Users\student\Desktop\website video 1.mp4" type="video/mp4">
            </video>
        </div>
        <div class="gallery-item">
            <video controls>
                <source src="C:\Users\student\Desktop\video website 3.mp4" type="video/mp4">
            </video>
        </div>
        <div class="gallery-item">
            <video controls>
                <source src="C:\Users\student\Desktop\website video 2.mp4" type="video/mp4">
            </video>
        </div>
         <div class="gallery-item">
            <video controls>
                <source src="C:\Users\student\Desktop\vide website 5.mp4" type="video/mp4">
            </video>
         </div>
    </div>
    <script>
        // Get all video elements
        const videos = document.querySelectorAll(".gallery-item video");
    
        videos.forEach(video => {
            video.addEventListener("play", function () {
                // Pause all other videos
                videos.forEach(v => {
                    if (v !== this) {
                        v.pause();
                    }
                });
            });
        });
    </script>    
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
    



    <div class="container-fluid mt-4">
        <div class="row d-flex justify-content-center gap-3">
            <!-- Form 2 North Timetable -->
            <div class="col-md-5">
                <div class="card p-4">
                    <h3 class="text-center">School Timetable</h3>
                    <button class="btn btn-info w-100 mb-2" onclick="toggleTimetable('form2NTimetable')">
                        Form 2 North Timetable
                    </button>
                    <div id="form2NTimetable" class="fade-toggle" style="display: none;">
                        <table class="table table-bordered table-striped">
                            <thead class="table-dark">
                                <tr>
                                    <th>Time/Day</th><th>Monday</th><th>Tuesday</th><th>Wednesday</th>
                                    <th>Thursday</th><th>Friday</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr><td>8:00 - 8:40</td><td>Math</td><td>English</td><td>History</td><td>Chemistry</td><td>Physics</td></tr>
                                <tr><td>8:40 - 9:20</td><td>Biology</td><td>Geography</td><td>Math</td><td>English</td><td>CRE</td></tr>
                                <tr class="table-warning"><td>Long Break</td><td colspan="5" class="text-center">Break</td></tr>
                                <tr><td>9:40 - 10:20</td><td>Physics</td><td>Math</td><td>English</td><td>History</td><td>Geography</td></tr>
                                <tr><td>10:20 - 11:00</td><td>Chemistry</td><td>CRE</td><td>Biology</td><td>Math</td><td>Physics</td></tr>
                                <tr class="table-warning"><td>Short Break</td><td colspan="5" class="text-center">Break</td></tr>
                                <tr><td>11:10 - 11:50</td><td>History</td><td>English</td><td>Physics</td><td>Geography</td><td>Chemistry</td></tr>
                                <tr><td>11:50 - 12:30</td><td>CRE</td><td>Math</td><td>Biology</td><td>English</td><td>History</td></tr>
                                <tr class="table-success"><td>LUNCH</td><td colspan="5" class="text-center">Lunch Break</td></tr>
                                <tr><td>2:00 - 2:40</td><td>Math</td><td>Physics</td><td>English</td><td>Biology</td><td>Geography</td></tr>
                                <tr><td>2:40 - 3:20</td><td>Chemistry</td><td>History</td><td>CRE</td><td>Math</td><td>English</td></tr>
                                <tr class="table-warning"><td>Break</td><td colspan="5" class="text-center">Break</td></tr>
                                <tr><td>3:30 - 4:10</td><td>Games</td><td>Games</td><td>Games</td><td>Games</td><td>Games</td></tr>
                            </tbody>
                        </table>
                    </div>
                </div>
            </div>
    
            <!-- Form 2 West Timetable -->
            <div class="col-md-5">
                <div class="card p-4">
                    <h3 class="text-center">Class Timetable</h3>
                    <button class="btn btn-info w-100 mb-2" onclick="toggleTimetable('form2WTimetable')">
                        Form 2 West Timetable
                    </button>
                    <div id="form2WTimetable" class="fade-toggle" style="display: none;">
                        <table class="table table-bordered table-striped">
                            <thead class="table-dark">
                                <tr>
                                    <th>Time/Day</th><th>Monday</th><th>Tuesday</th><th>Wednesday</th>
                                    <th>Thursday</th><th>Friday</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr><td>8:00 - 8:40</td><td>Geography</td><td>English</td><td>Math</td><td>Physics</td><td>Chemistry</td></tr>
                                <tr><td>8:40 - 9:20</td><td>Biology</td><td>Math</td><td>History</td><td>CRE</td><td>Physics</td></tr>
                                <tr class="table-warning"><td>Long Break</td><td colspan="5" class="text-center">Break</td></tr>
                                <tr><td>9:40 - 10:20</td><td>English</td><td>Physics</td><td>Geography</td><td>Math</td><td>CRE</td></tr>
                                <tr><td>10:20 - 11:00</td><td>Math</td><td>English</td><td>Chemistry</td><td>History</td><td>Physics</td></tr>
                                <tr class="table-warning"><td>Short Break</td><td colspan="5" class="text-center">Break</td></tr>
                                <tr><td>11:10 - 11:50</td><td>Physics</td><td>Math</td><td>English</td><td>Biology</td><td>Geography</td></tr>
                                <tr><td>11:50 - 12:30</td><td>CRE</td><td>History</td><td>Chemistry</td><td>Math</td><td>English</td></tr>
                                <tr class="table-success"><td>LUNCH</td><td colspan="5" class="text-center">Lunch Break</td></tr>
                                <tr><td>2:00 - 2:40</td><td>Math</td><td>Physics</td><td>History</td><td>English</td><td>CRE</td></tr>
                                <tr><td>2:40 - 3:20</td><td>Geography</td><td>Math</td><td>Physics</td><td>Biology</td><td>Chemistry</td></tr>
                                <tr class="table-warning"><td>Break</td><td colspan="5" class="text-center">Break</td></tr>
                                <tr><td>3:30 - 4:10</td><td>Games</td><td>Games</td><td>Games</td><td>Games</td><td>Games</td></tr>
                            </tbody>
                        </table>
                    </div>
                </div>
            </div>
        </div>
    </div>
    
    <script>
    function toggleTimetable(id) {
        var timetable = document.getElementById(id);
        if (timetable.style.display === "none" || timetable.style.display === "") {
            timetable.style.display = "block"; // Show table
        } else {
            timetable.style.display = "none"; // Hide table
        }
    }
    </script>
    
            





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
            newRow.insertCell(1).textContent = status;
            document.getElementById("studentName").value = "";
        }
    </script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
    <div class="container mt-5">
        <div class="row row-cols-1 row-cols-md-5 g-4">
            <div class="col">
                <div class="card h-100 text-dark">
                    <img src="https://via.placeholder.com/150" class="card-img-top" alt="Card Image">
                    <div class="card-body">
                        <h5 class="card-title">Announcements</h5>
                        <p class="card-text">Stay updated with the latest school news and notices.</p>
                        <a href="#" class="btn btn-primary">View More</a>
                    </div>
                </div>
            </div>
    
            <div class="col">
                <div class="card h-100 text-dark">
                    <img src="https://via.placeholder.com/150" class="card-img-top" alt="Card Image">
                    <div class="card-body">
                        <h5 class="card-title">Upcoming Events</h5>
                        <p class="card-text">Check out upcoming school events and activities.</p>
                        <a href="#" class="btn btn-primary">View More</a>
                    </div>
                </div>
            </div>
    
            <div class="col">
                <div class="card h-100 text-dark">
                    <img src="https://via.placeholder.com/150" class="card-img-top" alt="Card Image">
                    <div class="card-body">
                        <h5 class="card-title">Student Performance</h5>
                        <p class="card-text">Track your academic progress and performance.</p>
                        <a href="#" class="btn btn-primary">View More</a>
                    </div>
                </div>
            </div>
    
            <div class="col">
                <div class="card h-100 text-dark">
                    <img src="https://via.placeholder.com/150" class="card-img-top" alt="Card Image">
                    <div class="card-body">
                        <h5 class="card-title">School Gallery</h5>
                        <p class="card-text">Explore photos and videos from school events.</p>
                        <a href="#" class="btn btn-primary">View More</a>
                    </div>
                </div>
            </div>
    
            <div class="col">
                <div class="card h-100 text-dark">
                    <img src="https://via.placeholder.com/150" class="card-img-top" alt="Card Image">
                    <div class="card-body">
                        <h5 class="card-title">Online Payments</h5>
                        <p class="card-text">Make secure online payments for school fees.</p>
                        <a href="#" class="btn btn-primary">Pay Now</a>
                    </div>
                </div>
            </div>
        </div>
    </div>

    
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
    
            <!-- Copyright -->
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



