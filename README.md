<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>THE REALM</title>
  
  <style>
    body {
  margin: 0;
  overflow-x: hidden;
}
    body {
      background: black;
      color: white;
      font-family: 'Courier New', Courier, monospace;
      margin: 0;
      padding: 0;
    }
    nav {
      background: #100010;
      padding: 10px;
      border-bottom: 2px solid purple;
    }
    nav ul {
      display: flex;
      justify-content: space-around;
      list-style: none;
      margin: 0;
      padding: 0;
    }
    nav a {
      text-decoration: none;
      color: #87ceeb;
      font-weight: bold;
    }
    h2 {
      text-decoration: underline;
      color: gold;
    }
    section {
      padding: 20px;
    }
    .about, .myself, .blogs {
      background: linear-gradient(to bottom, #000000, #2e0854);
      margin-bottom: 20px;
    }
    img.small-img {
      width: 100px;
      height: auto;
      border-radius: 10px;
      border: 2px solid purple;
    }
    .spotify, .games, .quiz, .calendar {
      background: #111;
      color: #eee;
      padding: 20px;
      margin-bottom: 20px;
    }
    .adios {
      background: linear-gradient(to bottom, #2e0854, #000000);
      text-align: center;
      padding: 30px;
    }
    .game-box, .quiz-box {
      background: #222;
      padding: 15px;
      margin: 10px 0;
      border: 2px solid purple;
      border-radius: 10px;
    }
    .hunt-box {
  margin-top: 40px;
  padding: 20px;
  background-color: #1a001a;
  border: 2px dashed violet;
  color: white;
  position: relative;
}

.hunt-item {
  width: 40px;
  position: absolute;
  cursor: pointer;
  display: none;
  z-index: 10;
}

#item-bone { top: 120px; left: 60px; }
#item-vial { top: 200px; left: 300px; }
#item-herb { top: 350px; left: 180px; }

.hunt-box ul li.found {
  text-decoration: line-through;
  color: lime;
}
#scareContainer {
  display: none;
  position: fixed;
  top: 0;
  left: 0;
  width: 100vw;
  height: 100vh;
  background: rgba(0, 0, 0, 0.9);
  z-index: 9999;
  justify-content: center;
  align-items: center;
}

#scareContainer img {
  max-width: 80%;
  max-height: 80%;
  box-shadow: 0 0 30px red;
  animation: pulse 0.5s infinite alternate;
}

@keyframes pulse {
  from {
    transform: scale(1);
  }
  to {
    transform: scale(1.05);
  }
} 
#scareContainer {
  display: none;
  position: fixed;
  top: 0; left: 0;
  width: 100vw; height: 100vh;
  background: rgba(0, 0, 0, 0.95);
  z-index: 9999;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  animation: shake 0.3s ease-in-out infinite;
}

#scareImage {
  max-width: 80%;
  max-height: 80%;
  animation: pulse 0.5s infinite alternate;
  z-index: 10001;
}

#bloodFlash {
  position: absolute;
  top: 0; left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  z-index: 10000;
  display: none;
  animation: flash 0.5s ease;
}

@keyframes pulse {
  from { transform: scale(1); }
  to { transform: scale(1.05); }
}

@keyframes shake {
  0% { transform: translate(1px, 1px) rotate(0deg); }
  10% { transform: translate(-1px, -2px) rotate(-1deg); }
  20% { transform: translate(-3px, 0px) rotate(1deg); }
  30% { transform: translate(3px, 2px) rotate(0deg); }
  40% { transform: translate(1px, -1px) rotate(1deg); }
  50% { transform: translate(-1px, 2px) rotate(-1deg); }
  60% { transform: translate(-3px, 1px) rotate(0deg); }
  70% { transform: translate(3px, 1px) rotate(-1deg); }
  80% { transform: translate(-1px, -1px) rotate(1deg); }
  90% { transform: translate(1px, 2px) rotate(0deg); }
  100% { transform: translate(1px, -2px) rotate(-1deg); }
}

@keyframes flash {
  0% { opacity: 0; }
  50% { opacity: 0.8; }
  100% { opacity: 0; }
}

/* 🕷️ Toggle button */
#spiderToggle {
  position: fixed;
  top: 20px;
  left: 20px;
  font-size: 32px;
  cursor: pointer;
  z-index: 1001;
  color: red;
  animation: pulse 2s infinite;
}

/* 🕸️ Spiderbar Styles */
#spiderbar {
  position: fixed;
  top: 0;
  left: -220px;
  width: 200px;
  height: 100%;
  background-color: #0a0015;
  padding-top: 60px;
  box-shadow: 4px 0 10px #800080;
  transition: left 0.5s ease;
  z-index: 1000;
}

#spiderbar a {
  display: block;
  color: violet;
  padding: 14px;
  font-size: 18px;
  text-decoration: none;
  font-family: 'Creepster', cursive;
  text-align: center;
  transition: 0.3s;
}

