
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>THE LOST WEB</title>
  <style>
    /* General Game Section Style */
#games {
  background-color: #000;
  color: #fff;
  padding: 2rem;
  font-family: 'Creepster', cursive;
}

/* Memory Game */
#memory-board {
  display: grid;
  grid-template-columns: repeat(4, 80px);
  gap: 10px;
  justify-content: center;
}
.memory-card {
  width: 80px;
  height: 80px;
  background-color: #444;
  border-radius: 10px;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 2rem;
  transition: transform 0.3s;
}
.memory-card.flip {
  background-color: #fff;
  transform: rotateY(180deg);
}

/* Tic Tac Toe */
#tic-tac-toe {
  display: grid;
  grid-template-columns: repeat(3, 80px);
  gap: 5px;
  justify-content: center;
}
.cell {
  width: 80px;
  height: 80px;
  background-color: #111;
  color: #fff;
  font-size: 2rem;
  text-align: center;
  line-height: 80px;
  border: 1px solid #fff;
  cursor: pointer;
}

/* Simon Says */
.simon-btn {
  width: 80px;
  height: 80px;
  border-radius: 50%;
  opacity: 0.7;
  box-shadow: 0 0 10px #fff;
  cursor: pointer;
}
.simon-btn.active {
  opacity: 1;
}

/* Quiz */
#quiz-container {
  margin-top: 1rem;
}
#quiz-options button {
  display: block;
  margin: 0.5rem auto;
  padding: 0.5rem 1rem;
}
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
} nav ul {
  list-style: none;
  display: flex;
  justify-content: center;
  gap: 20px;
}
nav a {
  color: #fff;
  text-decoration: none;
}
nav a:hover {
  text-decoration: underline;
}
</style>
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
<p class="highlight">"Temporary Us"
by Kamakshi

I always knew who I was
a shadow I never truly liked.
Maybe God had plans to heal me,
or maybe… to break me twice.

Then you came—
like sunlight through a stormed sky,
told me I was special,
held me like no one else tried.
Loved me loud,
until I believed maybe I was worth it,
even though deep down,
I knew… it was temporary.

I’ve always feared the end.
The leaving.
The silence after "forever" fades.
And now I see it
the slow turning of the tables,
the way your eyes no longer stay.

It’s not your fault.
I know.
But it still hurts to see you
look at me like the rest do
like I’m the villain in a story
I never meant to write.

I want to let you go,
to watch you fly,
to see you smile even if
that smile isn’t mine.
But the selfish ache in me
clings to the memory
of when we were us
not just me.

We promised, didn’t we?
To always be.
But even forever can be
just a fleeting dream.
And I thought knowing the end
would make it easier
but I was wrong.

Now I can’t eat,
can’t sleep,
can’t even swallow
without pain sinking deep.
Each time your lips
speak another girl's name,
I swear
it carves me like a flame.

I know I’m not enough.
Maybe I never was.
But you…
you deserved the stars,
and I was just a moment
on your map of Mars.

Still, those small, glowing moments—
even if they were just pixels and light—
were the best chapters of my life.

I’m sorry
for the chaos I brought.
I’m sorry
for being a storm you never sought.
But if love counts for anything—
I swear,
I loved you with all I had to give.

I just want to rewind
just once
to feel whole again.
But maybe this pain…
maybe it’s mine to bear.
Maybe I deserve it.

Maybe I was never meant
to be anything
but
Temporary.</p>
    </div>
  </section>   

<script>
// ==== Memory Game ====
const emojis = ['👻','🕸️','🧙‍♀️','👻','🕸️','🧙‍♀️','🧛','🧛'];
let memoryFlipped = [];
let memoryMatched = [];
const memoryBoard = document.getElementById('memory-board');
function shuffle(array) {
  return array.sort(() => Math.random() - 0.5);
}
function createMemoryBoard() {
  memoryBoard.innerHTML = '';
  shuffle(emojis).forEach((emoji, i) => {
    const card = document.createElement('div');
    card.classList.add('memory-card');
    card.dataset.index = i;
    card.dataset.emoji = emoji;
    card.addEventListener('click', flipMemoryCard);
    memoryBoard.appendChild(card);
  });
}
function flipMemoryCard() {
  if (this.classList.contains('flip') || memoryFlipped.length >= 2) return;
  this.classList.add('flip');
  this.innerText = this.dataset.emoji;
  memoryFlipped.push(this);
  if (memoryFlipped.length === 2) {
    const [first, second] = memoryFlipped;
    if (first.dataset.emoji === second.dataset.emoji) {
      memoryMatched.push(first, second);
      memoryFlipped = [];
    } else {
      setTimeout(() => {
        first.classList.remove('flip');
        second.classList.remove('flip');
        first.innerText = '';
        second.innerText = '';
        memoryFlipped = [];
      }, 1000);
    }
  }
}
createMemoryBoard();

