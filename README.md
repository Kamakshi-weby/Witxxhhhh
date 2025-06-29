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
    <img src="IMG-20250625-WA0000.jpg" alt="About image" class="small-img" />
    <!-- 🕷️ Toggle Button -->
  

<p>I'm<strong>Kamakshi</strong>, your local gaming witch coder ✨. I build magic through code, poems, and pain. This place is all me — haunting, healing, and hella fun.</p>
   <div class="main-content"> <section id="myself" class="myself">
    <h2>This Witchy</h2>
    <img src="IMG-20250625-WA0001.jpg" alt="Myself image" class="small-img" />
    <p>Hi there! I'm Kamakshi and this is my first time creating a website where I blog and maybe live. About myself I'm 18 and I'm very much interested in coding and doing nothing but also a little bit of magic. I love making friends, and in person I maybe an extrovert but I'm not much confident if you ask me but that's ok. That's how life works right!?. I might not be perfect and neither is this website but I hope y'all like it 😄. Thanks for being here. Toodles!</p>
  </section> </div><section id="blogs" class="blogs">
    <h2>Blogs</h2>
    <h3>Blog 1: 23/06/2025</h3>
    <p>Nothing to post yet...sorry </p>
    <h3>Blog 2: 24/06/2025</h3>
    <p> a little more wait for some cool blogs...</p>
    <section id="echos" class="echos-section">
  <h2 class="spooky-heading">🫧 Echos from Beyond</h2>
  <article class="echo-entry">
    <div class="echo-card">
  <div class="echo-text">
    <h3>“MY MOM”</h3>
    <p>She has truly been the most precious gift I’ve ever received from God. And as I’ve grown, I’ve come to realize something that words can barely capture — no one, absolutely no one, can love me the way she does.

She’s in her 50s now, a brilliant and respected Advocate by profession. But to me, she’s more than just a lawyer — she’s my inspiration, my definition of strength, and the woman I aspire to be like every single day.

Not because she is my mother-but it’s the way she carries herself, her grace under pressure, and her ability to balance power with gentleness that leaves me in awe.

She wakes up early, gets everything at home running, and then drives off to her workplace to manage things there. She handles everything so smooth and makes difficult things so easy and still — after a long, exhausting day — she returns home and cooks the most comforting, delicious food you could ever imagine.

But more than all of that… it’s her love. Her endless, unconditional love.
The kind that heals me.
The kind that protects me.
The kind that no one else in this world can match.

She’s not just my mom.
She’s my strength.
She’s my soft place to fall.
She’s home.

I love you so much, Mumma — more than words could ever explain.
And every day, I thank the universe that you’re mine.</p>
  </div>
  <img src="IMG-20250629-WA0000.jpg" alt="Spooky spirit" class="echo-img">
</div>

  
<div id="echo-submission" class="echo-form">
  <h3>🫧 Whisper Your Own Echo...</h3>
  <textarea id="userStory" placeholder="The spirit moved, and I heard it say..."></textarea>
  <button onclick="submitEcho()">Submit</button>
</div>

<div id="userEchos" class="user-echos">
  <h3>🔮 Other Echos</h3>
</div>

 <section id="mirror" class="spooky-mirror">
  <h2 class="spooky-heading">🪞 Haunted Mirror</h2>
  <p id="mirrorMessage">Peer into the mirror... what do you seek?</p>
  <button onclick="talkToSpirit()">Speak to the Spirit</button>
  </section>
  <section id="quiz" class="quiz">
    <h2>🔮 What Kind of Witch Are You?</h2>
    <div class="quiz-box">
      <p><strong>Q1:</strong> What time of day or place calls to your soul?</p>
