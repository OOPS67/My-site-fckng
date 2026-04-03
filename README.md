<script>
let password = prompt("введите пароль");

if (password !=="1234") {document.body.innerHTML = ""; alert("НЕ ДОСТУПНО");
}
</script>

<h1>SECRET SITE</h1>
<p>ОПЛАТА ЗДЕСЬ</p>


</body>
< ! DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <title>ОПЛАТА ДОСТУПНА</title>
  <style>
    body {
      font-family: Arial;
      background: #0f0f0f
      color: white;
      text-alight: centre;
      padding-top: 80px;
    }
    .box {
      background: #1c1c1c;
      padding: 20px;
      border-radius: 12px;
      width: 300px;
      margin: auto;
    }
    button {
      padding: 12px;
      width: 100%;
      margin-top: 10px;
      border: none;
      border-radius: 8px;
      background: 00c853;
      color: white;
      font-size: 16px;
    }
    .code {
      margin-top: 20px;
      font-size: 18px;
      color: 00e5ff;
    }
  </style>
</head>

<body>

<div class="box">
  <h2>Доступ к сайту</h2>
  <p>Цена: 25000</p>
  
  <!-- КНОПКА ОПЛАТЫ -->
  <button onclick="pay()">ОПЛАТИТЬ</button>
  
  <!-- ПОСЛЕ ОПЛАТЫ -->
  <div id="access" class="code"></div>
  </div>
  
  <script>
  function pay() {
    // пока делаем имитацию оплаты
    window.open("html://kaspi.kz", "_blank");
    
    setTimeout(() => {
           document.petElementById("access").innerHTML =
  "Ваш код доступа: M12";
 }, 3000);
}
</script>

</body>
</html>
