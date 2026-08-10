💻 Step-by-Step Project BlueprintStep 1 — Setup Git Identitybashgit config --global user.name "achalkumarigupta"
git config --global user.email "achalgupta7722@gmail.com"
Use code with caution.Step 2 — Verify Identitybashgit config --global user.name
git config --global user.email
Use code with caution.Expected Output:textachalkumarigupta
achalgupta7722@gmail.com
Use code with caution.Step 3 — Create and Enter Project Folderbashmkdir "STUDENT PROJECT"
cd "STUDENT PROJECT"
Use code with caution.Step 4 — Initialize Gitbashgit init
Use code with caution.Step 5 — Create the 5 Filesbashtouch login.html student.html admin.html teacher.html courses.html
Use code with caution.Step 6 — Add Code to login.htmlOpen login.html and paste:html<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login - Student Management System</title>
</head>
<body>
    <h1>Student Management System</h1>
    <h2>Login</h2>
    <form action="student.html">
        <label for="username">Username:</label><br>
        <input type="text" id="username" name="username" required><br><br>
        <label for="password">Password:</label><br>
        <input type="password" id="password" name="password" required><br><br>
        <input type="submit" value="Login">
    </form>
</body>
</html>
Use code with caution.Step 7 — Add Code to student.htmlOpen student.html and paste:html<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Student Dashboard</title>
</head>
<body>
    <h1>Student Dashboard</h1>
    <p>Welcome, Student!</p>
    <hr>
    <nav>
        <ul>
            <li><a href="courses.html">View Courses</a></li>
            <li><a href="teacher.html">Teacher Information</a></li>
            <li><a href="admin.html">Admin Panel</a></li>
            <li><a href="login.html">Logout</a></li>
        </ul>
    </nav>
</body>
</html>
Use code with caution.Step 8 — Add Code to courses.htmlOpen courses.html and paste:html<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Available Courses</title>
</head>
<body>
    <h1>Available Courses</h1>
    <ul>
        <li>Computer Science</li>
        <li>Information Technology</li>
        <li>Data Science</li>
    </ul>
    <br>
    <a href="student.html">Back to Dashboard</a>
</body>
</html>
Use code with caution.Step 9 — Add Code to teacher.htmlOpen teacher.html and paste:html<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Teacher Information</title>
</head>
<body>
    <h1>Teacher Details</h1>
    <p>Your Class Teacher: Prof. Sharma</p>
    <p>Email: sharma@college.com</p>
    <br>
    <a href="student.html">Back to Dashboard</a>
</body>
</html>
Use code with caution.Step 10 — Add Code to admin.htmlOpen admin.html and paste:html<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Admin Dashboard</title>
</head>
<body>
    <h1>Admin Dashboard</h1>
    <p>Welcome to the Student Management System Admin Panel.</p>
    <hr>
    <h2>Student Records</h2>
    <table border="1" cellpadding="10">
        <tr>
            <th>Student ID</th>
            <th>Name</th>
            <th>Course</th>
            <th>Status</th>
        </tr>
        <tr>
            <td>20241CDV0021</td>
            <td>Achal Kumar Gupta</td>
            <td>Computer Science</td>
            <td>Active</td>
        </tr>
    </table>
    <hr>
    <h2>Admin Options</h2>
    <ul>
        <li>Add Student</li>
        <li>Remove Student</li>
        <li>Manage Courses</li>
    </ul>
    <br>
    <a href="student.html">Student Dashboard</a><br><br>
    <a href="login.html">Logout</a>
</body>
</html>
Use code with caution.Step 11 — Create Version 1 in Gitbashgit add .
git commit -m "Initial student project - Version 1"
Use code with caution.Step 12 — Link to GitHubbashgit branch -M main
git remote add origin https://github.com
git push -u origin main
Use code with caution.Step 13 — Create Version 2 (Make a Change)Open login.html and change <h1>Student Management System</h1> to <h1>Student Management System - Version 2</h1>. Then run:bashgit status
git add login.html
git commit -m "Version 2 - Updated login page heading"
git push     









📋 Phase 1 — Global Identity SetupRun these commands in your Git Bash terminal once to set up your profile:bashgit config --global user.name "achalkumarigupta"
git config --global user.email "achalgupta7722@gmail.com"
Use code with caution.Verify your registration details:bashgit config --global user.name
git config --global user.email
Use code with caution.📁 Phase 2 — Level 1: Local Setup & Basic ChangesInitialize Project: Run mkdir "StudentProject", cd "StudentProject", and git init.Create Files: Run touch login.html home.html faculty.html student.html hod.html README.md.Code Implementation: Create the 5 HTML files (login, home, faculty, student, hod) with unique content and a README.md file (similar to the structure provided in the original instructions).Initial Commit: Run git add . and git commit -m "Initial version of Student Management System".Push to Remote: Run git branch -M main, git remote add origin https://github.com, and git push -u origin main.🌿 Phase 3 — Level 2: Feature Branching & MergesCreate Feature Branches: Run git switch -c faculty-feature and git switch -c student-feature to isolate changes.Make Changes: Modify faculty.html and student.html with new content.Commit Changes: Use git add <file> and git commit -m "..." for each file.Push Branches: Run git push -u origin <branch-name>.Merge & Push: Switch back to main (git switch main), merge branches (git merge <branch-name>), and git push.🔄 Project Architecture Visual Flow Diagramtext                  [faculty-feature Branch] ➔ [Modify faculty.html] ➔ [Commit & Push] ──┐
                 /                                                                     ▼
[Local Main Branch] ➔ [Initial Commit] ➔ [Link Remote]                               [Merge into Main] ➔ [Final Git Push]
                 \                                                                     ▲
                  [student-feature Branch] ➔ [Modify student.html] ➔ [Commit & Push] ──┘
Use code with caution.Would you like to explore resolving merge conflicts next, or do you want to start building a custom CSS visual layout framework for your five screens?