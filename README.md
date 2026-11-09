
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Our Little World ♡</title>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Georgia, serif;
  background: linear-gradient(135deg, #fff0f5, #ffe1ec, #fce4ec);
  color: #75465b;
  min-height: 100vh;
  overflow-x: hidden;
}

#progress {
  position: fixed;
  top: 0;
  left: 0;
  height: 5px;
  width: 11.11%;
  background: #cf6f96;
  transition: width .4s;
  z-index: 20;
}

.heart {
  position: fixed;
  bottom: -30px;
  color: #e89ab8;
  animation: float 8s linear forwards;
  pointer-events: none;
  z-index: 0;
}

@keyframes float {
  to {
    transform: translateY(-110vh) rotate(360deg);
    opacity: 0;
  }
}

main {
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 35px 16px;
  position: relative;
  z-index: 1;
}

.section {
  display: none;
  width: 100%;
  max-width: 550px;
  background: rgba(255,255,255,.83);
  border: 1px solid white;
  border-radius: 25px;
  padding: 35px 24px;
  text-align: center;
  box-shadow: 0 12px 35px rgba(190,100,140,.15);
  animation: appear .5s ease;
}

.section.active {
  display: block;
}

@keyframes appear {
  from { opacity: 0; transform: translateY(15px); }
  to { opacity: 1; transform: translateY(0); }
}

.emoji {
  font-size: 45px;
  margin-bottom: 18px;
}

h1 {
  color: #c45d83;
  font-size: 31px;
  margin-bottom: 18px;
}

h2 {
  color: #c45d83;
  font-size: 23px;
  margin-bottom: 15px;
}

p {
  line-height: 1.9;
  font-size: 16px;
  margin-bottom: 17px;
}

.highlight {
  color: #b44370;
  font-weight: bold;
  background: #ffe0eb;
  padding: 3px 7px;
  border-radius: 6px;
}

.date {
  display: inline-block;
  background: #fbd1e0;
  padding: 14px 20px;
  border-radius: 15px;
  color: #a13f68;
  font-size: 22px;
  font-weight: bold;
  margin: 12px 0 20px;
  box-shadow: 0 4px 12px #e9b5ca;
}

button {
  border: none;
  cursor: pointer;
  font-family: Georgia, serif;
}

.nav-btn, .action-btn {
  background: #d8799e;
  color: white;
  padding: 13px 23px;
  border-radius: 28px;
  font-size: 15px;
  margin: 8px 4px;
  transition: .25s;
}

.nav-btn:hover, .action-btn:hover {
  background: #bd5e85;
  transform: translateY(-2px);
}

.back-btn {
  background: #f5d5e1;
  color: #a34f70;
}

.navigation {
  margin-top: 25px;
}

.small {
  font-size: 13px;
  color: #aa7b91;
  margin-top: 20px;
}

.card {
  background: #fff0f5;
  padding: 18px;
  border-radius: 17px;
  margin: 18px 0;
  line-height: 1.8;
}

.timeline {
  border-left: 3px solid #e9a5bf;
  text-align: left;
  padding-left: 18px;
  margin: 22px 8px;
}

.timeline p {
  margin-bottom: 20px;
}

.momo {
  font-size: 65px;
  margin: 15px;
}

.music {
  background: #fff0f5;
  padding: 20px;
  border-radius: 18px;
  margin: 20px 0;
}

.letter {
  text-align: left;
  line-height: 2;
  background: #fff4f7;
  padding: 20px;
  border-radius: 16px;
  white-space: pre-line;
}

input {
  width: 100%;
  padding: 14px;
  border: 2px solid #edbfd0;
  border-radius: 12px;
  font-size: 16px;
  outline: none;
  margin: 12px 0;
  color: #75465b;
  background: white;
}

input:focus {
  border-color: #cf6f96;
}

.feedback {
  min-height: 48px;
  margin-top: 12px;
  font-weight: bold;
  line-height: 1.7;
}

.hint-box {
  background: #fff0f5;
  padding: 15px;
  border-radius: 13px;
  margin-top: 12px;
  line-height: 1.7;
  display: none;
}

.secret {
  display: none;
  margin-top: 20px;
  animation: appear .8s ease;
}

.secret h1 {
  font-size: 36px;
  color: #c03970;
}

.secret-letter {
  background: #fff0f5;
  padding: 20px;
  border-radius: 16px;
  text-align: left;
  line-height: 2;
  margin-top: 20px;
  white-space: pre-line;
}

@media(max-width: 400px) {
  .section { padding: 28px 18px; }
  h1 { font-size: 27px; }
}
</style>
</head>

<body>

<div id="progress"></div>

<main>

