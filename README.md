<!DOCTYPE html>
<html lang="th">
<head>
  <meta charset="UTF-8">
  <title>Happy Anniversary 1 year</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <!-- Google Fonts for beautiful typography -->
  <link href="https://fonts.googleapis.com/css2?family=Kanit:wght@400;700&family=Pacifico&family=Sriracha&display=swap" rel="stylesheet">
  <style>
    body {
      background: linear-gradient(120deg, #ffd6e2 0%, #fffbe7 100%);
      min-height: 100vh;
      margin: 0;
      padding: 0;
      font-family: 'Kanit', sans-serif;
      color: #b8005c;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: flex-start;
    }
    .confetti {
      position: fixed;
      top: 0; left: 0; width: 100vw; height: 100vh;
      pointer-events: none;
      z-index: 10;
    }
    .header {
      margin-top: 50px;
      margin-bottom: 0.5em;
      font-size: 2.7rem;
      font-family: 'Pacifico', cursive;
      color: #b8005c;
      letter-spacing: 4px;
      text-shadow: 1px 5px 20px #ffdee6a0;
      position: relative;
      display: flex;
      flex-direction: column;
      align-items: center;
    }
    .header .heart {
      color: #e25555;
      font-size: 2.8rem;
      margin-top: -0.7em;
      animation: beat 1s infinite;
      filter: drop-shadow(0 2px 8px #e2555530);
    }
    @keyframes beat {
      0%, 100% { transform: scale(1);}
      50% { transform: scale(1.3);}
    }
    .main-card {
      display: flex;
      flex-direction: column;
      align-items: stretch;
      background: rgba(255,255,255,0.93);
      box-shadow: 0 6px 38px 0 #e2555522;
      border-radius: 40px;
      padding: 2.6em 2.5em 2.2em 2.5em;
      margin-bottom: 2.2em;
      width: 98vw;
      max-width: 480px;
      border: 2.8px solid #ffe6e6;
      position: relative;
      z-index: 2;
    }
    .days-box {
      background: linear-gradient(110deg, #ffe6e6 60%, #fffbe7 100%);
      border-radius: 22px;
      border: 2.5px solid #f9a6c3b8;
      box-shadow: 0 4px 20px #e2555524;
      padding: 1.5em 1em 1.2em 1em;
      margin-bottom: 1.8em;
      display: flex;
      flex-direction: column;
      align-items: center;
    }
    .days-label {
      font-size: 1.22em;
      color: #b8005c;
      font-weight: 600;
      margin-bottom: 1em;
      letter-spacing: 1.7px;
      font-family: 'Kanit', sans-serif;
    }
    .days-value {
      font-size: 2.3em;
      font-weight: 700;
      color: #eb3c74;
      letter-spacing: 2px;
      text-shadow: 0 2px 10px #ffd6e2a0;
      font-family: 'Kanit', sans-serif;
    }
    .sparkle {
      color: #ffc107;
      font-size: 1.3em;
      margin: 0 0.2em;
      animation: sparkle 1.2s infinite alternate;
    }
    @keyframes sparkle {
      0% { filter: brightness(1.2);}
      100% { filter: brightness(2.3);}
    }
    .message-box {
      background: linear-gradient(120deg, #fffbe7 70%, #ffe6e6 100%);
      border-radius: 20px;
      border: 2.5px solid #f7d2eb;
      box-shadow: 0 2px 16px #ffb3c070, 0 2px 6px #ffd6e2af;
      padding: 1.55em 1.6em 1.4em 1.6em;
      text-align: left;
      font-size: 1.15em;
      color: #b8005c;
      font-family: 'Sriracha', cursive, 'Kanit', sans-serif;
      line-height: 2.12;
      font-weight: 500;
      position: relative;
      margin-top: -0.1em;
      z-index: 1;
      box-sizing: border-box;
      display: flex;
      flex-direction: column;
      gap: 0.7em;
      white-space: pre-line;
    }
    .message-box::before {
      content: "💌";
      position: absolute;
      left: 1.25em;
      top: 1.1em;
      font-size: 1.35em;
      opacity: 0.39;
      pointer-events: none;
    }
    .video-section {
      margin: 1em 0 2em 0;
      background: linear-gradient(120deg, #fffbe7 80%, #ffe6e6 100%);
      border-radius: 22px;
      box-shadow: 0 4px 18px #e2555520;
      padding: 1.4em 1em 1.3em 1em;
      max-width: 480px;
      width: 98vw;
      border: 2px solid #f7d2eb;
      position: relative;
      z-index: 2;
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 1em;
    }
    .video-title {
      font-size: 1.1em;
      font-weight: bold;
      color: #b8005c;
      margin-bottom: 0.55em;
      letter-spacing: 1.2px;
      font-family: 'Kanit', sans-serif;
      text-align: center;
    }
    .video-embed {
      display: flex;
      justify-content: center;
      width: 100%;
      margin-bottom: 0.7em;
    }
    .video-msg {
      background: #fffbe7;
      border: 1.5px solid #f7d2eb;
      border-radius: 14px;
      padding: 1em 1em 0.9em 1em;
      color: #b8005c;
      font-family: 'Sriracha', cursive, 'Kanit', sans-serif;
      font-size: 1em;
      text-align: left;
      line-height: 2;
      box-shadow: 0 2px 12px #ffb3c070;
      margin: 0 auto;
      max-width: 410px;
    }
    .next-anniv-section {
      margin: 1.2em 0 2em 0;
      background: linear-gradient(120deg, #ffe6e6 80%, #fffbe7 100%);
      border-radius: 22px;
      box-shadow: 0 4px 18px #e2555520;
      padding: 1em 1em 1.4em 1em;
      max-width: 480px;
      width: 98vw;
      border: 2px solid #f9a6c3b8;
      position: relative;
      z-index: 2;
      text-align: center;
    }
    .next-anniv-title {
      font-size: 1.1em;
      font-weight: bold;
      color: #b8005c;
      margin-bottom: 0.7em;
      letter-spacing: 1.2px;
      font-family: 'Kanit', sans-serif;
      text-align: center;
    }
    .next-anniv-value {
      font-size: 1.2em;
      font-weight: 600;
      color: #eb3c74;
      letter-spacing: 1px;
      text-shadow: 0 2px 8px #ffd6e2a0;
    }
    .decorative-flowers {
      width: 100%;
      display: flex;
      justify-content: space-between;
      position: absolute;
      left: 0;
      top: -32px;
      z-index: 0;
      pointer-events: none;
    }
    .flower {
      width: 52px;
      height: 52px;
      opacity: 0.9;
    }
    @media (max-width: 600px) {
      .header { font-size: 1.35rem; }
      .main-card { padding: 1.1em 0.2em 1em 0.2em; }
      .days-value { font-size: 1.1em; }
      .days-label { font-size: 1em; }
      .days-box { padding: 0.7em 0.7em; }
      .message-box { padding: 1em 0.5em; font-size: 0.97em;}
      .video-section, .next-anniv-section { padding: 0.8em 0.4em 1em 0.4em; }
      .flower { width: 32px; height: 32px;}
      .video-msg { font-size: 0.95em; }
    }
  </style>
</head>
<body>
  <canvas id="confetti" class="confetti"></canvas>
  <div class="header">
    Happy Anniversary 1 year
    <span class="heart">♥</span>
  </div>
  <!-- วิดีโอความทรงจำ + ข้อความในกรอบ -->
  <div class="video-section">
    <div class="video-title">วิดีโอความทรงจำของเรา</div>
    <div class="video-embed">
      <!-- ใส่ไฟล์วิดีโอของคุณเอง เช่น mymemory.mp4 ในโฟลเดอร์เดียวกับไฟล์นี้ -->
      <video id="memoryvideo" width="320" height="180" controls loop>
        <source src="mymemory.mp4" type="video/mp4">
        วิดีโอนี้ไม่สามารถเล่นได้ในเบราว์เซอร์ของคุณ
      </video>
    </div>
    <div class="video-msg">
      ความทรงจำในทุกช่วงเวลาที่เราได้ใช้ร่วมกัน  
      ไม่ว่าจะเป็นเสียงหัวเราะ รอยยิ้ม หรือแม้แต่วันธรรมดาที่มีอ้วนอยู่ข้าง ๆ  
      ทุกวินาทีล้วนมีความหมายและเติมเต็มหัวใจของเค้าเสมอ  
      ขอบคุณที่เป็นแรงบันดาลใจ เป็นความสุข และเป็นคนสำคัญของกันและกัน  
      ขอให้วิดีโอนี้เตือนความรู้สึกดี ๆ และพาเรายิ้มไปด้วยกันในทุกวันนะ
    </div>
  </div>
  <!-- ฟีเจอร์ 3: นับถอยหลังสู่วันครบรอบถัดไป -->
  <div class="next-anniv-section">
    <div class="next-anniv-title">เวลานับถอยหลังสู่วันครบรอบปีถัดไป</div>
    <div class="next-anniv-value" id="next-anniv-countdown"></div>
  </div>
  <div class="main-card">
    <div class="decorative-flowers">
      <img src="https://img.icons8.com/color/96/000000/flower.png" class="flower" style="transform: rotate(-15deg);" alt="">
      <img src="https://img.icons8.com/color/96/000000/flower-doodle.png" class="flower" style="transform: rotate(14deg);" alt="">
    </div>
    <div class="days-box">
      <div class="days-label">
        เราได้เดินทางร่วมกันมาแล้ว
        <span class="sparkle">✨</span>
      </div>
      <div id="anniversary-msg" class="days-value"></div>
    </div>
    <div class="message-box" id="love-msg">
      <div>ตลอดระยะเวลาที่เราได้เดินทางเคียงข้างกัน ทุกวันของฉันเต็มไปด้วยความหมายและความสุขที่ได้รับจากเธอ</div>
      <div>ขอบคุณสำหรับทุกกำลังใจในวันที่เหนื่อยล้า สำหรับรอยยิ้มในวันที่เศร้า และสำหรับเสียงหัวเราะที่เราได้แบ่งปันกัน</div>
      <div>แม้บางครั้งเส้นทางข้างหน้าอาจไม่ง่าย เราก็ยังจับมือกันแน่นและก้าวผ่านทุกเรื่องราวไปด้วยกัน</div>
      <div>การมีอ้วนอยู่ข้าง ๆ ทำให้ทุกเช้าวันใหม่ของฉันสดใส และทุกค่ำคืนเต็มไปด้วยความอบอุ่นใจ</div>
      <div>เค้าซาบซึ้งกับความเข้าใจ ความใส่ใจ และคำปลอบโยนในวันที่เค้าต้องการ</div>
      <div>ขอบคุณที่เป็นแฟน และแรงบันดาลใจของเค้า</div>
      <div>เค้าจะดูแลหัวใจของเราให้ดีที่สุด จะเป็นกำลังใจและอยู่ข้าง ๆ กันในทุก ๆ วัน ไม่ว่าฝนจะตกหรือแดดจะออก</div>
      <div>ขอบคุณที่ทำให้ฉันได้รู้ว่าความรักที่แท้จริงนั้นสวยงามเพียงใด</div>
      <div>ขอให้เรายิ้ม หัวเราะ และสร้างความทรงจำดี ๆ ด้วยกันไปตลอด</div>
      <div>ไม่ว่าทุกข์หรือสุข ขอให้หัวใจเรายังคงเต้นจังหวะเดียวกัน</div>
      <div>รักเธอสุดหัวใจ รักมากขึ้นทุกวินาทีของวันเวลาที่เราได้ใช้ร่วมกัน ♥</div>
      <div style="text-align:right;margin-top:0.4em;">Happy Anniversary, my love.<br>ขอให้ปีต่อ ๆ ไป มีแต่รอยยิ้ม ความสุข และรักมั่นคงแบบนี้ตลอดไป</div>
    </div>
  </div>
  <script>
    // ตั้งวันครบรอบ (17 พ.ค. 2567 = 2024-05-17)
    const anniversaryStart = new Date('2024-05-17T00:00:00');
    function updateAnniversary() {
      const now = new Date();
      let diffMs = now - anniversaryStart;

      if (diffMs < 0) {
        document.getElementById('anniversary-msg').innerHTML =
          'รออีกนิดนะ วันครบรอบของเราจะเริ่มในไม่ช้า ♥';
        return;
      }

      // คำนวณวัน ชม. นาที วินาที
      const days = Math.floor(diffMs / (1000 * 60 * 60 * 24));
      diffMs -= days * (1000 * 60 * 60 * 24);

      const hours = Math.floor(diffMs / (1000 * 60 * 60));
      diffMs -= hours * (1000 * 60 * 60);

      const minutes = Math.floor(diffMs / (1000 * 60));
      diffMs -= minutes * (1000 * 60);

      const seconds = Math.floor(diffMs / 1000);

      document.getElementById('anniversary-msg').innerHTML =
        `<span>${days}</span> วัน <span>${hours}</span> ชั่วโมง <span>${minutes}</span> นาที <span>${seconds}</span> วินาที`;
    }
    updateAnniversary();
    setInterval(updateAnniversary, 1000);

    // นับถอยหลังสู่วันครบรอบถัดไป
    function updateNextAnnivCountdown() {
      const now = new Date();
      let nextYear = anniversaryStart.getFullYear() + Math.floor((now - anniversaryStart)/(365.25*24*60*60*1000)) + 1;
      let nextAnniv = new Date(anniversaryStart);
      nextAnniv.setFullYear(nextYear);

      let diffMs = nextAnniv - now;
      if (diffMs < 0) {
        document.getElementById('next-anniv-countdown').innerHTML = 'สุขสันต์วันครบรอบปีนี้!';
        return;
      }
      const days = Math.floor(diffMs / (1000 * 60 * 60 * 24));
      diffMs -= days * (1000 * 60 * 60 * 24);
      const hours = Math.floor(diffMs / (1000 * 60 * 60));
      diffMs -= hours * (1000 * 60 * 60);
      const minutes = Math.floor(diffMs / (1000 * 60));
      diffMs -= minutes * (1000 * 60);
      const seconds = Math.floor(diffMs / 1000);

      document.getElementById('next-anniv-countdown').innerHTML =
        `<span>${days}</span> วัน <span>${hours}</span> ชั่วโมง <span>${minutes}</span> นาที <span>${seconds}</span> วินาที`;
    }
    updateNextAnnivCountdown();
    setInterval(updateNextAnnivCountdown, 1000);

    // Confetti Effect (ลดจำนวนพรุ)
    (() => {
      const confetti = document.getElementById('confetti');
      if(!confetti) return;
      const ctx = confetti.getContext('2d');
      let W = window.innerWidth, H = window.innerHeight;
      confetti.width = W;
      confetti.height = H;
      let mp = 40; //ลดจำนวนพรุ
      let particles = [];
      for(let i = 0; i < mp; i++) {
        particles.push({
          x: Math.random()*W,
          y: Math.random()*H,
          r: Math.random()*7+3,
          d: Math.random()*mp,
          color: `rgba(${Math.floor(Math.random()*255)},${Math.floor(Math.random()*180+75)},${Math.floor(Math.random()*255)},0.7)`,
          tilt: Math.floor(Math.random()*10)-10,
          tiltAngleIncremental: (Math.random()*0.07)+.05,
          tiltAngle: 0
        });
      }
      function draw() {
        ctx.clearRect(0, 0, W, H);
        for(let i = 0; i < mp; i++) {
          let p = particles[i];
          ctx.beginPath();
          ctx.lineWidth = p.r;
          ctx.strokeStyle = p.color;
          ctx.moveTo(p.x + p.tilt + (p.r/3), p.y);
          ctx.lineTo(p.x + p.tilt, p.y + p.tilt + (p.r/5));
          ctx.stroke();
        }
        update();
      }
      function update() {
        for(let i = 0; i < mp; i++) {
          let p = particles[i];
          p.y += (Math.cos(p.d)+3 + p.r/2)/2;
          p.x += Math.sin(0.2) * 2;
          p.tiltAngle += p.tiltAngleIncremental;
          p.tilt = Math.sin(p.tiltAngle- (i%3)) * 13;
          if(p.y > H){
            p.x = Math.random()*W;
            p.y = -10;
          }
        }
      }
      setInterval(draw, 34);
      window.addEventListener('resize', function() {
        W = window.innerWidth;
        H = window.innerHeight;
        confetti.width = W;
        confetti.height = H;
      });
    })();
  </script>
</body>
</html>