#spiderbar a:hover {
  background: black;
  color: white;
  text-shadow: 0 0 5px magenta;
  transform: scale(1.1);
}
#spiderbar {
  position: fixed;
  top: 0;
  left: -250px; /* changed from -220px to -250px */
  width: 220px;
  height: 100%;
  background-color: #0a0015;
  padding-top: 60px;
  box-shadow: 4px 0 10px #800080;
  transition: left 0.4s ease;
  z-index: 1000;
  overflow-x: hidden;
}
body {
  margin: 0;
  padding: 0;
  overflow-x: hidden; /* Hides the black scroll space */
  background-color: #000010; /* or your page background */
}
#spiderbar {
  position: fixed;
  top: 0;
  left: -250px; /* fully off-screen */
  width: 220px;
  height: 100%;
  background-color: #0a0015;
  padding-top: 60px;
  box-shadow: 4px 0 10px #800080;
  transition: left 0.5s ease;
  z-index: 1000;
}
/* Show menu when active */
#spiderbar.active {
  left: 0;
}

/* Creepy pulse animation */
@keyframes pulse {
  0% { transform: scale(1); }
  50% { transform: scale(1.2); color: #ff00ff; }
  100% { transform: scale(1); }
}

body {
  margin-left: 180px; /* leaves room for vertical nav */
}
.echos-section {
  background-color: #0d0017;
  padding: 40px 20px;
  color: lavender;
  border-top: 2px solid violet;
  border-bottom: 2px solid violet;
}
.echos-section {
  background-color: #0d0017;
  padding: 40px 20px;
  color: lavender;
  border-top: 2px solid violet;
  border-bottom: 2px solid violet;
}

.echo-entry {
  margin-bottom: 30px;
  background-color: #1c002a;
  padding: 15px;
  border-left: 4px solid magenta;
  box-shadow: 0 0 10px rgba(255, 0, 255, 0.2);
}

.echo-entry h3 {
  font-family: 'Creepster', cursive;
  color: violet;
  margin-bottom: 10px;
  text-shadow: 0 0 3px magenta;
}
.echo-form {
  margin-top: 40px;
  background-color: #14001a;
  padding: 20px;
  border: 2px dashed violet;
  color: white;
  box-shadow: 0 0 10px rgba(200, 0, 255, 0.3);
}

.echo-form textarea {
  width: 100%;
  height: 100px;
  background-color: #1d002a;
  border: 1px solid violet;
  color: lavender;
  padding: 10px;
  font-family: 'Georgia', serif;
  margin-bottom: 10px;
}

.echo-form button {
  background-color: violet;
  color: black;
  font-weight: bold;
  border: none;
  padding: 8px 16px;
  cursor: pointer;
  transition: all 0.3s ease;
}

.echo-form button:hover {
  background-color: magenta;
  color: white;
  text-shadow: 0 0 5px black;
}

.user-echos {
  margin-top: 30px;
  background-color: #100014;
  padding: 15px;
  border-top: 1px solid magenta;
}

.user-echos .entry {
  background-color: #1c002a;
  margin-top: 10px;
  padding: 10px;
  color: lavender;
  border-left: 4px solid violet;
  font-style: italic;
}
body {
  margin-left: 180px; /* same as your sidebar width */
  background-color: black;
  color: white;
  font-family: 'Georgia', serif;
}
@media (max-width: 600px) {
  body {
    margin-left: 0;
  }
  .vertical-nav {uu
    position: relative;
    width: 100%;
    height: auto;
  }
}
/* Menu Toggle Button */
#menuToggle {
  position: fixed;
  top: 20px;
  left: 20px;
  background: #111;
  color: #fff;
  padding: 10px 15px;
  cursor: pointer;
  z-index: 1000;
  border: 1px solid #444;
  border-radius: 5px;
  font-family: 'Creepster', cursive; /* Optional spooky font */
}

/* Hidden Menu */
#spookyMenu {
  position: fixed;
  top: 0;
  left: -250px;
  width: 200px;
  height: 100%;
  background-color: #1a1a1a;
  color: white;
  padding-top: 60px;
  transition: left 0.3s ease;
  z-index: 999;
}

/* Menu Items */
#spookyMenu ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

#spookyMenu ul li {
  padding: 15px;
  text-align: left;
}

#spookyMenu ul li a {
  color: #ffcc00;
  text-decoration: none;
  font-weight: bold;
  transition: color 0.2s;
}

#spookyMenu ul li a:hover {
  color: #fff;
}

/* Active class to show menu */
#spookyMenu.active {
  left: 0;
}
body {
  margin: 0;
  padding: 0;
  overflow-x: hidden; /* This ensures no horizontal scroll from hidden elements */
}
/* Toggle Button (Top Right) */
#menuToggle {
  position: fixed;
  top: 20px;
  right: 20px;
  background: #111;
  color: #fff;
  padding: 10px 15px;
  cursor: pointer;
  z-index: 1000;
  border: 1px solid #444;
  border-radius: 5px;
}

