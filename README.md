# dazzthezeuz
dazzwebb11
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Social Hub</title>
  <style>
    body {
      background: url('https://share.google/mxLUr5lL0707bzeGd') center/cover no-repeat fixed;
      color: #fff;
      font-family: 'Poppins', sans-serif;
      text-align: center;
      padding: 50px;
      backdrop-filter: blur(2px);
      transition: opacity 0.6s ease;
    }
    h1 {
      margin-bottom: 30px;
      font-size: 36px;
      font-weight: 700;
      letter-spacing: 2px;
      text-shadow: 0 0 12px #00eaff, 0 0 25px #0077ff;
    }
    .social-container {
      display: flex;
      flex-direction: column;
      gap: 18px;
      width: 320px;
      margin: 0 auto;
      animation: fadeIn 1.2s ease-out;
    }
    a {
      display: block;
      padding: 16px;
      background: rgba(0, 0, 0, 0.55);
      border-radius: 14px;
      color: #fff;
      text-decoration: none;
      font-size: 20px;
      font-weight: 600;
      border: 2px solid #00d4ff;
      box-shadow: 0 0 12px #00eaff;
      transition: 0.25s;
    }
    a:hover {
      transform: scale(1.05);
      box-shadow: 0 0 25px #00eaff;
      background: rgba(0, 0, 0, 0.7);
    }
    @keyframes fadeIn {
      from {
        opacity: 0;
        transform: translateY(20px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }
    .btn {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 12px;
      padding: 16px;
      background: rgba(0,0,0,0.55);
      border-radius: 16px;
      border: 2px solid #00eaff;
      box-shadow: 0 0 12px #00eaff;
      transition: 0.35s ease;
      cursor: pointer;
      animation: glowPulse 2s infinite;
    }
    .btn:hover {
      transform: translateY(-6px) scale(1.08);
      box-shadow: 0 0 25px #00eaff, 0 0 45px #00bbff;
      background: rgba(0,0,0,0.8);
    }
    .icon {
      width: 28px;
      height: 28px;
      filter: drop-shadow(0 0 6px #00eaff);
    }
    @keyframes glowPulse {
      0% { box-shadow: 0 0 10px #00eaff; }
      50% { box-shadow: 0 0 22px #00bbff; }
      100% { box-shadow: 0 0 10px #00eaff; }
    }
    .fade-out { opacity: 0; transition: opacity 0.5s ease; }
  </style>
</head>
<body>
  <h1>Social Media Hub</h1>
  <div class="social-container">
    <a href="https://www.tiktok.com/@sdazztzy77?_r=1&_t=ZS-91SvJuocxSa" target="_blank" class="btn">
      <img src="https://cdn-icons-png.flaticon.com/512/3046/3046121.png" class="icon" alt="TikTok"> TikTok
    </a>
    <a href="https://www.instagram.com/sdazz_tzy_77?igsh=MWNqd3J5N2J2NGl1Zw==" target="_blank" class="btn">
      <img src="https://cdn-icons-png.flaticon.com/512/1384/1384063.png" class="icon" alt="Instagram"> Instagram
    </a>
    <a href="https://youtube.com/@serginhodazz?si=PNgkAEJCRQUhXpCE" target="_blank" class="btn">
      <img src="https://cdn-icons-png.flaticon.com/512/1384/1384060.png" class="icon" alt="YouTube"> YouTube
    </a>
    <a href="https://t.me/@sdazztzy77" target="_blank" class="btn">
      <img src="https://cdn-icons-png.flaticon.com/512/2111/2111646.png" class="icon" alt="Telegram"> Telegram
    </a>
    <a href="https://whatsapp.com/channel/0029Vb6Mk0K4o7qJeHOURY0k" target="_blank" class="btn">
      <img src="https://cdn-icons-png.flaticon.com/512/733/733585.png" class="icon" alt="WhatsApp"> WhatsApp
    </a>
  </div>
  <audio id="clickSound" src="https://cdn.pixabay.com/download/audio/2022/03/15/audio_7e53f87f5e.mp3?filename=ui-click-124608.mp3"></audio>
  <audio id="bgm" src="SpotiDown.App - i am a monster - Orlando Kallen.mp3" autoplay loop></audio>
  <script>
    const sound = document.getElementById('clickSound');
    document.querySelectorAll('.btn').forEach(btn => {
      btn.addEventListener('click', () => {
        sound.currentTime = 0;
        sound.play();
        document.body.classList.add('fade-out');
        setTimeout(() => {
          document.body.classList.remove('fade-out');
        }, 500);
      });
    });
  </script>
</body>
</html>
