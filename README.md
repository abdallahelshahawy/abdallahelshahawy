<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Abdallah Elshahawey</title>
  <style>
    body {
      font-family: "Poppins", sans-serif;
      background: radial-gradient(circle at center, #0a0a0f, #000);
      color: #fff;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
      overflow: hidden;
    }

    h1 {
      font-size: 3.5rem;
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 2px;
      color: #b400ff;
      text-shadow: 0 0 10px #b400ff, 0 0 20px #b400ff, 0 0 40px #b400ff;
      position: relative;
      animation: neonPulse 2s infinite alternate, heartbeatSync 2s infinite ease-in-out;
    }

    @keyframes neonPulse {
      from {
        text-shadow: 0 0 10px #b400ff, 0 0 20px #b400ff, 0 0 40px #b400ff;
      }
      to {
        text-shadow: 0 0 20px #ff00ff, 0 0 40px #b400ff, 0 0 80px #b400ff;
      }
    }

    @keyframes heartbeatSync {
      0%, 100% { transform: scale(1); }
      25% { transform: scale(1.05); }
      50% { transform: scale(1); }
      75% { transform: scale(1.07); }
    }

    .heartbeat-line {
      width: 180px;
      height: 2px;
      background: linear-gradient(90deg, transparent, #b400ff, transparent);
      position: relative;
      margin-top: 10px;
      overflow: hidden;
    }

    .heartbeat-line::before {
      content: "";
      position: absolute;
      left: 0;
      top: -10px;
      width: 100%;
      height: 20px;
      background: transparent;
      border-left: 2px solid #b400ff;
      border-right: 2px solid transparent;
      transform: translateX(-100%);
      animation: heartbeat 2s infinite linear;
    }

    @keyframes heartbeat {
      0%, 100% {
        transform: translateX(-100%);
      }
      25% {
        transform: translateX(10%);
        border-color: #ff00ff;
      }
      50% {
        transform: translateX(50%);
        border-color: #b400ff;
      }
      75% {
        transform: translateX(110%);
        border-color: #ff00ff;
      }
    }

    .contact {
      margin-top: 40px;
      font-size: 1.1rem;
    }

    .contact a {
      color: #b400ff;
      text-decoration: none;
      border-bottom: 1px dashed #b400ff;
      transition: all 0.3s ease;
    }

    .contact a:hover {
      color: #ff00ff;
      border-bottom-color: #ff00ff;
      text-shadow: 0 0 10px #ff00ff;
    }

    .robot {
      position: absolute;
      bottom: 40px;
      width: 100px;
      animation: floatRobot 3s ease-in-out infinite;
    }

    @keyframes floatRobot {
      0%, 100% {
        transform: translateY(0);
      }
      50% {
        transform: translateY(-10px);
      }
    }
  </style>
</head>
<body>
  <h1>Abdallah Elshahawey</h1>
  <div class="heartbeat-line"></div>

  <div class="contact">
    📧 <a href="mailto:abdallahelshahawey@gmail.com">abdallahelshahawey@gmail.com</a>
  </div>

  <img class="robot" src="https://cdn-icons-png.flaticon.com/512/4712/4712027.png" alt="3D Robot">
</body>
</html>
```
