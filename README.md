<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Thư Tình Dành Tặng Vợ</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      text-align: center;
      padding: 2rem;
      background: #ffe6e6;
      color: #333;
    }
    h1 {
      color: #d6336c;
    }
    .message {
      white-space: pre-line;
      font-size: 1.2rem;
      margin: 1rem 0 2rem;
    }
    button {
      background-color: #d6336c;
      color: white;
      border: none;
      padding: 1rem 2rem;
      font-size: 1.1rem;
      border-radius: 8px;
      cursor: pointer;
      transition: background-color 0.3s;
    }
    button:hover {
      background-color: #b82e58;
    }
  </style>
</head>
<body>
  <h1>Thư Tình Gửi Vợ Hoàng Nhật</h1>
  <div class="message">
    Chúc Vợ muộn ngày 1/6 vui vẻ nhée.<br/>
    Anh yêu vợ nhiều lắm luôn áa.<br/>
    Vợ Hoàng Nhật mãi mãi luôn bên cạnh anh nhée.
  </div>
  
  <button id="toggle-music">Phát Nhạc</button>

  <audio id="bg-music" loop>
    <source src="https://drive.google.com/uc?export=download&id=10teOWHganeLlzjnAfrww7-ymE5iH4E73" type="audio/mpeg" />
    Trình duyệt không hỗ trợ phát nhạc.
  </audio>

  <script>
    const music = document.getElementById('bg-music');
    const btn = document.getElementById('toggle-music');
    let playing = false;

    btn.addEventListener('click', () => {
      if (playing) {
        music.pause();
        btn.textContent = 'Phát Nhạc';
      } else {
        music.play();
        btn.textContent = 'Tạm Dừng Nhạc';
      }
      playing = !playing;
    });
  </script>
</body>
</html>
