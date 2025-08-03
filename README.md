<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>One Piece Home</title>
<style>
  /* Basic Reset */
  * {
    box-sizing: border-box;
  }
  body {
    background-color: #121212;
    color: white;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    margin: 0; padding: 0;
  }
  nav {
    background: linear-gradient(90deg, #0b0b0b, #1a1a1a);
    box-shadow: 0 4px 8px rgba(0,0,0,0.7);
    padding: 12px 20px;
    position: relative;
    z-index: 100;
  }
  .menu-button {
    width: 35px;
    height: 28px;
    cursor: pointer;
    position: relative;
    display: inline-block;
  }
  .menu-button span {
    background: white;
    display: block;
    height: 4px;
    width: 100%;
    border-radius: 2px;
    position: absolute;
    left: 0;
    transition: 0.3s ease;
  }
  .menu-button span:nth-child(1) { top: 0; }
  .menu-button span:nth-child(2) { top: 12px; }
  .menu-button span:nth-child(3) { top: 24px; }
  .menu-button.active span:nth-child(1) {
    transform: rotate(45deg);
    top: 12px;
  }
  .menu-button.active span:nth-child(2) {
    opacity: 0;
  }
  .menu-button.active span:nth-child(3) {
    transform: rotate(-45deg);
    top: 12px;
  }
  .menu-items {
    max-height: 0;
    overflow: hidden;
    transition: max-height 0.4s ease;
    text-align: center;
  }
  .menu-items.active { max-height: 500px; }
  .menu-items a {
    display: block;
    padding: 12px 0;
    color: #eee;
    text-decoration: none;
    font-weight: 600;
    font-size: 20px;
    border-bottom: 1px solid rgba(255,255,255,0.1);
    transition: color 0.3s ease;
  }
  .menu-items a:hover {
    color: #f9d71c;
    text-shadow: 0 0 6px #f9d71c;
  }
  .menu-items a.active {
    color: #f9d71c;
    font-weight: 700;
    text-shadow: 0 0 8px #f9d71c;
    border-bottom: 2px solid #f9d71c;
    padding-bottom: 4px;
  }
  @media (min-width: 700px) {
    .menu-button { display: none; }
    .menu-items {
      max-height: none !important;
      display: flex;
      justify-content: center;
      overflow: visible;
      text-align: initial;
    }
    .menu-items a {
      border: none;
      margin: 0 25px;
      font-size: 18px;
      padding: 0;
      line-height: 1;
    }
    .menu-items a.active {
      border-bottom: 2px solid #f9d71c;
      padding-bottom: 6px;
    }
  }
  .container {
    max-width: 900px;
    margin: 30px auto;
    padding: 0 20px;
    text-align: center;
  }

  /* Straw Hat Crew */
  #straw-hat-crew {
    max-width: 800px;
    margin: 40px auto;
    text-align: left;
    padding: 0 20px;
  }
  #straw-hat-crew h2 {
    font-family: 'Pirata One', cursive;
    font-size: 2.5em;
    color: #f9d71c;
    text-align: center;
    margin-bottom: 20px;
  }
  #straw-hat-crew ul {
    list-style-type: disc;
    padding-left: 20px;
  }
  #straw-hat-crew li {
    margin-bottom: 10px;
    font-size: 1.1em;
  }
  #straw-hat-crew strong {
    color: #f9d71c;
  }

  /* Journey section */
  #journey {
    max-width: 800px;
    margin: 40px auto 80px auto;
    text-align: left;
    padding: 0 20px;
  }
  #journey h2 {
    font-family: 'Pirata One', cursive;
    font-size: 2.5em;
    color: #f9d71c;
    text-align: center;
    margin-bottom: 20px;
  }
  #journey p {
    font-size: 1.2em;
    line-height: 1.6;
    color: #eee;
    margin-bottom: 15px;
  }
</style>
<link href="https://fonts.googleapis.com/css2?family=Pirata+One&display=swap" rel="stylesheet" />
</head>
<body>
  <nav>
    <div class="menu-button" id="menu-button" aria-label="Toggle menu" role="button" tabindex="0">
      <span></span><span></span><span></span>
    </div>
    <div class="menu-items" id="menu-items">
      <a href="index.html" class="active">Home</a>
      <a href="devil-fruit.html">Devil Fruit</a>
      <a href="character.html">Character</a>
      <a href="story.html">Story</a>
    </div>
  </nav>

  <div class="container">
    <h1>Welcome to the One Piece Site</h1>
    <p>Meet the legendary Straw Hat Crew who sail the Grand Line!</p>

    <section id="straw-hat-crew">
      <h2>The Straw Hat Crew</h2>
      <ul>
        <li><strong>Monkey D. Luffy</strong> – Captain with the power of the Gum-Gum Fruit.</li>
        <li><strong>Roronoa Zoro</strong> – Master swordsman aiming to be the best.</li>
        <li><strong>Nami</strong> – Skilled navigator and weather expert.</li>
        <li><strong>Usopp</strong> – Sharpshooter and creative inventor.</li>
        <li><strong>Sanji</strong> – Talented cook and fighter with powerful kicks.</li>
        <li><strong>Tony Tony Chopper</strong> – Doctor and reindeer with human powers.</li>
        <li><strong>Nico Robin</strong> – Archaeologist with knowledge of ancient history.</li>
        <li><strong>Franky</strong> – Cyborg shipwright who built the Thousand Sunny.</li>
        <li><strong>Brook</strong> – Musician and swordsman who returned from the dead.</li>
        <li><strong>Jinbe</strong> – Fish-man helmsman and loyal ally.</li>
      </ul>
    </section>

    <section id="journey">
      <h2>The Journey of the Straw Hat Crew</h2>
      <p>
        After setting sail from their hometown, the Straw Hat Pirates began their grand adventure across the treacherous Grand Line, encountering powerful enemies, making new friends, and uncovering the mysteries of the world.
      </p>
      <p>
        Each crew member pursues their personal dreams while supporting each other through countless battles and challenges. From battling the Marines and rival pirates to exploring strange islands and ancient ruins, their bond grows stronger with every adventure.
      </p>
      <p>
        Their journey is full of laughter, tears, and unwavering determination — a testament to the spirit of freedom and friendship that defines One Piece.
      </p>
      <p>
        As they move closer to the legendary treasure “One Piece,” the Straw Hats face more dangerous foes and uncover dark secrets that could change the fate of the world forever.
      </p>
    </section>
  </div>

  <script>
    const menuButton = document.getElementById('menu-button');
    const menuItems = document.getElementById('menu-items');
    menuButton.addEventListener('click', () => {
      menuButton.classList.toggle('active');
      menuItems.classList.toggle('active');
    });
    menuButton.addEventListener('keydown', e => {
      if(e.key === 'Enter' || e.key === ' ') {
        e.preventDefault();
        menuButton.click();
      }
    });
  </script>
</body>
</html>
