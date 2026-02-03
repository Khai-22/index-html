# index-html
for my valentine Chel
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Happy Valentine’s Day</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      font-family: Arial, sans-serif;
    }

    .card {
      text-align: center;
      color: white;
    }

    .heart {
      width: 100px;
      height: 100px;
      background: red;
      position: relative;
      transform: rotate(-45deg);
      animation: beat 1s infinite;
      margin: 0 auto 20px;
    }

    .heart::before,
    .heart::after {
      content: "";
      width: 100px;
      height: 100px;
      background: red;
      border-radius: 50%;
      position: absolute;
    }

    .heart::before {
      top: -50px;
      left: 0;
    }

    .heart::after {
      left: 50px;
      top: 0;
    }

    @keyframes beat {
      0%, 100% { transform: scale(1) rotate(-45deg); }
      50% { transform: scale(1.1) rotate(-45deg); }
    }

    h1 {
      margin: 0;
    }
  </style>
</head>
<body>
  <div class="card">
    <div class="heart"></div>
    <h1>Happy Valentine’s Day ❤️</h1>
    <p>You make my heart beat faster</p>
  </div>
</body>
</html>
