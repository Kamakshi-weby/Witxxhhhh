
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
        
          <script>
window.onload = function () {
  // ✅ TIC TAC TOE
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

  // ✅ MEMORY MATCH
  const emojis = ['👻','🕸️','🎃','🧛','🧙‍♀️','👽','👻','🕸️','🎃','🧛','🧙‍♀️','👽'];
  const shuffle = [...emojis].sort(() => 0.5 - Math.random());
  const memoryBoard = document.getElementById('memoryBoard');
  let flipped = [];
  if (memoryBoard) {
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
  }

  // ✅ SIMON SAYS
  const simonButtons = document.querySelectorAll('.simon-btn');
  let simonSequence = [];
  let userSequence = [];

  function flash(btn) {
    btn.style.opacity = '0.5';
    setTimeout(() => btn.style.opacity = '1', 300);
  }

  function playSimon() {
    const random = simonButtons[Math.floor(Math.random() * simonButtons.length)];
    simonSequence.push(random);
    userSequence = [];
    simonSequence.forEach((btn, i) => {
      setTimeout(() => flash(btn), i * 600);
    });
  }

  simonButtons.forEach(btn => {
    btn.addEventListener('click', () => {
      flash(btn);
      userSequence.push(btn);
      const index = userSequence.length - 1;
      if (userSequence[index] !== simonSequence[index]) {
        alert('Wrong! Game Over. Try again.');
        simonSequence = [];
        userSequence = [];
        playSimon();
      } else if (userSequence.length === simonSequence.length) {
        setTimeout(playSimon, 1000);
      }
    });
  });

  if (simonButtons.length > 0) {
    playSimon();
  }

  // ✅ BOLLYWOOD TRIVIA
  const triviaContainer = document.querySelector('.trivia-board');
  const questions = [
    { q: 'Who played the role of Rancho in 3 Idiots?', a: 'Aamir Khan' },
    { q: 'Which movie has the iconic song \"Tujh Mein Rab Dikhta Hai\"?', a: 'Rab Ne Bana Di Jodi' },
    { q: 'Who directed \"Dilwale Dulhania Le Jayenge\"?', a: 'Aditya Chopra' },
    { q: 'Name the movie with the dialogue \"Mogambo Khush Hua\".', a: 'Mr. India' },
  { q: 'Who is the King of Bollywood?', o: ['Salman', 'SRK', 'Aamir', 'Ranbir'], a: 1 },
  { q: 'Which movie won Filmfare 2023?', o: ['RRR', 'Pathaan', 'Jawan', 'Gully Boy'], a: 2 },
  { q: 'Which actress is called "Desi Girl"?', o: ['Katrina', 'Priyanka', 'Alia', 'Deepika'], a: 1 },
  { q: 'Who played the role of Munna Bhai?', o: ['Aamir Khan', 'Salman Khan', 'Sanjay Dutt', 'Shah Rukh Khan'], a: 2 },
  { q: 'Which movie has the song "Kal Ho Naa Ho"?', o: ['Veer-Zaara', 'Kal Ho Naa Ho', 'Kabhi Khushi Kabhie Gham', 'Dil Se'], a: 1 },
  { q: 'Which actor starred in "Dangal"?', o: ['Salman Khan', 'Akshay Kumar', 'Aamir Khan', 'Ajay Devgn'], a: 2 },
  { q: 'Who directed "Kabir Singh"?', o: ['Sandeep Vanga', 'Karan Johar', 'Rohit Shetty', 'Zoya Akhtar'], a: 0 },
  { q: 'What is the real name of Govinda?', o: ['Ravi Kapoor', 'Govind Ahuja', 'Sunil Shetty', 'Rakesh Roshan'], a: 1 },
  { q: 'Which film is based on hockey?', o: ['Chak De India', 'Dangal', 'Lagaan', 'Mary Kom'], a: 0 },
  { q: 'Who played Bajirao in "Bajirao Mastani"?', o: ['Ranbir Kapoor', 'Hrithik Roshan', 'Ranveer Singh', 'Shahid Kapoor'], a: 2 },
  { q: 'In which year did "Sholay" release?', o: ['1975', '1980', '1982', '1970'], a: 0 },
  { q: 'What is Katrina Kaif\'s debut movie?', o: ['Boom', 'Namastey London', 'Maine Pyaar Kyun Kiya', 'Zindagi Na Milegi Dobara'], a: 0 },
  { q: 'Which movie has the character Geet?', o: ['Barfi!', 'Jab We Met', 'Queen', 'Tamasha'], a: 1 },
  { q: 'Who composed the music for "Dil Se"?', o: ['Pritam', 'Shankar-Ehsaan-Loy', 'A.R. Rahman', 'Vishal-Shekhar'], a: 2 },
  { q: 'Who is called Mr. Perfectionist in Bollywood?', o: ['Shah Rukh Khan', 'Hrithik Roshan', 'Aamir Khan', 'Saif Ali Khan'], a: 2 },
  { q: 'Which movie features the song "Tujh Mein Rab Dikhta Hai"?', o: ['Rab Ne Bana Di Jodi', 'Dilwale', 'Jab Tak Hai Jaan', 'Fan'], a: 0 },
  { q: 'What is the profession of Shahid in "Kabir Singh"?', o: ['Lawyer', 'Doctor', 'Engineer', 'Singer'], a: 1 },
  { q: 'Which actor was in "Andaz Apna Apna"?', o: ['Govinda', 'Aamir & Salman', 'Ajay Devgn', 'Saif & SRK'], a: 1 },
  { q: 'Who played the lead in "Raazi"?', o: ['Deepika', 'Kangana', 'Alia Bhatt', 'Kareena'], a: 2 },
  { q: 'Which movie is India\'s official entry to Oscars 2022?', o: ['RRR', 'Chhello Show', 'The Kashmir Files', 'Rocketry'], a: 1 },
  { q: 'What is the highest-grossing Indian film ever?', o: ['PK', 'Dangal', 'Baahubali 2', 'Pathaan'], a: 2 },
  { q: 'Who played the character of Kabir in "War"?', o: ['Tiger Shroff', 'Hrithik Roshan', 'Ranveer Singh', 'Shahid Kapoor'], a: 1 },
  { q: 'Which film was based on surgical strikes?', o: ['Uri', 'Shershaah', 'Raazi', 'Attack'], a: 0 },
  { q: 'Which actor is known for his dance?', o: ['Nawazuddin', 'Hrithik Roshan', 'Aamir Khan', 'Pankaj Tripathi'], a: 1 },
  { q: 'Which actress debuted in "Student of the Year"?', o: ['Kriti Sanon', 'Kiara Advani', 'Alia Bhatt', 'Sara Ali Khan'], a: 2 },
  { q: 'What role did Akshay play in "Toilet"?', o: ['Villain', 'Reporter', 'Social Worker', 'Husband'], a: 3 },
  { q: 'Which movie stars SRK & Kajol in Europe?', o: ['Dilwale', 'DDLJ', 'Kabhi Khushi...', 'My Name is Khan'], a: 1 },
  { q: 'Who is the director of "RRR"?', o: ['Rajkumar Hirani', 'Rohit Shetty', 'SS Rajamouli', 'Zoya Akhtar'], a: 2 },
  { q: 'What does "PK" stand for in the movie?', o: ['Pakistani Kid', 'Peekay (Drunk)', 'Pintu Kumar', 'None'], a: 1 },
  { q: 'Which movie has the line: "How\'s the Josh?"', o: ['Shershaah', 'Bhuj', 'Uri', 'Kesari'], a: 2 }
];
  

  let triviaIndex = 0;

  function showTrivia() {
    if (!triviaContainer) return;
    if (triviaIndex >= questions.length) {
      triviaContainer.innerHTML = '<p>✨ You completed the quiz! ✨</p>';
      return;
    }

    const qObj = questions[triviaIndex];
    const qEl = document.createElement('div');
    qEl.className = 'trivia-q';
    qEl.innerText = qObj.q;

    const input = document.createElement('input');
    input.placeholder = 'Your answer...';
    input.style.margin = '10px';

    const btn = document.createElement('button');
    btn.innerText = 'Submit';
    btn.onclick = () => {
      if (input.value.trim().toLowerCase() === qObj.a.toLowerCase()) {
        alert('Correct!');
      } else {
        alert('Oops! Right answer: ' + qObj.a);
      }
      triviaIndex++;
      showTrivia();
    };

    triviaContainer.innerHTML = '';
    triviaContainer.appendChild(qEl);
    triviaContainer.appendChild(input);
    triviaContainer.appendChild(btn);
  }

  showTrivia();
};
</script></body>

