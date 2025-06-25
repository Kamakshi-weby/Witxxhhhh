
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>THE LOST WEB</title>
  <style>
    body {
      margin: 0;
      font-family: 'Courier New', monospace;
      background: #0d0d0d;
      color: #e0e0e0;
    }
    nav {
      background: #1a1a1a;
      display: flex;
      justify-content: space-around;
      padding: 1em;
      position: sticky;
      top: 0;
      z-index: 1000;
      box-shadow: 0 0 15px #4b0082;
    }
    nav a {
      text-decoration: none;
      color: #f5f5f5;
      font-weight: bold;
      font-size: 1.1em;
      border-bottom: 2px solid transparent;
      transition: all 0.3s ease;
    }
    nav a:hover {
      color: #c084fc;
      border-bottom: 2px solid #c084fc;
    }
    <nav style="background: #111; padding: 1rem; display: flex; justify-content: center; gap: 2rem; position: sticky; top: 0; z-index: 1000; font-family: 'Creepster', cursive;">
  <a href="#home" style="color: #fff; text-decoration: none;">Home</a>
  <a href="#about" style="color: #fff; text-decoration: none;">About</a>
  <a href="#thiswitchy" style="color: #fff; text-decoration: none;">This Witchy</a>
  <a href="#blogs" style="color: #fff; text-decoration: none;">Blogs</a>
  <a href="#games" style="color: #fff; text-decoration: none;">Game</a>
  <a href="#adios" style="color: #fff; text-decoration: none;">Adios</a>
</nav>
    section {
      padding: 3em;
      border-radius: 15px;
      margin: 2em;
      box-shadow: inset 0 0 20px #111;
    }
    h2 {
      text-decoration: underline;
      color: #faf089;
      margin-bottom: 1em;
    }
    .highlight {
      color: #c084fc;
      background-color: #1f1f1f;
      padding: 0.3em 0.6em;
      border-radius: 5px;
    }
    img.small-img {
      width: 120px;
      height: auto;
      border-radius: 10px;
      margin: 1em 0;
      box-shadow: 0 0 10px #c084fc;
    }
    audio {
      display: none;
    }
    #home {
      background: linear-gradient(135deg, #1a1a1a, #262626);
    }
    #about {
      background: linear-gradient(135deg, #111827, #312e81);
    }
    #witchy {
      background: radial-gradient(circle at top left, #4b0082, #1e1b4b);
    }
    #blogs {
      background: linear-gradient(135deg, #2d2d2d, #000000);
    }
    #adios {
      background: linear-gradient(135deg, #111111, #4b006e);
    }
    .game-container {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 2em;
      margin-top: 2em;
    }
    .game-card {
      background: #222;
      border-radius: 12px;
      padding: 1em;
      text-align: center;
      box-shadow: 0 0 10px #6b21a8;
    }
    .game-card h3 {
      margin-bottom: 1em;
      color: #facc15;
    }
    .tic-board {
      display: grid;
      grid-template-columns: repeat(3, 60px);
      gap: 5px;
      justify-content: center;
    }
    .tic-cell {
      width: 60px;
      height: 60px;
      background: #0f172a;
      color: #facc15;
      border: 2px solid #4b0082;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.5em;
      font-weight: bold;
      cursor: pointer;
    }
    .memory-board, .simon-board, .trivia-board {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 10px;
    }
    .memory-card, .simon-btn, .trivia-q {
      background: #1f1b2e;
      padding: 1em;
      border-radius: 10px;
      color: #fff;
      box-shadow: 0 0 10px #8b5cf6;
      cursor: pointer;
    }
    .tic-cell {
  width: 80px;
  height: 80px;
  background-color: #000;
  color: #fff;
  font-size: 2rem;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
}
@import url('https://fonts.googleapis.com/css2?family=Creepster&display=swap');

.simon-btn {
  width: 100px;
  height: 100px;
  border-radius: 50%;
  box-shadow: 0 0 15px rgba(255, 255, 255, 0.2);
  cursor: pointer;
  transition: transform 0.1s, box-shadow 0.3s;
}

.simon-btn:active {
  transform: scale(0.95);
}

.simon-btn.glow {
  box-shadow: 0 0 25px white;
} .memory-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(60px, 1fr));
  max-width: 400px;
  margin: 2rem auto;
  gap: 10px;
  justify-items: center;
}

