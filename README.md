<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>🎉 Happy Birthday Chellam 🎉</title>
  <style>
    body {
      background: black;
      color: #00ffcc;
      font-family: 'Courier New', monospace;
      text-align: center;
      padding: 50px 20px;
      overflow: hidden;
    }
    .tap {
      font-size: 24px;
      color: #ff66aa;
      animation: blink 1s step-start infinite;
    }
    #message {
      display: none;
      margin-top: 30px;
      font-size: 18px;
      line-height: 1.8;
      white-space: pre-wrap;
    }
    @keyframes blink {
      50% { opacity: 0; }
    }
    .heart {
      position: fixed;
      width: 20px;
      height: 20px;
      background: red;
      transform: rotate(45deg);
      animation: fall 6s linear infinite;
    }
    .heart::before,
    .heart::after {
      content: '';
      position: absolute;
      width: 20px;
      height: 20px;
      background: red;
      border-radius: 50%;
    }
    .heart::before { top: -10px; left: 0; }
    .heart::after { top: 0; left: -10px; }
    @keyframes fall {
      0% { transform: translateY(0) rotate(45deg); opacity: 1; }
      100% { transform: translateY(100vh) rotate(45deg); opacity: 0; }
    }
  </style>
</head>
<body onclick="revealMessage()">
  <div class="tap">💋 Tap anywhere to reveal your surprise 💋</div>

  <div id="message">
Happy b'day to a true gem
Enjoy ur day da chelllooo
my konjing patner 💋
May ur heart be full of happiness 😊
Cheers to another year of great memories
May all ur dreams come true this year da chellooo
May ur bday bring ur endless happiness have fun da mah
Wishing u a year filled with blessings and smiles
Wishing you a year of health happiness 😊 and success
Even when I close my eyes my thoughts are only about you
You didn’t just enter my life – you added colors to every moment
Your smile is the sound my heart waits for every day
Today is your❤️ birthday🎂… just because you’re a part of my world.
I wish every dream of yours turns into reality, and every effort of yours becomes a victory🤗

En ❤️ la nethan admin user👨‍💻
Ne en life la login akiruka logout option lam kidaiyathu da 🤭
Un love la infinite loop ..exit kudukave mudiyala 😌
Dei chellamea en heart beat la root access eduthuta ❤️‍🩹
but you didn’t just hack Mobiles — you hacked my heart first ❤️

Happy Birthday, my everything.
I don’t just wish for your happiness, I want to be the reason for it always.

"You will be glad and have great delight; and numbers of people will have joy at his birth
May the Lord send his blessing on you and keep you
May the light of the Lord's face be shining on you in grace:
May the Lord's approval be resting on you and may he give you peace.
May he give you your heart's desire, and put all your purposes into effect

Chello Sakura varai naan unkuda dhan iruppen
En life la kedacha rba periya gift da chelllooo ne 🫂
Ne ennoda paathi lam illa ennoda fullume nedhan da en uiree
Yarum happy aa vachukatha alavuku enaya happy aa vachukutta rba thanks da pow ne en life la vanthathu ku

Ne ethukum feel panna kudathu un life full aaa enjoy Pannu da mah
Jesus un pakkam da chello pls Yarukakavum alatha da chello
Unnaya ala vachathuku romba sorryyy kannna
God bless u da chelllooo 💋

I love u very much da chellooo 🫂💋
Ummmmmmmmmmmmmmmmmmmmmmmmmmmmmmmaaaaaaaaaaa 💋
  </div>

  <audio id="kissSound" src="https://www.fesliyanstudios.com/play-mp3/387"></audio>

  <script>
    let opened = false;
    function revealMessage() {
      if (!opened) {
        document.querySelector('.tap').style.display = 'none';
        document.getElementById('message').style.display = 'block';
        document.getElementById('kissSound').play();
        setInterval(createHeart, 300);
        opened = true;
      }
    }

    function createHeart() {
      const heart = document.createElement("div");
      heart.classList.add("heart");
      heart.style.left = Math.random() * 100 + "vw";
      heart.style.animationDuration = (Math.random() * 2 + 4) + "s";
      document.body.appendChild(heart);
      setTimeout(() => heart.remove(), 6000);
    }
  </script>
</body>
</html>
