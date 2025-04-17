<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <title>Mau ngga jadi pacar aku?</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      margin-top: 100px;
    }
    h1 {
      font-size: 32px;
      margin-bottom: 40px;
    }
    button {
      padding: 15px 30px;
      font-size: 20px;
      margin: 20px;
      cursor: pointer;
      border: none;
      border-radius: 8px;
    }
    #mau {
      background-color: #4CAF50;
      color: white;
    }
    #tidak {
      background-color: #f44336;
      color: white;
      position: absolute;
    }
  </style>
</head>
<body>
  <h1>Mau ngga jadi pacar aku?</h1>
  <button id="mau" onclick="alert('Yay! Sekarang kamu jadi pacar aku!')">Mau</button>
  <button id="tidak">Tidak</button>

  <script>
    const btnTidak = document.getElementById('tidak');

    btnTidak.addEventListener('mouseover', () => {
      const x = Math.floor(Math.random() * (window.innerWidth - 100));
      const y = Math.floor(Math.random() * (window.innerHeight - 50));
      btnTidak.style.left = `${x}px`;
      btnTidak.style.top = `${y}px`;
    });
  </script>
</body>
</html>
