<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Student Management System</title>

    <style>
        .logo::before {
            content: '';
            position: absolute;
            width: 120%;
            height: 120%;
            top: -10%;
            left: -10%;
            background: radial-gradient( circle, rgba(0, 229, 255, .15), transparent 70%);
            z-index: -1;
            animation: pulseGlow 3s infinite;
        }
        
        @keyframes pulseGlow {
            0% {
                transform: scale(1);
                opacity: .5;
            }
            50% {
                transform: scale(1.2);
                opacity: 1;
            }
            100% {
                transform: scale(1);
                opacity: .5;
            }
        }
        
        .hero {
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 0 20px;
        }
        
        .hero-content {
            max-width: 900px;
            margin: auto;
        }
        
        .hero-badge {
            display: inline-block;
            padding: 10px 20px;
            background: rgba(0, 255, 255, 0.12);
            border: 1px solid rgba(0, 255, 255, 0.3);
            border-radius: 50px;
            color: #00ffff;
            font-size: 14px;
            font-weight: 600;
            margin-bottom: 25px;
        }
        
        .hero-content h1 {
            font-size: 64px;
            color: #ffffff;
            font-weight: 700;
            margin-bottom: 25px;
            line-height: 1.2;
        }
        
        .hero-content p {
            font-size: 20px;
            line-height: 1.8;
            color: #cbd5e1;
            max-width: 750px;
            margin: 0 auto 35px;
        }
        
        .hero-btn {
            display: inline-block;
            padding: 15px 35px;
            text-decoration: none;
            border-radius: 12px;
            background: linear-gradient(135deg, #2563eb, #06b6d4);
            color: #fff;
            font-size: 17px;
            font-weight: 600;
            transition: 0.3s;
        }
        
        .hero-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 25px rgba(37, 99, 235, .4);
        }
        
        html {
            scroll-behavior: smooth;
        }
        
        .navbar {
            position: fixed;
            top: 0;
            width: 100%;
            padding: 18px 50px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            background: rgba(15, 23, 42, .75);
            backdrop-filter: blur(18px);
            border-bottom: 1px solid rgba(255, 255, 255, .08);
            z-index: 1000;
        }
        
        .logo {
            font-size: 32px;
            font-weight: 800;
            letter-spacing: 1px;
            color: #ffffff;
            position: relative;
            cursor: pointer;
            transition: 0.4s ease;
            animation: logoFloat 4s ease-in-out infinite;
        }
        
        .logo span {
            background: linear-gradient(135deg, #00e5ff, #2563eb);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            text-shadow: 0 0 15px rgba(0, 229, 255, .4);
        }
        
        .logo::after {
            content: '';
            position: absolute;
            left: 0;
            bottom: -8px;
            width: 0;
            height: 3px;
            background: linear-gradient(90deg, #00e5ff, #2563eb);
            transition: 0.5s;
            border-radius: 10px;
        }
        
        .logo:hover::after {
            width: 100%;
        }
        
        .logo:hover {
            transform: scale(1.05);
        }
        
        @keyframes logoFloat {
            0% {
                transform: translateY(0px);
            }
            50% {
                transform: translateY(-4px);
            }
            100% {
                transform: translateY(0px);
            }
        }
        
        .navbar nav a {
            color: white;
            text-decoration: none;
            margin-left: 25px;
            font-weight: 600;
        }
        
        .hero {
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 50px;
        }
        
        .hero-content {
            max-width: 900px;
        }
        
        .hero-content h1 {
            font-size: 65px;
            color: white;
            line-height: 1.2;
            margin-bottom: 20px;
        }
        
        .hero-content p {
            font-size: 22px;
            color: #cbd5e1;
            margin-bottom: 35px;
        }
        
        .hero-btn {
            display: inline-block;
            padding: 16px 35px;
            background: linear-gradient(45deg, #00ffff, #0066ff);
            color: white;
            text-decoration: none;
            border-radius: 12px;
            font-size: 18px;
            font-weight: bold;
        }
        
        .hero-btn:hover {
            box-shadow: 0 0 25px cyan;
        }
        
        .features {
            padding: 120px 50px;
        }
        
        .features h2 {
            color: white;
            text-align: center;
            font-size: 42px;
            margin-bottom: 50px;
        }
        
        .feature-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 25px;
        }
        
        .card {
            background: rgba(255, 255, 255, .08);
            backdrop-filter: blur(10px);
            padding: 30px;
            border-radius: 20px;
            color: white;
            transition: .3s;
        }
        
        .card:hover {
            transform: translateY(-10px);
            box-shadow: 0 0 25px rgba(0, 255, 255, .4);
        }
        
        .card h3 {
            margin-bottom: 15px;
            color: #00ffff;
        }
        
        #dashboard {
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', sans-serif;
        }
        
        body {
            min-height: 100vh;
            background: radial-gradient(circle at top left, #1e3a8a 0%, transparent 35%), radial-gradient(circle at bottom right, #0891b2 0%, transparent 35%), #0f172a;
            color: white;
        }
        
        .container {
            width: 900px;
            padding: 30px;
            border-radius: 20px;
            backdrop-filter: blur(15px);
            background: rgba(255, 255, 255, 0.08);
            border: 1px solid rgba(255, 255, 255, 0.15);
            box-shadow: 0 0 40px rgba(0, 255, 255, .2);
        }
        
        .container h1 {
            text-align: center;
            margin-bottom: 25px;
            color: #fff;
            font-size: 36px;
        }
        
        h1 {
            text-align: center;
            color: #fff;
            margin-bottom: 25px;
            font-size: 35px;
            letter-spacing: 2px;
            text-transform: uppercase;
        }
        
        .top-bar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
        }
        
        .container {
            width: 90%;
            max-width: 900px;
            margin: 50px auto;
            padding: 30px;
            border-radius: 20px;
            backdrop-filter: blur(15px);
            background: rgba(255, 255, 255, 0.08);
            border: 1px solid rgba(255, 255, 255, 0.15);
            box-shadow: 0 0 40px rgba(0, 255, 255, .15);
        }
        
        .counter p {
            margin-top: 10px;
            color: #cbd5e1;
            font-size: 15px;
            letter-spacing: 1px;
        }
        
        #dashboard {
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 100px 20px;
        }
        
        .search {
            width: 250px;
            padding: 10px;
            border: none;
            outline: none;
            border-radius: 10px;
        }
        
        .form-group {
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 15px;
            margin-bottom: 25px;
            flex-wrap: wrap;
        }
        
        .form-group input {
            width: 280px;
            padding: 14px;
            border: none;
            border-radius: 10px;
            outline: none;
        }
        
        input {
            flex: 1;
            padding: 14px;
            border: none;
            border-radius: 10px;
            outline: none;
            font-size: 15px;
        }
        
        button {
            border: none;
            padding: 14px 20px;
            border-radius: 10px;
            cursor: pointer;
            font-weight: bold;
            transition: .3s;
        }
        
        .add-btn {
            background: linear-gradient(45deg, #00ffff, #0066ff);
            color: white;
        }
        
        .add-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 0 20px cyan;
        }
        
        table {
            width: 100%;
            margin: 0 auto;
            border-collapse: collapse;
        }
        
        thead {
            background: linear-gradient(45deg, #00ffff, #0066ff);
        }
        
        th {
            color: white;
            padding: 15px;
        }
        
        td {
            color: white;
            padding: 15px;
            text-align: center;
            background: rgba(255, 255, 255, 0.05);
        }
        
        tr:hover td {
            background: rgba(0, 255, 255, .15);
        }
        
        .delete-btn {
            background: #ff3b3b;
            color: white;
        }
        
        .delete-btn:hover {
            background: #ff0000;
            transform: scale(1.05);
        }
        
        .empty {
            text-align: center;
            color: #ccc;
            padding: 20px;
        }
    </style>
</head>

<body>
    <header class="navbar">
        <div class="logo">
            <span>R</span>UDRA <span>P</span>ATEL
        </div>

        <nav>
            <a href="#home">Home</a>
            <a href="#features">Features</a>
            <a href="#dashboard">Dashboard</a>
        </nav>
    </header>

    <section class="hero">

        <div class="hero-content">

            <span class="hero-badge">
            Student Information System
        </span>

            <h1>
                Student Management System
            </h1>

            <p>
                A centralized platform for managing student records, course information, and academic details. The system helps educational institutions maintain accurate data, improve accessibility, and simplify administrative tasks.
            </p>

            <a href="#dashboard" class="hero-btn">
            View Dashboard
        </a>

        </div>

    </section>

    <section id="features" class="features">

        <h2>Platform Features</h2>

        <div class="feature-grid">

            <div class="card">
                <h3>Student Records</h3>
                <p>
                    Store and manage student data securely and efficiently.
                </p>
            </div>

            <div class="card">
                <h3>Course Tracking</h3>
                <p>
                    Organize courses and academic information with ease.
                </p>
            </div>

            <div class="card">
                <h3>Fast Performance</h3>
                <p>
                    Optimized interface with real-time updates and responsiveness.
                </p>
            </div>

        </div>

    </section>

    <section id="dashboard">
        <div class="container">
            <h1>Student Management System</h1>

            <div class="form-group">
                <input type="text" id="name" placeholder="Student Name">
                <input type="text" id="course" placeholder="Course">
                <button class="add-btn" onclick="addStudent()">
    Add Student
</button> </div>

            <table>
                <thead>
                    <tr>
                        <th>ID</th>
                        <th>Name</th>
                        <th>Course</th>
                        <th>Action</th>
                    </tr>
                </thead>
                <tbody id="studentTable">
                </tbody>
            </table>
        </div>

        <script>
            function updateCounter() {
                document.getElementById("studentCount").innerText =
                    students.length;
            }

            function searchStudent() {

                const searchValue =
                    document.getElementById("search")
                    .value.toLowerCase();

                const rows =
                    document.querySelectorAll("#studentTable tr");

                rows.forEach(row => {

                    const text =
                        row.innerText.toLowerCase();

                    row.style.display =
                        text.includes(searchValue) ?
                        "" :
                        "none";
                });
            }
            let students = [];
            let id = 1;

            function addStudent() {

                const name = document.getElementById("name").value.trim();
                const course = document.getElementById("course").value.trim();

                if (name === "" || course === "") {
                    alert("Please fill all fields");
                    return;
                }

                students.push({
                    id: id++,
                    name: name,
                    course: course
                });

                document.getElementById("name").value = "";
                document.getElementById("course").value = "";

                displayStudents();
            }

            function deleteStudent(studentId) {
                students = students.filter(
                    student => student.id !== studentId
                );

                displayStudents();
            }

            function displayStudents() {

                const table =
                    document.getElementById("studentTable");

                table.innerHTML = "";

                students.forEach(student => {

                    table.innerHTML += `
        <tr>
            <td>${student.id}</td>
            <td>${student.name}</td>
            <td>${student.course}</td>
            <td>
                <button
                    class="delete-btn"
                    onclick="deleteStudent(${student.id})">
                    Delete
                </button>
            </td>
        </tr>
        `;
                });
            }
        </script>

</body>

</html>
