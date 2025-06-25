
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
  
  <!-- 👾 GAMES SECTION: Creepy & Cool --><section id="games" style="background: #0a0a0a; color: white; padding: 2rem;">
  <h1 style="text-align: center; font-family: 'Creepster', cursive; text-decoration: underline; font-size: 2rem;">Games 👻</h1>  <!-- 🧠 SIMON SAYS GAME -->  <section style="margin-top: 3rem;">
    <h2 style="text-align:center; text-decoration: underline; font-family: 'Creepster', cursive;">Simon Says</h2>
    <p id="score" style="text-align:center; font-size: 1.2rem;">Score: 0</p>
    <div id="simon-game" style="display: grid; grid-template-columns: repeat(2, 100px); gap: 1rem; justify-content: center;">
      <div class="simon-btn" id="green" style="background: #34d399;"></div>
      <div class="simon-btn" id="red" style="background: #f43f5e;"></div>
      <div class="simon-btn" id="yellow" style="background: #facc15;"></div>
      <div class="simon-btn" id="blue" style="background: #3b82f6;"></div>
    </div>
  </section>  <!-- 🎴 MEMORY MATCH GAME -->  <section style="margin-top: 3rem;">
    <h2 style="text-align:center; text-decoration: underline; font-family: 'Creepster', cursive;">Memory Match 👁️</h2>
    <div id="memoryBoard" class="memory-grid"></div>
  </section>  <!-- ♟️ TIC TAC TOE -->  <section style="margin-top: 3rem;">
    <h2 style="text-align:center; text-decoration: underline; font-family: 'Creepster', cursive;">Tic Tac Toe</h2>
    <div id="tic-tac-toe-board" style="display: grid; grid-template-columns: repeat(3, 80px); gap: 10px; justify-content: center; margin-top: 1rem;"></div>
  </section>  <!-- 🎬 BOLLYWOOD TRIVIA QUIZ -->  <section style="margin-top: 3rem;">
    <h2 style="text-align:center; text-decoration: underline; font-family: 'Creepster', cursive;">Bollywood Trivia 🎬</h2>
    <div id="quiz-container" style="max-width: 600px; margin: auto; background: #222; padding: 1rem; border-radius: 10px;">
      <p id="question" style="font-size: 1.2rem; font-weight: bold;"></p>
      <div id="options" style="display: flex; flex-direction: column; gap: 0.5rem; margin-top: 1rem;"></div>
      <button id="next-btn" style="margin-top: 1rem; padding: 0.5rem 1rem; background: #34d399; color: black; border: none; border-radius: 5px; cursor: pointer;">Next</button>
      <p id="score-quiz" style="margin-top: 1rem;"></p>
    </div>
  </section>
</section><!-- STYLE + SCRIPT CONTINUES BELOW --><style>
  @import url('https://fonts.googleapis.com/css2?family=Creepster&display=swap');
  /* Existing styles remain unchanged */
