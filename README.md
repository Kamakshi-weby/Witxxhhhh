<!DOCTYPE html><html lang="en">
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
  </style>
</head>
<body>
  <audio autoplay loop>
    <source src="creepy-music.mp3" type="audio/mpeg" />
    Your browser does not support the audio element.
  </audio>  <nav>
    <a href="#home">Home</a>
    <a href="#about">About</a>
    <a href="#witchy">This Witchy</a>
    <a href="#blogs">Blogs</a>
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
  </section>  <section id="games">
    <h2>Games 🎮</h2>
    <div class="game-container">
      <div class="game-card">
        <h3>Tic Tac Toe</h3>
        <div class="tic-board" id="ticBoard">
          <div class="tic-cell"></div><div class="tic-cell"></div><div class="tic-cell"></div>
          <div class="tic-cell"></div><div class="tic-cell"></div><div class="tic-cell"></div>
          <div class="tic-cell"></div><div class="tic-cell"></div><div class="tic-cell"></div>
        </div>
      </div>
      <div class="game-card">
        <h3>Memory Match</h3>
        <div class="memory-board" id="memoryBoard"></div>
      </div>
      <div class="game-card">
        <h3>Simon Says</h3>
        <div class="simon-board">
          <div class="simon-btn" style="background:#a855f7">Purple</div>
          <div class="simon-btn" style="background:#f43f5e">Pink</div>
          <div class="simon-btn" style="background:#38bdf8">Blue</div>
          <div class="simon-btn" style="background:#34d399">Green</div>
        </div>
      </div>
      <div class="game-card">
        <h3>Bollywood Trivia</h3>
        <div class="trivia-board">
          <div class="trivia-q">Who played the role of Rancho in 3 Idiots?</div>
          <div class="trivia-q">Which movie has the iconic song "Tujh Mein Rab Dikhta Hai"?</div>
          <div class="trivia-q">Who directed "Dilwale Dulhania Le Jayenge"?</div>
          <div class="trivia-q">Name the movie with the dialogue "Mogambo Khush Hua".</div>
        </div>
      </div>
    </div>
  </section>  <section id="adios">
    <h2>Adios</h2>
    <p>Thanks for floating through my world. Come back soon... or I'll hex you 😈✨</p>
  </section>  <script>
    // Tic Tac Toe
    const cells = document.querySelectorAll('.tic-cell');
    let currentPlayer = 'X';
    cells.forEach(cell => {
      cell.addEventListener('click', () => {
        if (cell.textContent === '') {
          cell.textContent = currentPlayer;
          currentPlayer = currentPlayer === 'X' ? 'O' : 'X';
        }
      });
    });

    // Memory Match
    const emojis = ['👻','🕸️','🎃','🧛','🧙‍♀️','👽','👻','🕸️','🎃','🧛','🧙‍♀️','👽'];
    const shuffle = [...emojis].sort(() => 0.5 - Math.random());
    const memoryBoard = document.getElementById('memoryBoard');
    let flipped = [];
    shuffle.forEach((em, i) => {
      const card = document.createElement('div');
      card.className = 'memory-card';
      card.dataset.index = i;
      card.innerText = '🃏';
      card.onclick = () => {
        if (flipped.length < 2 && !card.classList.contains('matched')) {
          card.innerText = em;
          flipped.push({ el: card, val: em });
          if (flipped.length === 2) {
            if (flipped[0].val === flipped[1].val) {
              flipped[0].classList.add('matched');
              flipped[1].classList.add('matched');
              flipped = [];
            } else {
              setTimeout(() => {
                flipped[0].innerText = '🃏';
                flipped[1].innerText = '🃏';
                flipped = [];
              }, 800);
            }
          }
        }
      };
      memoryBoard.appendChild(card);
    });
  </script></body>
</html>
