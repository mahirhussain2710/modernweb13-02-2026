# 13-02-2026 MW
## Name:
### mahir hussain s
### 212223040109
## code:
index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>My Portfolio</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Navigation Bar -->
    <div class="navbar">
        <button class="tablink active" onclick="openTab(event,'home')">Home</button>
        <button class="tablink" onclick="openTab(event,'about')">About</button>
        <button class="tablink" onclick="openTab(event,'contact')">Contact</button>
    </div>

    <!-- Home -->
    <div id="home" class="tabcontent" style="display:block;">
        <div class="card">
            <h1>Welcome</h1>
            <p>Hello! I'm Mahir 👋</p>
            <p>A passionate Web Developer.</p>
        </div>
    </div>

    <!-- About -->
    <div id="about" class="tabcontent">
        <div class="card">
            <h1>About Me</h1>
            <p>I love building websites and solving programming problems.</p>
            <p><strong>Skills:</strong> HTML, CSS, JavaScript, Python</p>
        </div>
    </div>

    <!-- Contact -->
    <div id="contact" class="tabcontent">
        <div class="card">
            <h1>Contact Me</h1>
            <p>Email: yourmail@gmail.com</p>
            <p>Phone: 9876543210</p>
            <button class="contact-btn">Send Message</button>
        </div>
    </div>

    <script src="script.js"></script>
</body>
</html>
```
script.js
```
function openTab(evt, tabName) {
    var i, tabcontent, tablinks;

    tabcontent = document.getElementsByClassName("tabcontent");
    for (i = 0; i < tabcontent.length; i++) {
        tabcontent[i].style.display = "none";
    }

    tablinks = document.getElementsByClassName("tablink");
    for (i = 0; i < tablinks.length; i++) {
        tablinks[i].classList.remove("active");
    }

    document.getElementById(tabName).style.display = "block";
    evt.currentTarget.classList.add("active");
}
```
style.css
```
body {
    margin: 0;
    font-family: 'Segoe UI', sans-serif;
    background: linear-gradient(135deg, #667eea, #764ba2);
    color: white;
}

/* Navbar */
.navbar {
    display: flex;
    justify-content: center;
    background: rgba(0,0,0,0.3);
    padding: 15px;
}

.navbar button {
    background: transparent;
    border: none;
    color: white;
    padding: 12px 25px;
    font-size: 16px;
    cursor: pointer;
    transition: 0.3s;
    border-radius: 25px;
}

.navbar button:hover {
    background: white;
    color: #764ba2;
}

.navbar button.active {
    background: white;
    color: #764ba2;
}

/* Tab Content */
.tabcontent {
    display: none;
    padding: 60px 20px;
    text-align: center;
    animation: fadeEffect 0.6s;
}

@keyframes fadeEffect {
    from {opacity: 0;}
    to {opacity: 1;}
}

h1 {
    font-size: 40px;
    margin-bottom: 20px;
}

/* Card */
.card {
    background: rgba(255,255,255,0.15);
    padding: 30px;
    margin: auto;
    max-width: 500px;
    border-radius: 20px;
    box-shadow: 0 8px 20px rgba(0,0,0,0.3);
}

/* Contact Button */
.contact-btn {
    background: white;
    color: #764ba2;
    padding: 12px 20px;
    border: none;
    border-radius: 25px;
    cursor: pointer;
    margin-top: 15px;
    transition: 0.3s;
}

.contact-btn:hover {
    background: #764ba2;
    color: white;
}
```
## Screenshot:
<img width="1920" height="1080" alt="Screenshot (28)" src="https://github.com/user-attachments/assets/79dcd119-d5a6-4a7b-91a7-7eb531f7ed91" />
<img width="1920" height="1080" alt="Screenshot (27)" src="https://github.com/user-attachments/assets/16d19d77-c2a7-4df8-b4a9-193c950d2c5f" />
<img width="1920" height="1080" alt="Screenshot (26)" src="https://github.com/user-attachments/assets/7d55e120-7de9-4824-8cf2-f6a2001246ff" />

