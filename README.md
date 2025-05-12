<!DOCTYPE html>
<html lang="zh-Hant">
<head>
  <meta charset="UTF-8">
  <title>密碼鎖</title>
</head>
<body>

<h2>請輸入密碼</h2>
<input type="password" id="passwordInput" placeholder="輸入密碼">
<button onclick="checkPassword()">解鎖</button>
<p id="messageBox" style="color: red;"></p>

<script>
  function checkPassword() {
    const input = document.getElementById("passwordInput").value;
    const correct = "1234";
    const message = document.getElementById("messageBox");

    if (input === correct) {
      window.location.href = "https://sites.google.com/view/summer-501-601";
    } else {
      message.textContent = "密碼錯誤，請再試一次。";
    }
  }
</script>

</body>
</html>