.memory-card {
  width: 60px;
  height: 60px;
  font-size: 1.5rem;
  display: flex;
  align-items: center;
  justify-content: center;
  background: #222;
  border-radius: 10px;
  color: white;
  cursor: pointer;
  box-shadow: 0 0 10px rgba(255,255,255,0.1);
  transition: all 0.2s ease;
}

.memory-card.matched {
  background: #4ade80;
  color: #111;
  cursor: default;
} </style>
</head>
<body> <audio autoplay loop>
  <source src="https://files.freemusicarchive.org/storage-freemusicarchive-org/music/no_curator/Myuu/The_Dark_Piano/Myuu_-_Ghost_Story.mp3" type="audio/mpeg">
</audio>
  <audio autoplay loop>
    <source src="creepy-music.mp3" type="audio/mpeg" />
    Your browser does not support the audio element.
  </audio>  <nav>
    <a href="#home">Home</a>
    <a href="#about">About</a>
    <a href="#witchy">This Witchy</a>
    <a href="#blogs">Blogs</a>
    <a href="#games">Games</a>
    <a href="#adios">Adios</a>
  </nav>  <section id="home">
    <h2>Welcome to the Realm 🌑</h2>
    <p>Step into a space of magic, mystery, and fun. Welcome to my ghosty-cool web realm!</p>
  </section>  <section id="about">
    <h2>About Me</h2>
    <img src="IMG-20250625-WA0000.jpg" alt="About Image" class="small-img" />
    <p>I’m <span class="highlight">Kamakshi</span>, your local gaming witch coder ✨. I build magic through code, poems, and games. This place is all me — haunting, healing, and hella fun.</p>
  </section>  <section id="witchy">
    <h2>This Witchy</h2>
    <img src="IMG-20250625-WA0001.jpg" alt="Witchy Image" class="small-img" />
    <p>Hi there! I'm Kamakshi and this is my first time creating a website where I blog and maybe live. About myself I'm 18 and I'm very much interested in gaming and doing nothing but also a little bit of coding. I love making friends, and in person I maybe an extrovert but I'm not much confident if you ask me but that's ok. That's how life works right!?. I might not be perfect and neither is this website but I hope y'all like it 🙂. Thanks for being here. Toddles!</p>
  </section>  <section id="blogs">
    <h2>Blogs</h2>
    <div class="blog-post">
      <p class="highlight">Blog 1: Its been a rough day and while blaming god for everything that's happening in my life I realised what the actual problem was and so here I'm discussing about THE REAL PROBLEM......with this poem-----> There's nothing more important to me than to be... to live...to feel but still the question echoes: is it truly necessary? Alone without love, no tender care to cradle my heart, seeking souls to halt this solitude, but shadows chase me still, like demons dancing in the dark of my restless mind. The world once sparkled bright in solitary glow, but now I'm encircled by strangers whose hearts are void, each glance a dagger, every word a wound, they bury my hope deeper than any weapon can wound. Innocence was my shroud, believing in binds of closeness, convincing myself it’s me, that I’m the flaw, but no, no, no— I’m just a marionette, strings pulled for their delight, yet I’ve grown; perhaps my heart remains a timid child, screaming silently, longing to cry, longing to be whole, and still I know, the mirror reflects the problem within me, cause yes! the problem is me.....

23/06/2025</p>
      <p class="highlight">Blog 2: I've been realising lately that everything I do will never be enough or maybe...... I'M NOT ACTUALLY DOING ENOUGH------>

Crying in silence, running through pain, Screaming inside like a voice in the rain. I've given my all, done more than I could, Yet still I'm unseen, misunderstood.

For those that I love, I’ve carried the weight, Faced every storm, surrendered to fate. But they look at me with eyes so cold, And I’m lost in stories I've already told.

Lost in the past, in shadows I flee, Trapped in a place I never wished to be. I wonder aloud—what do I desire? When did my soul lose its fire?

I’ve become someone I never planned, A stranger shaped by unseen hands. Not cruel, not heartless, not a foe— Just tired, just broken, moving slow.

They say I’m wrong, they think I’m weak, But maybe I’m just too soft to speak. Maybe my love was never enough To heal the cracks, to smooth the rough.

I’ve searched within, I’ve tried my best, But some battles don’t end in rest. Now I stand with nothing left to prove, Just the ache of all I couldn’t move.

So if I seem like I’m drifting apart, Know it’s not hate—it’s a heavy heart. I gave my all, yet here I stand, Still wondering if I was ever enough... in anyone’s hands......