<!-- SECTION 1 -->
<div class="section active" id="s1">
  <div class="emoji">🌸</div>
  <h1>A Little Surprise</h1>
  <p>
    Sometimes, one unexpected message becomes
    the beginning of something beautiful...
  </p>

  <div class="date">31 October 2026</div>

  <p>
    The day two strangers crossed paths,
    and an unexpected friendship began. ♡
  </p>

  <p>
    This little website has a story,
    some surprises, and a special place
    dedicated to you.
  </p>

  <button class="action-btn" onclick="go(2)">
    Begin Our Journey ♡
  </button>

  <div class="small">Made with friendship & a little magic ✨</div>
</div>


<!-- SECTION 2 -->
<div class="section" id="s2">
  <div class="emoji">📖</div>
  <h1>How It All Started</h1>

  <p>
    Every beautiful story has a beginning.
    And ours started with something as simple
    as an Instagram message.
  </p>

  <div class="timeline">
    <p>📱 <b>A little message</b><br>
    Someone decided to say hello. (Yes, it was me! 😂)</p>

    <p>💬 <b>A conversation</b><br>
    One message slowly turned into conversations.</p>

    <p>❤️ <b>A friendship</b><br>
    And somehow, a stranger became a special friend.</p>
  </div>

  <div class="card">
    I never knew that sending one simple message
    would introduce me to someone like you.
  </div>

  <p>Funny how the smallest beginnings can mean so much. ♡</p>

  <div class="navigation">
    <button class="nav-btn back-btn" onclick="go(1)">← Back</button>
    <button class="nav-btn" onclick="go(3)">Next →</button>
  </div>
</div>


<!-- SECTION 3 -->
<div class="section" id="s3">
  <div class="emoji">🌍</div>
  <h1>Our Little World</h1>

  <p>
    Different places, different skies,
    but somehow we found a little world of our own.
  </p>

  <div class="card">
    <h2>FRIEND + SHIP = ?</h2>
    <p>
      Sometimes distance separates places,
      but it doesn't have to separate people.
    </p>
  </div>

  <p>
    We haven't met in person yet,
    but that doesn't make our friendship
    any less meaningful.
  </p>

  <p>
    Miles apart, but connected through
    countless conversations. ♡
  </p>

  <div class="navigation">
    <button class="nav-btn back-btn" onclick="go(2)">← Back</button>
    <button class="nav-btn" onclick="go(4)">Next →</button>
  </div>
</div>


<!-- SECTION 4 -->
<div class="section" id="s4">
  <div class="emoji">🥟</div>
  <h1>Momo Corner</h1>

  <div class="momo">🥟🥟🥟</div>

  <h2>Guess who loves MOMO?</h2>

  <p>
    Of course, it's YOU! 😂
  </p>

  <div class="card">
    If friendship had a favourite food,
    I bet yours would be momo!
  </div>

  <button class="action-btn" onclick="momoSurprise()">
    Give Me Some MOMO! 🥟
  </button>

  <p id="momoMessage" class="feedback"></p>

  <p class="small">Sending you unlimited virtual momos! 😂</p>

  <div class="navigation">
    <button class="nav-btn back-btn" onclick="go(3)">← Back</button>
    <button class="nav-btn" onclick="go(5)">Next →</button>
  </div>
</div>


<!-- SECTION 5 -->
<div class="section" id="s5">
  <div class="emoji">🎧</div>
  <h1>Your Voice, Your Magic</h1>

  <div class="music">
    <div style="font-size:45px;">🎶</div>
    <h2>A Voice Worth Listening To</h2>
    <p>Some voices make songs beautiful.
    Yours makes them unforgettable.</p>
  </div>

  <p>
    A little appreciation for the girl
    whose singing deserves its own playlist.
  </p>

  <div class="card">
    Never stop singing.
    The world deserves to hear your beautiful voice. ♡
  </div>

  <p class="small">
    A special music recording can be added here later,
    with your permission.
  </p>

  <div class="navigation">
    <button class="nav-btn back-btn" onclick="go(4)">← Back</button>
    <button class="nav-btn" onclick="go(6)">Next →</button>
  </div>
</div>


<!-- SECTION 6 -->
<div class="section" id="s6">
  <div class="emoji">💌</div>
  <h1>A Letter For You</h1>

  <p>
    There are some things that deserve
    more than an ordinary message.
  </p>

  <div class="card">
    <h2>A little letter, just for you ♡</h2>
    <p>
      I may not have met you in person yet,
      but that doesn't make our friendship
      any less meaningful.
    </p>
    <p>
      Thank you for every conversation,
      every laugh, and every little moment
      that made an ordinary day better.
    </p>
    <p>
      I'm genuinely glad that our paths crossed.
      I hope this friendship keeps growing
      into something beautiful.
    </p>
    <p><b>I'm glad I sent that first message. ❤️</b></p>
  </div>

  <div class="navigation">
    <button class="nav-btn back-btn" onclick="go(5)">← Back</button>
    <button class="nav-btn" onclick="go(7)">Next →</button>
  </div>
