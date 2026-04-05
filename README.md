<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Live Love Animation</title>
<style>
  body {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background-color: #222;
    margin: 0;
    font-family: Arial, sans-serif;
  }

  .animated-text {
    font-size: 4em;
    font-weight: bold;
    letter-spacing: 0.1em;
    animation: pulse 2s infinite, colorChange 1s infinite;
  }

  @keyframes pulse {
    0% { transform: scale(1); }
    50% { transform: scale(1.2); }
    100% { transform: scale(1); }
  }

  @keyframes colorChange {
    0% { color: #ff4d4d; }
    25% { color: #ffcc00; }
    50% { color: #4dff4d; }
    75% { color: #00ccff; }
    100% { color: #ff4d4d; }
  }
</style>
</head>
<body>
  <div class="animated-text">😁THANK YOU🌹</div>
</body>
</html>