24/06/2025</p>
    </div>
  </section>   
  <!-- 🎮 GAMES SECTION: Fully Functional Creepy Vibe Games --><section id="games" style="background: linear-gradient(135deg, #0a0a0a, #1f1f1f); color: #fff; padding: 3rem; font-family: 'Creepster', cursive;">
  <h2 style="text-align:center; font-size: 2.5rem; text-decoration: underline;">Creepy Cool Games</h2>  <!-- 🧠 MEMORY MATCH -->  <div id="memory-game" style="margin-top: 3rem;">
    <h3 style="text-align:center;">Memory Match 🃏</h3>
    <div id="memory-board" style="display: grid; grid-template-columns: repeat(4, 100px); gap: 10px; justify-content: center;"></div>
  </div>  <!-- ❌ TIC TAC TOE -->  <div id="tic-tac-toe" style="margin-top: 3rem;">
    <h3 style="text-align:center;">Tic Tac Toe ❌⭕</h3>
    <div style="display: grid; grid-template-columns: repeat(3, 100px); gap: 5px; justify-content: center;">
      <div class="cell"></div><div class="cell"></div><div class="cell"></div>
      <div class="cell"></div><div class="cell"></div><div class="cell"></div>
      <div class="cell"></div><div class="cell"></div><div class="cell"></div>
    </div>
    <p id="ttt-status" style="text-align:center; margin-top: 1rem;"></p>
  </div>  <!-- 🔊 SIMON SAYS -->  <div id="simon" style="margin-top: 3rem;">
    <h3 style="text-align:center;">Simon Says 🔮</h3>
    <div id="simon-board" style="display: flex; justify-content: center; gap: 1rem;">
      <button class="simon-btn" style="width: 100px; height: 100px; background: red;"></button>
      <button class="simon-btn" style="width: 100px; height: 100px; background: green;"></button>
      <button class="simon-btn" style="width: 100px; height: 100px; background: blue;"></button>
      <button class="simon-btn" style="width: 100px; height: 100px; background: yellow;"></button>
    </div>
    <button id="start-simon" style="margin: 1rem auto; display: block;">Start Game</button>
  </div>  <!-- 🎬 BOLLYWOOD TRIVIA -->  <div id="trivia" style="margin-top: 3rem;">
    <h3 style="text-align:center;">Bollywood Trivia 🎥</h3>
    <div id="trivia-question" style="text-align:center; margin-bottom: 1rem;"></div>
    <div id="trivia-options" style="text-align:center;"></div>
    <div id="trivia-result" style="text-align:center; margin-top: 1rem;"></div>
  </div>
</section><script>
// 🎮 Memory Match Game
const cards = ["👻", "🧛", "🕷️", "🧙", "🎃", "🧟", "🕸️", "🩸"];
let memoryDeck = [...cards, ...cards];
let flipped = [], lock = false;
function shuffle(arr) {
  for (let i = arr.length - 1; i > 0; i--) {
    const j = Math.floor(Math.random() * (i + 1));
    [arr[i], arr[j]] = [arr[j], arr[i]];
  }
  return arr;
}
function renderMemoryGame() {
  const board = document.getElementById("memory-board");
  board.innerHTML = "";
  shuffle(memoryDeck).forEach((icon, idx) => {
    const card = document.createElement("div");
    card.classList.add("memory-card");
    card.dataset.icon = icon;
    card.style.cssText = "background:#333; color:#333; width:100px; height:100px; display:flex; align-items:center; justify-content:center; font-size:2rem; cursor:pointer; border:1px solid #888; border-radius:10px; transition:all .3s";
    card.onclick = () => flipCard(card);
    board.appendChild(card);
  });
}
function flipCard(card) {
  if (lock || flipped.includes(card)) return;
  card.innerText = card.dataset.icon;
  card.style.color = "#fff";
  flipped.push(card);
  if (flipped.length === 2) {
    lock = true;
    setTimeout(() => {
      const [c1, c2] = flipped;
      if (c1.dataset.icon !== c2.dataset.icon) {
        c1.innerText = c2.innerText = "";
        c1.style.color = c2.style.color = "#333";
      }
      flipped = [];
      lock = false;
    }, 1000);
  }
}