</style><script>
window.onload = function () {
  // Existing game scripts (Simon, Memory, Tic Tac Toe) remain unchanged

  // 🎬 Bollywood Trivia
  const trivia = [
    { q: "Who played the lead role in the movie '3 Idiots'?", o: ["Salman Khan", "Shahrukh Khan", "Aamir Khan", "Hrithik Roshan"], a: 2 },
    { q: "Which actress starred in 'Queen'?", o: ["Alia Bhatt", "Kangana Ranaut", "Deepika Padukone", "Kriti Sanon"], a: 1 },
    { q: "Who directed 'Dilwale Dulhania Le Jayenge'?", o: ["Karan Johar", "Aditya Chopra", "Yash Chopra", "Rohit Shetty"], a: 1 },
    { q: "Movie 'Lagaan' is based on what sport?", o: ["Hockey", "Football", "Kabaddi", "Cricket"], a: 3 },
    { q: "What is the name of the main character in 'PK'?", o: ["Rancho", "Chatur", "PK", "Jagdish"], a: 2 },
    { q: "Which movie features the dialogue 'Mogambo khush hua'?", o: ["Mr. India", "Sholay", "Karan Arjun", "Singham"], a: 0 },
    { q: "Who played 'Bajrangi' in 'Bajrangi Bhaijaan'?", o: ["Salman Khan", "Aamir Khan", "Akshay Kumar", "John Abraham"], a: 0 },
    { q: "Which film has the song 'Tum Hi Ho'?", o: ["Aashiqui 2", "Baaghi", "Half Girlfriend", "Kalank"], a: 0 },
    { q: "In which movie is the character 'Simran' found?", o: ["DDLJ", "Race 3", "Dabangg", "Ra.One"], a: 0 },
    { q: "Who is the villain in 'Dhoom 2'?", o: ["John Abraham", "Hrithik Roshan", "Aamir Khan", "Ranbir Kapoor"], a: 1 },
    { q: "Which movie has 'All Is Well' song?", o: ["Student of the Year", "3 Idiots", "Kal Ho Naa Ho", "Koi Mil Gaya"], a: 1 },
    { q: "Which actor starred in 'Barfi'?", o: ["Ranbir Kapoor", "Varun Dhawan", "Sidharth Malhotra", "Arjun Kapoor"], a: 0 },
    { q: "What is the name of the robot in 'Robot'?", o: ["Chitti", "Baba", "Robo", "Bittoo"], a: 0 },
    { q: "Which movie is based on India's 1983 cricket win?", o: ["MS Dhoni", "83", "Jersey", "Lagaan"], a: 1 },
    { q: "Who directed 'Kabhi Khushi Kabhie Gham'?", o: ["Karan Johar", "Farah Khan", "Rohit Shetty", "Zoya Akhtar"], a: 0 },
    { q: "Which movie features character 'Murad'?", o: ["Dangal", "Rock On", "Gully Boy", "Kaabil"], a: 2 },
    { q: "Which movie is about a blind pianist?", o: ["Andhadhun", "Kaabil", "Black", "Badla"], a: 0 },
    { q: "Which actor played Sanjay Dutt in 'Sanju'?", o: ["Ranbir Kapoor", "Ranveer Singh", "Shahid Kapoor", "Tiger Shroff"], a: 0 },
    { q: "Which movie features 'Zindagi Na Milegi Dobara'?", o: ["ZNMD", "Dil Chahta Hai", "Tamasha", "YJHD"], a: 0 },
    { q: "Which movie won Best Film at Filmfare 2023?", o: ["Drishyam 2", "Gangubai Kathiawadi", "RRR", "Bhediya"], a: 1 },
    { q: "Which film had 'Apna Time Aayega'?", o: ["Rockstar", "Gully Boy", "Raees", "Sultan"], a: 1 },
    { q: "Who played 'Geet' in 'Jab We Met'?", o: ["Kareena Kapoor", "Katrina Kaif", "Anushka Sharma", "Kriti Sanon"], a: 0 },
    { q: "Which movie was based on a mathematician's life?", o: ["Super 30", "Batla House", "Jersey", "Shakuntala Devi"], a: 0 },
    { q: "Which movie had the quote 'Baburao ka style hai'?", o: ["Phir Hera Pheri", "Welcome", "Golmaal", "Dhamaal"], a: 0 },
    { q: "In which movie did Salman Khan play twin roles?", o: ["Judwaa", "Kick", "Race 3", "Ready"], a: 0 }
  ];
  let currentQ = 0, scoreT = 0;
  const qEl = document.getElementById('question');
  const oEl = document.getElementById('options');
  const nextBtn = document.getElementById('next-btn');
  const scoreEl = document.getElementById('score-quiz');

  function loadQuestion() {
    qEl.textContent = trivia[currentQ].q;
    oEl.innerHTML = '';
    trivia[currentQ].o.forEach((opt, i) => {
      const btn = document.createElement('button');
      btn.textContent = opt;
      btn.style.background = '#444';
      btn.style.border = 'none';
      btn.style.color = 'white';
      btn.style.padding = '0.5rem';
      btn.style.borderRadius = '5px';
      btn.style.cursor = 'pointer';
      btn.onclick = () => {
        if (i === trivia[currentQ].a) {
          btn.style.background = '#22c55e';
          scoreT++;
        } else {
          btn.style.background = '#ef4444';
        }
        Array.from(oEl.children).forEach(child => child.disabled = true);
      };
      oEl.appendChild(btn);
    });
  }

  nextBtn.onclick = () => {
    if (currentQ < trivia.length - 1) {
      currentQ++;
      loadQuestion();
    } else {
      qEl.textContent = 'Quiz complete!';
      oEl.innerHTML = '';
      nextBtn.disabled = true;
      scoreEl.textContent = `Your Score: ${scoreT} / ${trivia.length}`;
    }
  };

  loadQuestion();
};
</script></body>