// ==== Tic Tac Toe ====
const cells = document.querySelectorAll('.cell');
let currentPlayer = 'X';
document.getElementById('ttt-status').innerText = `Turn: ${currentPlayer}`;
cells.forEach(cell => {
  cell.addEventListener('click', () => {
    if (cell.innerText === '') {
      cell.innerText = currentPlayer;
      currentPlayer = currentPlayer === 'X' ? 'O' : 'X';
      document.getElementById('ttt-status').innerText = `Turn: ${currentPlayer}`;
    }
  });
});

// ==== Simon Says ====
let simonPattern = [];
let simonUser = [];
let simonColors = ['red', 'green', 'blue', 'yellow'];
function flashSimon(color) {
  const btn = document.getElementById(color);
  btn.classList.add('active');
  setTimeout(() => btn.classList.remove('active'), 400);
}
function playSimonPattern() {
  let i = 0;
  const interval = setInterval(() => {
    flashSimon(simonPattern[i]);
    i++;
    if (i >= simonPattern.length) clearInterval(interval);
  }, 600);
}
function startSimon() {
  simonPattern = [];
  simonUser = [];
  nextSimonColor();
}
function nextSimonColor() {
  const color = simonColors[Math.floor(Math.random() * 4)];
  simonPattern.push(color);
  playSimonPattern();
}
simonColors.forEach(color => {
  document.getElementById(color).addEventListener('click', () => {
    simonUser.push(color);
    flashSimon(color);
    const current = simonUser.length - 1;
    if (simonUser[current] !== simonPattern[current]) {
      alert('Wrong pattern! Try again.');
      simonUser = [];
      return;
    }
    if (simonUser.length === simonPattern.length) {
      simonUser = [];
      nextSimonColor();
    }
  });
});

// ==== Bollywood Trivia ====
const questions = [
  {
    question: "Who played the role of 'Rancho' in 3 Idiots?",
    options: ["Aamir Khan", "Ranbir Kapoor", "Salman Khan", "Shah Rukh Khan"],
    answer: "Aamir Khan"
  },
  {
    question: "Which movie featured the song 'Chaiyya Chaiyya'?",
    options: ["Dil Se", "Raees", "Don", "Kal Ho Na Ho"],
    answer: "Dil Se"
  },
  {
    question: "Which actress starred in 'Queen'?",
    options: ["Kangana Ranaut", "Deepika Padukone", "Alia Bhatt", "Kareena Kapoor"],
    answer: "Kangana Ranaut"
  },
  {
    question: "In which movie did Shah Rukh Khan play a hockey coach?",
    options: ["Chak De! India", "Darr", "Fan", "Main Hoon Na"],
    answer: "Chak De! India"
  }
];
let quizIndex = 0;
function showQuestion() {
  const q = questions[quizIndex];
  document.getElementById('quiz-question').innerText = q.question;
  const optionsDiv = document.getElementById('quiz-options');
  optionsDiv.innerHTML = '';
  q.options.forEach(opt => {
    const btn = document.createElement('button');
    btn.innerText = opt;
    btn.onclick = () => checkAnswer(opt);
    optionsDiv.appendChild(btn);
  });
}
function checkAnswer(selected) {
  const correct = questions[quizIndex].answer;
  const feedback = selected === correct ? "✅ Correct!" : `❌ Wrong. It was ${correct}`;
  document.getElementById('quiz-feedback').innerText = feedback;
}
function nextQuestion() {
  quizIndex = (quizIndex + 1) % questions.length;
  document.getElementById('quiz-feedback').innerText = '';
  showQuestion();
}
showQuestion();
</script>
<section id="adios" style="background-color: #0a0a0a; color: #fff; padding: 4rem; font-family: 'Creepster', cursive;">
  <h2 style="text-align: center; text-decoration: underline; font-size: 2.5rem;">🌙 Adios</h2>
  <p style="text-align: center; max-width: 600px; margin: auto; font-size: 1.3rem;">
    Thank you for exploring my little spooky world! 
    This was just a witchy beginning—more chaos, more spells, and more stories will brew soon. 
    Stay weird, stay magical. ✨🧙‍♀️💀<br><br>
    Adios, fellow night crawler!
  </p>
    </section>
    </body>