/* Right Slide Menu */
#spookyMenu {
  position: fixed;
  top: 0;
  right: -250px; /* hidden by default */
  width: 200px;
  height: 100%;
  background-color: #1a1a1a;
  color: white;
  padding-top: 60px;
  transition: right 0.3s ease;
  z-index: 999;
}

/* Show when active */
#spookyMenu.active {
  right: 0;
}

/* Menu items */
#spookyMenu ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

#spookyMenu ul li {
  padding: 15px;
}

#spookyMenu ul li a {
  color: #ffcc00;
  text-decoration: none;
  font-weight: bold;
  transition: color 0.2s ease;
}

#spookyMenu ul li a:hover {
  color: #fff;
}
/* Reset default list styles */
.main-navbar ul {
  list-style: none;
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: center;
  background-color: #000; /* spooky black */
  border-bottom: 1px solid #444;
  overflow-x: auto;
}

.main-navbar li {
  margin: 0;
}

.main-navbar a {
  display: block;
  padding: 15px 20px;
  text-decoration: none;
  color: #ffcc00;
  font-weight: bold;
  transition: background 0.2s, color 0.2s;
  white-space: nowrap;
}

.main-navbar a:hover {
  background-color: #222;
  color: white;
}
body {
  margin: 0;
  padding: 0;
  overflow-x: hidden;
}
.echo-card {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: #240031; /* your purple-dark theme */
  padding: 10px;
  border-radius: 12px;
  box-shadow: 0 0 8px #ff00ff;
  margin-bottom: 20px;
}

.echo-text {
  flex: 1;
  color: white;
  font-family: 'Cursive', serif;
}

.echo-img {
  width: 60px;
  height: auto;
  margin-left: 10px;
  border-radius: 8px;
}
.echo-card {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: #240031; /* your dark purple background */
  padding: 15px;
  border-radius: 16px;
  box-shadow: 0 0 12px #ff4fff;
  margin-bottom: 24px;
}
.echo-img {
  width: 120px;
  height: auto;
  max-width: 100%;
  border: 3px solid #ff99ff; /* Cute pink border */
  border-radius: 12px;
  box-shadow: 0 0 12px #ff99ff;
  object-fit: cover;
  display: block;
}
.echo-card {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap; /* ✅ Helps on smaller screens */
  gap: 15px;
}
@media screen and (max-width: 600px) {
  .echo-card {
    flex-direction: column;
    align-items: flex-start;
  }

  .echo-img {
    margin-top: 10px;
    width: 100px;
  }
}

.chromaverse-invite {
  margin-top: 20px; /* You can increase this to move it lower */
    }
</style>
</head>
<body><nav class="main-navbar">
  <ul>
    <li><a href="#home">🏠 Home</a></li>
    <li><a href="#about">📜 About</a></li>
    <li><a href="#myself">🧙‍♀️ Myself</a></li>
    <li><a href="#blogs">📚 Blogs</a></li>
    <li><a href="#games">🎮 Games</a></li>
    <li><a href="#playlist">🎵 Playlist</a></li>
    <li><a href="#adios">🌙 Adios</a></li>
  </ul>
</nav>
    <section id="home">
    <h2>Welcome to the Realm 🌒</h2>
    <p>Step into a space of magic, mystery, and fun. Welcome to my ghosty-cool web realm!</p>
  </section>  <section id="about" class="about">
    <h2>About Me</h2>
    <img src="file_0000000094d461f5a206b05a4e4ec2ed.png" alt="About image" class="small-img" />
    <!-- 🕷️ Toggle Button -->
  

<p>I'm<strong>Kamakshi</strong>, your local gaming witch coder ✨. I build magic through code, poems, and pain. This place is all me — haunting, healing, and hella fun.</p>
   <div class="main-content"> <section id="myself" class="myself">
    <h2>This Witchy</h2>
    <img src="5A6ABF91B5E13A4E907FE5B2CDCA7C31F748AD45" alt="Myself image" class="small-img" />
    <p>Hi there! I'm Kamakshi and this is my first time creating a website where I blog and maybe live. About myself I'm 18 and I'm very much interested in coding and doing nothing but also a little bit of magic. I love making friends, and in person I maybe an extrovert but I'm not much confident if you ask me but that's ok. That's how life works right!?. I might not be perfect and neither is this website but I hope y'all like it 😄. Thanks for being here. Toodles!</p>
  </section> </div><section id="blogs" class="blogs">
    <h2>Blogs</h2>
    <h3>Blog 1: 23/06/2025</h3>
    <p>Nothing to post yet...sorry </p>
    <h3>Blog 2: 24/06/2025</h3>
    <p> a little more wait for some cool blogs...</p>
