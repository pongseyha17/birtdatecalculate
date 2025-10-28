<?php
// birthdate_calculator.php
date_default_timezone_set('Asia/Phnom_Penh');

$result = "";
if ($_SERVER["REQUEST_METHOD"] === "POST") {
    $birthdate = $_POST['birthdate'] ?? '';

    if ($birthdate) {
        $birth = new DateTime($birthdate);
        $today = new DateTime();
        $age = $today->diff($birth)->y;

        // Calculate next birthday
        $nextBirthday = new DateTime($birth->format('m-d'));
        $nextBirthday->setDate($today->format('Y'), $birth->format('m'), $birth->format('d'));

        if ($nextBirthday < $today) {
            $nextBirthday->modify('+1 year');
        }

        $daysLeft = $today->diff($nextBirthday)->days;

        $result = "
            <div style='margin-top:20px;'>
                <strong>You are:</strong> $age years old.<br>
                <strong>Next birthday:</strong> " . $nextBirthday->format('l, d M Y') . "<br>
                <strong>Days left:</strong> $daysLeft day(s)
            </div>
        ";
    } else {
        $result = "<div style='color:red;'>Please select your birthdate.</div>";
    }
}
?>

<!doctype html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>Birthdate Calculator</title>
<style>
    body {
        font-family: Arial, sans-serif;
        background: linear-gradient(180deg, #0f1724, #050c16);
        color: #fff;
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100vh;
        margin: 0;
    }
    .container {
        background: rgba(255,255,255,0.05);
        padding: 20px 30px;
        border-radius: 10px;
        box-shadow: 0 5px 20px rgba(0,0,0,0.5);
        text-align: center;
        width: 300px;
    }
    input[type="date"] {
        width: 100%;
        padding: 10px;
        border-radius: 8px;
        border: none;
        outline: none;
        font-size: 16px;
        margin-top: 10px;
    }
    button {
        margin-top: 15px;
        padding: 10px 15px;
        border: none;
        border-radius: 8px;
        background-color: #06b6d4;
        color: white;
        font-size: 16px;
        cursor: pointer;
    }
    button:hover {
        background-color: #0891b2;
    }
</style>
</head>
<body>
<div class="container">
    <h2>🎂 Birthdate Calculator</h2>
    <form method="POST">
        <input type="date" name="birthdate" required>
        <br>
        <button type="submit">Calculate</button>
    </form>
    <?php echo $result; ?>
</div>
</body>
</html>
