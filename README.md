<script>
let password = prompt("введите пароль");

if (password !=="1234") {document.body.innerHTML = ""; alert("НЕ ДОСТУПНО");
}
</script>

<h1>SECRET SITE</h1>
<p>ОПЛАТА ЗДЕСЬ</p>

<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <title>ОПЛАТА ДОСТУПНА</title>

  <style>
    body {
      font-family: Arial;
      background: #0f0f0f;
      color: white;
      text-align: center;
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
      background: #00c853;
      color: white;
      font-size: 16px;
    }

    .code {
      margin-top: 20px;
      font-size: 18px;
      color: #00e5ff;
    }
  </style>
</head>

<body>

<script>
let password = prompt("Введите пароль");

if (password !== "1234") {
  alert("НЕ ДОСТУПНО");
  document.body.innerHTML = "";
}
</script>

<h1>SECRET SITE</h1>
<p>ОПЛАТА ЗДЕСЬ</p>

<div class="box">
  <h2>Доступ к сайту</h2>
  <p>Цена: 25000 ₸</p>

  <button onclick="pay()">ОПЛАТИТЬ</button>

  <div id="access" class="code"></div>
</div>

<script>
function pay() {
  window.open("https://kaspi.kz", "_blank");

  setTimeout(() => {
    document.getElementById("access").innerHTML =
      "Ваш код доступа: M12";
  }, 3000);
}
</script>

</body>
</html>