// ❌ Tic Tac Toe
const cells = document.querySelectorAll(".cell");
let currentPlayer = "X";
let board = Array(9).fill("");
cells.forEach((cell, i) => {
  cell.style.cssText = "background:#222; color:#fff; font-size:2rem; display:flex; align-items:center; justify-content:center; height:100px; border:1px solid #444;";
  cell.addEventListener("click", () => {
    if (!board[i]) {
      board[i] = currentPlayer;
      cell.innerText = currentPlayer;
      currentPlayer = currentPlayer === "X" ? "O" : "X";
      document.getElementById("ttt-status").innerText = `Turn: ${currentPlayer}`;
    }
  });
});

// 🔮 Simon Says
let simonSequence = [], userSequence = [];
const simonBtns = document.querySelectorAll(".simon-btn");
document.getElementById("start-simon").onclick = () => {
  simonSequence = [];
  nextSimonColor();
};
function nextSimonColor() {
  const idx = Math.floor(Math.random() * simonBtns.length);
  simonSequence.push(idx);
  animateSimon();
  userSequence = [];
}
function animateSimon() {
  simonSequence.forEach((idx, i) => {
    setTimeout(() => {
      simonBtns[idx].style.opacity = 0.5;
      setTimeout(() => simonBtns[idx].style.opacity = 1, 300);
    }, i * 600);
  });
}
simonBtns.forEach((btn, idx) => {
  btn.onclick = () => {
    userSequence.push(idx);
    if (userSequence[userSequence.length - 1] !== simonSequence[userSequence.length - 1]) {
      alert("Wrong pattern! Try again.");
    } else if (userSequence.length === simonSequence.length) {
      setTimeout(nextSimonColor, 1000);
    }
  };
});

// 🎬 Bollywood Trivia
const triviaData = [
  { q: "Who played Munna Bhai in 'Munna Bhai M.B.B.S.'?", o: ["Salman Khan", "Aamir Khan", "Sanjay Dutt", "Shah Rukh Khan"], a: 2 },
  { q: "Which movie features the song 'Kal Ho Naa Ho'?", o: ["Kuch Kuch Hota Hai", "Kal Ho Naa Ho", "Kabhi Khushi Kabhie Gham", "Veer-Zaara"], a: 1 },
  { q: "'3 Idiots' was directed by?", o: ["Rajkumar Hirani", "Farhan Akhtar", "Karan Johar", "Anurag Kashyap"], a: 0 },
  { q: "Which movie had the character 'Geet' played by Kareena Kapoor?", o: ["Jab We Met", "Kabir Singh", "Chameli", "Bodyguard"], a: 0 },
  { q: "Who played the role of 'Rancho'?", o: ["Salman Khan", "Sharman Joshi", "R. Madhavan", "Aamir Khan"], a: 3 },
  { q: "Which is India's first Oscar-winning film?", o: ["Mother India", "Gandhi", "Lagaan", "Slumdog Millionaire"], a: 3 },
  { q: "Film with 'All is Well' song?", o: ["Student of the Year", "3 Idiots", "PK", "Dil Chahta Hai"], a: 1 },
  { q: "Which actress starred in 'Queen'?", o: ["Kangana Ranaut", "Alia Bhatt", "Deepika Padukone", "Anushka Sharma"], a: 0 },
  { q: "Movie with the line 'Don ko pakadna mushkil hi nahi...'?", o: ["Don", "Raees", "Sholay", "Dhoom"], a: 0 },
  { q: "Which movie features 'Chaiyya Chaiyya'?", o: ["Dil Se", "Swades", "Kabhi Alvida Naa Kehna", "Tanu Weds Manu"], a: 0 }
];
let triviaIndex = 0;
function showTrivia() {
  const q = triviaData[triviaIndex];
  document.getElementById("trivia-question").innerText = q.q;
  const opts = q.o.map((opt, i) => `<button onclick="checkTrivia(${i})">${opt}</button>`).join("<br>");
  document.getElementById("trivia-options").innerHTML = opts;
}
function checkTrivia(selected) {
  const correct = triviaData[triviaIndex].a;
  document.getElementById("trivia-result").innerText = selected === correct ? "Correct!" : "Oops, wrong answer.";
  triviaIndex = (triviaIndex + 1) % triviaData.length;
  setTimeout(() => {
    document.getElementById("trivia-result").innerText = "";
    showTrivia();
  }, 1500);
}

window.onload = () => {
  renderMemoryGame();
  showTrivia();
};</section>
</script></body>
