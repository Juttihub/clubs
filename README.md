# clubs
ระบบสมาชิกชมรม โรงเรียนเซนต์เมรี่
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>Login</title>
</head>
<body>
    <div class="login-container">
        <h2><img src="logo.png" alt="โลโก้" /> เข้าสู่ระบบ</h2>
        <form method="post" action="process_login.php">
            <label for="username">ชื่อผู้ใช้:</label>
            <input type="text" name="username" required><br><br>
            <label for="password">รหัสผ่าน:</label>
            <input type="password" name="password" required><br><br>
            <button type="submit">เข้าสู่ระบบ</button>
        </form>
        <?php
        if (isset($login_error)) {
            echo "<p style='color: red;'>$login_error</p>";
        }
        ?>
    </div>
</body>
</html>