<input type="radio" name="q1" value="forest" /> A misty forest at dawn 🌲<br />
<input type="radio" name="q1" value="storm" /> Thunderstorms in the evening 🌩️<br />
<input type="radio" name="q1" value="shadow" /> Midnight shadows 🌑<br />
<input type="radio" name="q1" value="fire" /> Blazing sunlight and fire rituals 🔥<br />
<input type="radio" name="q1" value="ice" /> Snow-covered silence ❄️<br />
<input type="radio" name="q1" value="sea" /> Waves crashing at night 🌊<br />
<input type="radio" name="q1" value="bone" /> Dusty bones and forgotten whispers 🦴<br />
<input type="radio" name="q1" value="cosmic" /> Stargazing from your window 💫<br />
      <button onclick="getWitchResult()">Reveal My Witch Type</button>
      <p id="witchResult"></p>
    </div>
  </section> 
  <div id="secretTrigger" style="text-align: center; margin: 60px 0;">
  <p style="color: #999;">
    ⚠️ <span onclick="triggerScare()" style="cursor: pointer; text-decoration: underline;">Do not click this</span>
  </p>
  <div id="scareContainer">
    <img
      id="scareImage"
      src="IMG-20250629-WA0001.jpg"
      alt="Scary Face"
    />

  </div>
  </div>
  <section id="games" class="games">
    <h2>🕹️ Witchy Games</h2>
    <div class="game-box">
      <h3>🃏 Tarot Card Generator</h3>
      <button onclick="drawTarot()">Draw a Card</button>
      <p id="tarotResult"></p>
    </div>
    <div class="game-box">
      <h3>✨ Spell Generator</h3>
      <button onclick="generateSpell()">Cast Spell</button>
      <p id="spellResult"></p>
    </div>
    <div class="game-box">
      <h3>🧪 Potion Maker</h3>
      <button onclick="makePotion()">Brew Potion</button>
      <p id="potionResult"></p>
    </div>
    <div class="game-box">
      <h3>🔍 Hidden Object Game</h3>
      <p>Coming soon! (interactive room with items)</p>
    </div>
  </section>  <section id="calendar" class="calendar">
    <h2>🌕 Spooky Calendar</h2>
    <ul>
      <li>🌝 Full Moon – 21 July 2025</li>
      <li>🔮 Mercury Retrograde – 5 Aug to 28 Aug 2025</li>
      <li>🌑 New Moon – 4 August 2025</li>
      <li>🕯️ Witch's Market – 13 July 2025</li>
