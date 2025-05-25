<!DOCTYPE html>
<html>
<head>
  <title>Login - Hotspot</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <style>
    body {
      margin: 0;
      padding: 0;
      background: url('background.jpg') no-repeat center center fixed;
      background-size: cover;
      font-family: 'Segoe UI', sans-serif;
      display: flex;
      align-items: center;
      justify-content: center;
      height: 100vh;
    }
    .login-box {
      background: rgba(0, 0, 0, 0.7);
      padding: 30px 20px;
      border-radius: 12px;
      color: #fff;
      width: 90%;
      max-width: 350px;
      text-align: center;
    }
    .login-box img {
      width: 80px;
      margin-bottom: 15px;
    }
    .login-box h2 {
      margin-bottom: 20px;
      font-size: 22px;
    }
    .login-box input[type="text"],
    .login-box input[type="password"] {
      width: 100%;
      padding: 12px;
      margin: 10px 0;
      border: none;
      border-radius: 6px;
    }
    .login-box input[type="submit"] {
      width: 100%;
      background: #3498db;
      border: none;
      padding: 12px;
      color: white;
      font-size: 16px;
      border-radius: 6px;
      cursor: pointer;
    }
    .login-box input[type="submit"]:hover {
      background: #2980b9;
    }
    .footer {
      margin-top: 15px;
      font-size: 12px;
      opacity: 0.6;
    }
  </style>
</head>
<body>

  <div class="login-box">
    <img src="logo.png" alt="Logo">
    <h2>Welcome to Free Wi-Fi</h2>
    <form name="login" action="$(link-login-only)" method="post">
      <input type="hidden" name="dst" value="$(link-orig)" />
      <input type="hidden" name="popup" value="true" />
      <input type="text" name="username" placeholder="Username" />
      <input type="password" name="password" placeholder="Password" />
      <input type="submit" value="Log In" />
    </form>
    <div class="footer">Powered by MikroTik</div>
  </div>

</body>
</html>
