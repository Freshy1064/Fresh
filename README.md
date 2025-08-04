<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>One Piece Devil Fruits</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #000;
      color: #fff;
    }

    header {
      background-color: #111;
      padding: 15px 30px;
      text-align: center;
      font-size: 30px;
      font-weight: bold;
      border-bottom: 3px solid #e91e63;
    }

    .container {
      padding: 30px;
      text-align: center;
    }

    .devil-fruit-list {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
    }

    .devil-fruit {
      background-color: #1e1e1e;
      border: 2px solid #e91e63;
      border-radius: 10px;
      padding: 20px;
      width: 200px;
      transition: transform 0.3s ease, background-color 0.3s ease;
      cursor: pointer;
    }

    .devil-fruit:hover {
      transform: scale(1.05);
      background-color: #2c2c2c;
    }

    .devil-fruit h3 {
      margin: 0 0 10px 0;
      color: #e91e63;
    }

    .devil-fruit p {
      font-size: 14px;
    }
  </style>
</head>
<body>

  <header>
    Devil Fruits of One Piece
  </header>

  <div class="container">
    <p>Click on any Devil Fruit to explore more:</p>

    <div class="devil-fruit-list">
      <div class="devil-fruit" onclick="location.href='https://freshy1064.github.io/One-pieceI/'">
        <h3>Gomu Gomu no Mi</h3>
        <p>Luffy's legendary Devil Fruit that turns his body into rubber.</p>
      </div>

      <div class="devil-fruit" onclick="location.href='https://freshy1064.github.io/One-pieceI/'">
        <h3>Mera Mera no Mi</h3>
        <p>Flame Flame Fruit, once eaten by Ace, controls fire.</p>
      </div>

      <div class="devil-fruit" onclick="location.href='https://freshy1064.github.io/One-pieceI/'">
        <h3>Hie Hie no Mi</h3>
        <p>Ice Ice Fruit used by Aokiji, can freeze anything instantly.</p>
      </div>

      <div class="devil-fruit" onclick="location.href='https://freshy1064.github.io/One-pieceI/'">
        <h3>Pika Pika no Mi</h3>
        <p>Light Light Fruit used by Kizaru, grants speed of light powers.</p>
      </div>
    </div>
  </div>

</body>
</html>