<li>💀 Ancestor Night – 31 October 2025</li>
<li>🧛 Blood Moon Eclipse – 8 November 2025</li>
<li>🎃 Samhain Festival – 31 October 2025</li>
<li>📿 Dark Spirit Portal Opening – 21 December 2025</li>
<li>🔔 Hex Hour – Every Friday the 13th</li>
    </ul>
  </section> 
  <section id="horoscope" class="horoscope-section">
  <h2 class="spooky-heading">🧿 Your Spooky Horoscope</h2>
  <label for="sign">Choose your sign:</label>
  <select id="sign">
    <option value="">--Select--</option>
    <option value="aries">♈ Aries</option>
    <option value="taurus">♉ Taurus</option>
    <option value="gemini">♊ Gemini</option>
    <option value="cancer">♋ Cancer</option>
    <option value="leo">♌ Leo</option>
    <option value="virgo">♍ Virgo</option>
    <option value="libra">♎ Libra</option>
    <option value="scorpio">♏ Scorpio</option>
    <option value="sagittarius">♐ Sagittarius</option>
    <option value="capricorn">♑ Capricorn</option>
    <option value="aquarius">♒ Aquarius</option>
    <option value="pisces">♓ Pisces</option>
  </select>
  <button onclick="getSpookyHoroscope()">Reveal My Fate</button>
  <p id="spookyResult" style="margin-top: 20px; color: violet; font-style: italic;"></p>
  </section>
  <section id="playlist" class="spotify">
    <h2>🔮 Some Creepy Vibes</h2>
    <p><em>🧪 This playlist was brewed under a blood moon with ghostly hands and glittering shadows. It’s not just music — it’s a spell. Press play and vanish. 💫👻 
    <iframe style="border-radius:12px" src="https://open.spotify.com/embed/playlist/1Pg4aIDGiFGKhgAfwDa3b3?utm_source=generator" width="100%" height="152" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
  
  <footer id="adios" class="adios"><footer style="text-align:center; padding: 50px 20px; background: linear-gradient(90deg, #0b0019, #1e0033); color: violet; font-family: 'Creepster', cursive; font-size: 22px; letter-spacing: 2px; text-shadow: 2px 2px 6px purple;">
 <h2>🌙 Adios</h2>
    <p>Thank you for exploring my little spooky world! This was just a witchy beginning — more chaos, more spells, and more stories will brew soon. Stay weird, stay magical. ✨👾💀<br />
    Adios, fellow night crawlers!</p>
  </footer>  <script>
    function getWitchResult() {
      const val = document.querySelector('input[name="q1"]:checked');
      if (!val) return alert("Choose an answer!");
      const type = val.value;
      const types = {
  forest: "🌲 You're a Forest Witch! You draw power from nature and earth spirits.",
  storm: "🌩️ You're a Storm Witch! You thrive in chaos, change, and lightning strikes.",
  shadow: "🌑 You're a Shadow Witch! You're mysterious, deep, and see the unseen.",
  fire: "🔥 You're a Fire Witch! Passionate, fierce, and born to lead.",
  ice: "❄️ You're an Ice Witch! Calm, elegant, and unshakably in control.",
  sea: "🌊 You're a Sea Witch! Emotions, tides, and the unknown call to you.",
  bone: "🦴 You're a Bone Witch! Wise, ancient, connected to the spirit realm.",
  cosmic: "💫 You're a Cosmic Witch! You read stars and dream with galaxies."
};
      document.getElementById("witchResult").innerText = types[type];
    }

    function drawTarot() {
      const cards = ["The Moon", "The Tower", "The Lovers", "Death", "The Star"];
      const meanings = {
        "The Moon": "Confusion, illusion, dreams.",
        "The Tower": "Sudden change, upheaval.",
        "The Lovers": "Connection, choice, harmony.",
        "Death": "Endings, transformation, rebirth.",
        "The Star": "Hope, guidance, inspiration."
      };
      const pick = cards[Math.floor(Math.random() * cards.length)];
      document.getElementById("tarotResult").innerText = `${pick}: ${meanings[pick]}`;
    }

    function generateSpell() {
      const names = ["Binding Whispers", "Night Veil", "Crystal Echo", "Blood Pact"];
      const ingredients = ["raven feather", "moon water", "black salt", "phantom root"];
      const chants = ["Morva elthra senna!", "Zel nocht varun!", "Silven drak osh!"];
      const spell = names[Math.floor(Math.random() * names.length)];
      const ing = ingredients.sort(() => 0.5 - Math.random()).slice(0, 2).join(", ");
      const chant = chants[Math.floor(Math.random() * chants.length)];
      document.getElementById("spellResult").innerText = `${spell}\nIngredients: ${ing}\nIncantation: ${chant}`;
    }

    function makePotion() {
     const results = [
  "Potion of Eternal Confidence",
  "Love Elixir",
  "Invisibility Draught",
  "Truth Serum",
  "Witch's Brew of Misfortune",
  "Serpent's Tongue Serum",
  "Liquid Luck (Felix Felicis)",
  "Memory Mist",
  "Nightmare Nectar",
  "Dragon’s Breath Potion",
  "Potion of Shapeshifting",
  "Ghost Whisper Tonic",
  "Elixir of Time Freeze",
  "Poison of Eternal Sleep",
  "Soul Binding Vial",
  "Potion of Endless Night",
  "Spider Silk Serum",
  "Moonlight Elixir",
  "Goblin Gigglegoo",
  "Cauldron of Curses"
]; 
      document.getElementById("potionResult").innerText = `You brewed: ${results[Math.floor(Math.random() * results.length)]}`;
    }
  </script><script>
  function talkToSpirit() {
    const messages = [
      "You are not alone... the spirits walk with you.",
      "Your future is cloudy, but something stirs in the shadows.",
      "Beware the full moon... it brings more than light.",
      "A forgotten soul is watching. Are you ready to listen?",
      "Your power grows stronger, but so does the danger.",
      "You will soon meet someone... or something.",
      "The mirror sees all — even what you try to hide."
    ];
    const mirror = document.getElementById("mirrorMessage");
    const spirit = messages[Math.floor(Math.random() * messages.length)];
    mirror.innerText = `"${spirit}"`;
  }
</script>
<script>
  function triggerScare() {
    const scare = document.getElementById("scareContainer");
    const blood = document.getElementById("bloodFlash");
    scare.style.display = "flex";
    blood.style.display = "block";

    const scream = new Audio("https://www.myinstants.com/media/sounds/wilhelm-scream.mp3");
    scream.play();

    setTimeout(() => {
      scare.style.display = "none";
      blood.style.display = "none";
    }, 3000);
  }
