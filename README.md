<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Pawan | Coding Services</title>
    <link rel="icon" href="https://via.placeholder.com/64/000000/00eaff?text=P" />
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background: #000;
            color: #fff;
            overflow-x: hidden;
        }
        /* Animated Gradient Background */
        .bg-animate {
            position: fixed;
            top: 0; left: 0;
            width: 100%; height: 100%;
            background: linear-gradient(135deg, #001f3f, #000428, #004e92);
            background-size: 400% 400%;
            z-index: -1;
            animation: gradientShift 15s ease infinite;
        }
        @keyframes gradientShift {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        /* Fade-in animations */
        .fade {
            opacity: 0;
            transform: translateY(20px);
            animation: fadeUp 1.2s ease forwards;
        }
        @keyframes fadeUp {
            to { opacity: 1; transform: translateY(0); }
        }
        /* Floating WhatsApp Button */
        #floatWA {
            position: fixed;
            bottom: 20px;
            right: 20px;
            width: 60px;
            height: 60px;
            border-radius: 50%;
            background: #25D366;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 30px;
            color: white;
            text-decoration: none;
            box-shadow: 0 0 15px #25D366;
            z-index: 9999;
        }
        header {
            padding: 90px 20px;
            text-align: center;
        }
        .hero-title { font-size: 48px; font-weight: bold; }
        .typing {
            font-size: 22px;
            width: 0;
            white-space: nowrap;
            overflow: hidden;
            border-right: 3px solid #00eaff;
            animation: typing 4s steps(40) infinite alternate;
        }
        @keyframes typing {
            0% { width: 0; }
            100% { width: 350px; }
        }
        .btn {
            padding: 12px 28px;
            background: #00eaff;
            color: #000;
            border-radius: 8px;
            text-decoration: none;
            font-size: 18px;
            font-weight: bold;
            display: inline-block;
            margin-top: 20px;
        }
        .section {
            padding: 60px 20px;
            max-width: 1100px;
            margin: auto;
        }
        h2 { font-size: 32px; color: #00eaff; }
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(270px, 1fr));
            gap: 25px;
        }
        .card {
            background: #111;
            padding: 25px;
            border-radius: 16px;
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.5);
            transition: 0.3s;
        }
        .card:hover { transform: translateY(-8px); }
        form { background: #111; padding: 25px; border-radius: 12px; }
        input, textarea {
            width: 100%; padding: 10px; margin: 10px 0;
            background: #1a1a1a; border: 1px solid #333;
            color: white; border-radius: 8px;
        }
        footer { text-align: center; padding: 30px; background: #000; }
    </style>

    <script>
        window.onload = () => {
            document.querySelectorAll('.fade').forEach((el, i) => {
                el.style.animationDelay = (i * 0.3) + 's';
            });
        }
    </script>
</head>
<body>

<!-- Floating Navbar -->
<nav style="position:fixed;top:0;left:0;width:100%;padding:15px;background:#000a;backdrop-filter:blur(6px);z-index:999;display:flex;justify-content:space-between;align-items:center;">
    <div style="font-size:22px;color:#00eaff;font-weight:bold;">NeonCoder</div>
    <button onclick="toggleMode()" style="padding:8px 18px;border-radius:8px;border:none;background:#00eaff;color:#000;font-weight:bold;cursor:pointer;">Dark/Light</button>
</nav>
<script>
function toggleMode(){
    document.body.classList.toggle('light');
}
</script>
<style>
body.light{background:#fff;color:#000;}
body.light .card{background:#f2f2f2;color:#000;}
body.light h2{color:#005577;}
</style>


<!-- Animated Code Banner (Option D) -->
<div style="width:100%;padding:20px 0;background:#050505;box-shadow:0 0 20px #00eaff inset;overflow:hidden;white-space:nowrap;color:#00eaff;font-family:monospace;font-size:18px;">
    <marquee scrollamount="7">def hello(): print("Hello from NeonCoder") • for i in range(10): pass • import pandas as pd • console.log('Web Dev!') • public class Main {public static void main(String[] args){ }}</marquee>
</div>

<!-- Skills With Code (Option A) -->
<div class="section fade">
    <h2>My Coding Skills</h2>
    <div class="grid">
        <div class="card"><h3>Python</h3><pre style="white-space:pre-wrap;">import os
print("Automation Ready!")</pre></div>
        <div class="card"><h3>Java</h3><pre style="white-space:pre-wrap;">class Main { public static void main(String[] a){ }}</pre></div>
        <div class="card"><h3>C++</h3><pre style="white-space:pre-wrap;">#include<iostream>
int main(){ std::cout << "C++"; }</pre></div>
    </div>
</div>

<!-- Featured Project With Code (Option B) -->
<div class="section fade">
    <h2>Featured Project</h2>
    <div class="card">
        <h3>File Auto Sorter</h3>
        <pre style="white-space:pre-wrap;">import shutil, os
ext = {".png":"Images", ".txt":"Text"}
for f in os.listdir():
    e = os.path.splitext(f)[1]
    if e in ext: shutil.move(f, ext[e])</pre>
    </div>
</div>

<!-- Live Code Box (Option C) -->
<div class="section fade">
    <h2>Live Code Box</h2>
    <div class="card">
        <pre style="white-space:pre-wrap;">console.log("NeonCoder Live Box Ready!")</pre>
    </div>
</div>

<div class="bg-animate"></div>

<a id="floatWA" href="https://wa.me/message/A3K3YLYRSALHJ1?src=qr">💬</a>

<header class="fade">
    <img src="https://via.placeholder.com/130/000000/00eaff?text=PG" style="border-radius:50%;border:3px solid #00eaff;box-shadow:0 0 20px #00eaff;" />
    <div class="hero-title">NeonCoder</div>
    <div class="typing">Python • Websites • Automation • AI Tools</div>
    <a class="btn" href="#contact">Hire Me</a>
</header>

<div class="section fade">
    <h2>Services</h2>
    <div class="grid">
        <div class="card"><h3>Python Automation</h3><p>Scripts, tools, bots.</p></div>
        <div class="card"><h3>Websites</h3><p>Fast, clean pages.</p></div>
        <div class="card"><h3>Data Cleaning</h3><p>pandas-based work.</p></div>
        <div class="card"><h3>AI Tools</h3><p>AI images/videos.</p></div>
    </div>
</div>

<div class="section fade">
    <h2>Pricing</h2>
    <div class="grid">
        <div class="card"><h3>Basic Script</h3><p>₹200–₹500</p></div>
        <div class="card"><h3>Advanced Tool</h3><p>₹500–₹1500</p></div>
        <div class="card"><h3>Website</h3><p>₹700–₹2500</p></div>
    </div>
</div>

<div class="section fade">
    <h2>My Projects</h2>
    <div class="grid">
        <div class="card"><h3>File Organizer</h3></div>
        <div class="card"><h3>CSV Cleaner</h3></div>
        <div class="card"><h3>AI Image Maker</h3></div>
    </div>
</div>

<div class="section fade" id="contact">
    <h2>Contact</h2>
    <form>
        <label for="name">Your Name</label>
        <input id="name" type="text" placeholder="Your Name">
        <label for="email">Your Email</label>
        <input id="email" type="email" placeholder="Your Email">
        <label for="requirement">Your Requirement</label>
        <textarea id="requirement" rows="4" placeholder="Your Requirement"></textarea>
        <label for="contactemail">My Contact Email</label>
        <input id="contactemail" type="text" value="shreeramgoud28@gmail.com" readonly>
        <button class="btn" type="submit">Send</button>
    </form>
</div>

<footer>
    <a class="btn" href="resume.pdf" download>Download Resume</a><br><br>
    <a class="btn" href="mailto:shreeramgoud28@gmail.com">Email Me</a>
    <p>© 2025 NeonCoder — Coding Services</p>
</footer>

</body>
</html>