</div>


<!-- SECTION 7 -->
<div class="section" id="s7">
  <div class="emoji">🧩</div>
  <h1>The Secret Mission</h1>

  <p>
    Welcome, detective! 🔍
    Three little puzzles are waiting for you.
    Find the clues hidden throughout this website!
  </p>

  <div class="card">
    <b>Puzzle 1 — The Beginning</b>
    <p>What is the date when our friendship story began?</p>
    <input id="answer1" placeholder="Enter your answer...">
    <button class="action-btn" onclick="check(1)">Check Answer</button>
    <button class="nav-btn back-btn" onclick="hint(1)">Hint 💡</button>
    <div class="hint-box" id="hint1"></div>
    <div class="feedback" id="feedback1"></div>
  </div>

  <div class="card">
    <b>Puzzle 2 — Complete the Word</b>
    <p>FRIEND + SHIP = ?</p>
    <input id="answer2" placeholder="Enter your answer...">
    <button class="action-btn" onclick="check(2)">Check Answer</button>
    <button class="nav-btn back-btn" onclick="hint(2)">Hint 💡</button>
    <div class="hint-box" id="hint2"></div>
    <div class="feedback" id="feedback2"></div>
  </div>

  <div class="card">
    <b>Puzzle 3 — A Favourite Thing</b>
    <p>Which food has its own special corner on this website?</p>
    <input id="answer3" placeholder="Enter your answer...">
    <button class="action-btn" onclick="check(3)">Check Answer</button>
    <button class="nav-btn back-btn" onclick="hint(3)">Hint 💡</button>
    <div class="hint-box" id="hint3"></div>
    <div class="feedback" id="feedback3"></div>
  </div>

  <p id="puzzleProgress" class="feedback">Solved: 0 / 3</p>

  <div class="navigation">
    <button class="nav-btn back-btn" onclick="go(6)">← Back</button>
    <button class="nav-btn" onclick="go(8)">Next →</button>
  </div>
</div>


<!-- SECTION 8 -->
<div class="section" id="s8">
  <div class="emoji">♾️</div>
  <h1>A Promise For Tomorrow</h1>

  <p>
    We haven't met in person yet.
    We haven't shared the same room,
    or laughed together face to face.
  </p>

  <div class="card">
    But I hope someday we will.
    And until that day comes,
    let's keep making beautiful memories
    through every conversation.
  </div>

  <p>
    May distance remain just a number,
    and may we never become distant
    in each other's lives.
  </p>

  <h2>Not just friends by chance,</h2>
  <h2>but friends for a lifetime. ♡</h2>

  <p>One unexpected beginning. A friendship I hope never ends. ♾️</p>

  <button class="action-btn" onclick="go(9)">
    One Last Surprise... 👀
  </button>

  <div class="navigation">
    <button class="nav-btn back-btn" onclick="go(7)">← Back</button>
  </div>
</div>


<!-- SECTION 9 -->
<div class="section" id="s9">
  <div class="emoji">🤫</div>
  <h1>The Final Secret</h1>

  <p>
    Before this little journey ends,
    there's something I've wanted to tell you.
  </p>

  <div class="card">
    Some secrets are difficult to keep...
    and this one is finally ready to come out. 😂
  </div>

  <button class="action-btn" id="revealButton" onclick="revealSecret()">
    I'M READY FOR THE TRUTH 👀
  </button>

  <div class="secret" id="secret">
    <h1>I CAN SPEAK! 😭❤️</h1>

    <div class="secret-letter">
Okay... there's something I've been wanting to tell you. ❤️

Do you remember when I told you that I couldn't speak?

And do you remember what you said?

You said you would learn sign language so that we could still communicate with each other.

I don't think you realize how much that moment meant to me.

You were willing to learn an entirely new language just to make sure we could understand each other. You didn't make me feel different, you didn't make me feel left out. Instead, you were ready to make an effort just to stay connected with me.

And honestly, that touched my heart more than I could ever explain.

But there's something I need to confess...

I CAN SPEAK. 😭❤️

Yes... I know. I can already imagine your reaction right now! 😂

I'm truly sorry for not telling you the truth earlier. I never wanted to make you feel that your kindness was something to laugh about. In fact, it made me realize how lucky I am to have a friend like you.

You were ready to learn a whole new way of communicating just for me, while I didn't even realize how much that little gesture would mean.

