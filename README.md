# to-nhi
<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8">
  <title>Gửi Nguyễn Đan Nhi 💖</title>
  <style>
    body {
      background: linear-gradient(135deg, #ffd6ec, #ffeaea);
      font-family: 'Segoe UI', sans-serif;
      text-align: center;
      padding: 50px;
      overflow: hidden;
    }

    h1 {
      font-size: 2em;
      color: #d63384;
      margin-bottom: 40px;
    }

    .typewriter {
      display: inline-block;
      color: #333;
      font-size: 1.2em;
      border-right: 2px solid #000;
      white-space: nowrap;
      overflow: hidden;
      width: 0;
      animation: typing 8s steps(100, end) forwards, blink 0.75s step-end infinite;
    }

    @keyframes typing {
      from { width: 0; }
      to { width: 100%; }
    }

    @keyframes blink {
      50% { border-color: transparent; }
    }

    .heart {
      position: absolute;
      width: 20px;
      height: 20px;
      background-color: pink;
      transform: rotate(45deg);
      animation: float 6s linear infinite;
    }

    .heart::before, .heart::after {
      content: '';
      position: absolute;
      width: 20px;
      height: 20px;
      background-color: pink;
      border-radius: 50%;
    }

    .heart::before {
      top: -10px;
      left: 0;
    }

    .heart::after {
      left: -10px;
      top: 0;
    }

    @keyframes float {
      0% {
        bottom: 0;
        opacity: 1;
      }
      100% {
        bottom: 100%;
        opacity: 0;
      }
    }
  </style>
</head>
<body>
  <h1>Gửi Nguyễn Đan Nhi 💌</h1>

  <div class="typewriter">
    Anh xin lỗi vì đã không nói rõ ràng với em từ đầu. Anh không muốn em phải thấy lăn tăn hay không chắc chắn trong chuyện của tụi mình. Anh cứ nghĩ là mình ở cạnh nhau, quan tâm nhau từng chút một là đủ để em hiểu anh nghiêm túc. Nhưng anh sai khi không nói điều đó rõ ràng với em. Vậy thì hôm nay anh sẽ làm anh chưa từng nhưng mà đáng lẽ phải nói với em từ lâu: Là anh yêu em và em hãy là người anh yêu từ nay về sau nhé.
  </div>

  <!-- Nhạc nền (bật nếu cần) -->
  <!--
  <audio autoplay loop>
    <source src="your-music.mp3" type="audio/mpeg">
    Trình duyệt không hỗ trợ nhạc nền.
  </audio>
  -->

  <script>
    // Hiệu ứng tim bay
    setInterval(() => {
      const heart = document.createElement('div');
      heart.classList.add('heart');
      heart.style.left = Math.random() * 100 + 'vw';
      heart.style.animationDuration = 5 + Math.random() * 3 + 's';
      document.body.appendChild(heart);
      setTimeout(() => heart.remove(), 8000);
    }, 300);
  </script>
</body>
</html>
