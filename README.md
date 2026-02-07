<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>For Bhumiiiii ❤️</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: linear-gradient(135deg, #ffdde1, #ee9ca7);
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      text-align: center;
      padding: 20px;
    }

    .card {
      background: white;
      padding: 25px;
      border-radius: 20px;
      max-width: 420px;
      width: 100%;
      box-shadow: 0 10px 30px rgba(0,0,0,0.2);
    }

    h1 {
      font-size: 26px;
      margin-bottom: 10px;
      color: #ff2d55;
    }

    p {
      font-size: 18px;
      color: #333;
      margin-bottom: 25px;
    }

    .buttons {
      display: flex;
      justify-content: center;
      gap: 15px;
      flex-wrap: wrap;
    }

    button {
      border: none;
      padding: 14px 22px;
      border-radius: 14px;
      font-size: 18px;
      cursor: pointer;
      transition: 0.2s ease;
    }

    #yesBtn {
      background: #ff2d55;
      color: white;
      font-size: 18px;
    }

    #noBtn {
      background: #444;
      color: white;
      font-size: 18px;
    }

    /* Popup */
    .popup {
      position: fixed;
      inset: 0;
      background: rgba(0,0,0,0.6);
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 20px;
    }

    .popupBox {
      background: white;
      padding: 25px;
      border-radius: 18px;
      max-width: 400px;
      width: 100%;
      text-align: center;
      box-shadow: 0 10px 30px rgba(0,0,0,0.3);
    }

    .popupBox h2 {
      margin: 0;
      color: #ff2d55;
      font-size: 24px;
    }

    .popupBox button {
      margin-top: 18px;
      background: #ff2d55;
      color: white;
      width: 100%;
      font-size: 18px;
      border-radius: 14px;
    }

    #result {
      margin-top: 20px;
      font-size: 20px;
      font-weight: bold;
      color: #ff2d55;
    }
  </style>
</head>

<body>

  <!-- Popup -->
  <div class="popup" id="popup">
    <div class="popupBox">
      <h2>Good Morning Madam Jiii ❤️</h2>
      <button onclick="closePopup()">Aww okay 😘</button>
    </div>
  </div>

  <!-- Main Card -->
  <div class="card">
    <h1>Hey Bhumiiiii ❤️</h1>
    <p>
      Today is a special day... 🥺✨ <br><br>
      Will you accept my proposal? 💍❤️
    </p>

    <div class="buttons">
      <button id="yesBtn" onclick="sayYes()">YES 😍</button>
      <button id="noBtn" onclick="sayNo()">NO 🙄</button>
    </div>

    <div id="result"></div>
  </div>

  <script>
    let yesSize = 18;

    function closePopup() {
      document.getElementById("popup").style.display = "none";
    }

    function sayNo() {
      yesSize += 10;
      const yesBtn = document.getElementById("yesBtn");
      yesBtn.style.fontSize = yesSize + "px";
      yesBtn.style.padding = (14 + yesSize/4) + "px " + (22 + yesSize/3) + "px";
    }

    function sayYes() {
      document.getElementById("result").innerHTML =
        "YAYYYYY ❤️🥰 I love you Bhumiiiii 😘💍";
    }
  </script>

</body>
</html>