</script>
<script>
  const horoscopes = {
    aries: [
      "Aries, your flame burns bright tonight... but beware who follows its light.",
      "Your courage may attract spirits. Burn sage at dusk.",
      "A shadow has its eye on you. Be bold, but not careless."
    ],
    taurus: [
      "Taurus, something old is clinging to your aura. Cleanse with earth and salt.",
      "Your stubbornness will summon ancient energy. Are you ready to deal with it?",
      "A creature walks where you once stood. It remembers you."
    ],
    gemini: [
      "Two faces, two paths. One leads to light, the other to screams.",
      "Speak less today. The spirits are listening.",
      "Your reflection may answer before you do. Avoid mirrors."
    ],
    cancer: [
      "The moon is whispering to you. Listen closely, but do not answer.",
      "Your feelings summon more than just memories tonight.",
      "Something watery wants to drag you under — emotionally or otherwise."
    ],
    leo: [
      "You’re glowing... which means dark things are watching.",
      "Pride may attract a challenge. A ghostly one.",
      "Don’t roar too loud. It may wake what sleeps below."
    ],
    virgo: [
      "You notice the patterns... but some were never meant to be seen.",
      "Dust your corners. Something’s hiding behind the perfection.",
      "Your logic won’t help when magic slips through the cracks."
    ],
    libra: [
      "Balance is breaking. Tip too far, and you’ll see the veil tear.",
      "You’ll be haunted by a choice. But which one?",
      "Mirror magic surrounds you — don’t stare too long."
    ],
    scorpio: [
      "Death isn’t the end for you today... it’s a beginning.",
      "A secret you’ve buried is clawing its way out.",
      "Your energy is magnetic — even to the dead."
    ],
    sagittarius: [
      "Wander far, but don’t follow the voices.",
      "You’ll find something lost. It may not want to be found.",
      "A new path opens. But it smells of ash and blood."
    ],
    capricorn: [
      "You're grounded — but something is trying to pull you down further.",
      "Be cautious with time. The past wants you back.",
      "Bones remember footsteps. Walk lighter today."
    ],
    aquarius: [
      "Your visions grow clearer, but they may not be your own.",
      "The air crackles. Something magical is reaching for you.",
      "Dreams will deliver a message tonight. Do not ignore it."
    ],
    pisces: [
      "You see beyond the veil — but something is staring back.",
      "Water remembers. Don’t let it carry away your truth.",
      "Tonight, your dreams become a door. Will you walk through?"
    ]
  };

  function getSpookyHoroscope() {
    const sign = document.getElementById("sign").value;
    const result = document.getElementById("spookyResult");

    if (!sign) {
      result.innerText = "Please choose your zodiac sign, child of the stars...";
      return;
    }

    const options = horoscopes[sign];
    const message = options[Math.floor(Math.random() * options.length)];
    result.innerText = message;
  }
</script>
<script>
  function submitEcho() {
    const story = document.getElementById("userStory").value.trim();
    const userEchos = document.getElementById("userEchos");

    if (story === "") {
      alert("The spirits demand a message...");
      return;
    }

    const entry = document.createElement("div");
    entry.className = "entry";
    entry.innerText = story;
    userEchos.appendChild(entry);

    document.getElementById("userStory").value = "";
  }
</script>
<script>
  const toggleBtn = document.getElementById("menuToggle");
  const menu = document.getElementById("spookyMenu");

  toggleBtn.addEventListener("click", () => {
    menu.classList.toggle("active");
  });
</script>
<p class="chromaverse-invite" style="margin-top: 20px;">
  Ready to leave the shadows behind? Step into the light of The Chromaverse.
</p>
<div style="text-align: center; margin-top: 3rem; margin-bottom: 3rem;">
  <a href="THE CHROMAVERSE.html">
    <button style="
      background: linear-gradient(to right, #ff00cc, #3333ff);
      border: none;
      padding: 14px 28px;
      font-size: 18px;
      color: white;
      border-radius: 12px;
      cursor: pointer;
      box-shadow: 0 0 15px #ff00cc;
      transition: transform 0.3s ease;
    " onmouseover="this.style.transform='scale(1.1)'" onmouseout="this.style.transform='scale(1)'">
       🎮Enter The Chromaverse🎮
    </button>
  </a>
</div>


