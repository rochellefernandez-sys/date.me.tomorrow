<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Date with Me?</title>
  <style>
    body {
      font-family: 'Arial', sans-serif;
      background: linear-gradient(135deg, #FFDEE9, #B5FFFC);
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      height: 100vh;
      text-align: center;
      color: #333;
    }

    h1 {
      font-size: 3em;
      margin-bottom: 20px;
    }

    p {
      font-size: 1.5em;
      margin-bottom: 30px;
    }

    button {
      font-size: 1.2em;
      padding: 15px 30px;
      margin: 10px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      transition: 0.3s;
    }

    #yes {
      background-color: #FF6B6B;
      color: white;
    }

    #no {
      background-color: #4ECDC4;
      color: white;
      position: relative;
    }

    #no:hover {
      background-color: #1A535C;
    }
  </style>
</head>
<body>
  <h1>Hey, Dongsy! 💖</h1>
  <p>Would you go on a date with me?</p>
  <button id="yes">Yes 😍</button>
  <button id="no">No 😢</button>

  <script>
    const yesButton = document.getElementById('yes');
    const noButton = document.getElementById('no');

    yesButton.addEventListener('click', () => {
      alert("Yay! I can't wait! 💕");
    });

    // Make the 'No' button move away when hovered
    noButton.addEventListener('mouseenter', () => {
      const x = Math.random() * (window.innerWidth - noButton.clientWidth);
      const y = Math.random() * (window.innerHeight - noButton.clientHeight);
      noButton.style.position = "absolute";
      noButton.style.left = x + "px";
      noButton.style.top = y + "px";
    });
  </script>
</body>
</html>