Thank you for being so thoughtful, patient and kind.

And please, don't ever think that your willingness to learn sign language was wasted. It showed me something beautiful about you — that you genuinely care about the people who matter to you.

We haven't met in person yet, but moments like this remind me that a meaningful connection doesn't always need physical presence.

One day, I hope we'll meet, laugh about this together, and remember this little confession as one of the funniest stories of our friendship.

Until then, please stay the same kind-hearted person you've always been.

I'm sorry for the little lie, but I'll always be grateful for the beautiful friendship behind it.

You didn't need to learn a new language to reach me. Your kindness had already reached my heart. ♡
    </div>

    <p style="margin-top:20px;">
      Thank you for being you. ❤️
    </p>
  </div>

  <div class="navigation">
    <button class="nav-btn back-btn" onclick="go(8)">← Back</button>
    <button class="nav-btn" onclick="go(1)">Start Again ♡</button>
  </div>
</div>

</main>

<script>
let current = 1;

function go(number) {
  document.querySelectorAll(".section").forEach(section => {
    section.classList.remove("active");
  });

  document.getElementById("s" + number).classList.add("active");
  current = number;

  document.getElementById("progress").style.width =
    (number / 9 * 100) + "%";

  window.scrollTo({ top: 0, behavior: "smooth" });
}

function momoSurprise() {
  document.getElementById("momoMessage").innerText =
    "🥟 Virtual momo delivery successful! Unlimited momos for you! 😂❤️";
}

let hintCounts = [0, 0, 0, 0];
let solved = [false, false, false, false];

const hints = {
  1: [
    "Think about the day when a simple Instagram message started something special. 💌",
    "The date is highlighted somewhere near the beginning of this website. 👀",
    "Go back to the A Little Surprise section and look carefully! 🌸",
    "Detectiveee! 😂 Visit Section 1. The date is waiting for you!"
  ],
  2: [
    "Think about the special connection between two people. ❤️",
    "The answer is made by joining the two words shown in the question.",
    "Visit Our Little World. The two parts of the answer are highlighted there!",
    "You're making me work hard! 😂 Go to Section 3 and combine FRIEND and SHIP."
  ],
  3: [
    "Think about the food she loves. 🥟",
    "It's a popular food with a soft outer layer and a tasty filling.",
    "You can find the answer in the Momo Corner section!",
    "Detective, go to Section 4! 😂 The answer is right there."
  ]
};

const answers = {
  1: ["31 october 2026", "31-10-2026", "31/10/2026", "october 31 2026"],
  2: ["friendship", "friend ship"],
  3: ["momo", "momos"]
};

function check(number) {
  const input = document.getElementById("answer" + number);
  const feedback = document.getElementById("feedback" + number);

  const answer = input.value.trim().toLowerCase().replace(/\s+/g, " ");

  if (answers[number].includes(answer)) {
    if (!solved[number]) {
      solved[number] = true;
      feedback.innerText = "Correct! You're a brilliant detective! ❤️✨";
      feedback.style.color = "#a34f70";
      updateProgress();
    } else {
      feedback.innerText = "Already solved! Well done again! ❤️";
    }
  } else {
    feedback.innerText = "Oops! Not quite. Try again! 😂";
    feedback.style.color = "#c45d83";
  }
}

function hint(number) {
  if (solved[number]) {
    document.getElementById("hint" + number).style.display = "block";
    document.getElementById("hint" + number).innerText =
      "You already solved this one! No more hints needed, detective! ❤️";
    return;
  }

  hintCounts[number]++;

  const count = hintCounts[number];
  const list = hints[number];
  const message = list[Math.min(count - 1, list.length - 1)];

  const box = document.getElementById("hint" + number);
  box.style.display = "block";
  box.innerText = "Hint " + count + ": " + message;
}

function updateProgress() {
  const total = solved.slice(1).filter(Boolean).length;
  document.getElementById("puzzleProgress").innerText =
    "Solved: " + total + " / 3";
}

function revealSecret() {
  document.getElementById("secret").style.display = "block";
  document.getElementById("revealButton").style.display = "none";
}

// Floating hearts
function createHeart() {
  const heart = document.createElement("div");
  heart.className = "heart";
  heart.innerText = Math.random() > 0.5 ? "♡" : "♥";
  heart.style.left = Math.random() * 100 + "vw";
  heart.style.fontSize = (14 + Math.random() * 18) + "px";
  heart.style.animationDuration = (5 + Math.random() * 5) + "s";

  document.body.appendChild(heart);

  setTimeout(() => heart.remove(), 10000);
}

setInterval(createHeart, 800);
</script>

</body>
</html>
