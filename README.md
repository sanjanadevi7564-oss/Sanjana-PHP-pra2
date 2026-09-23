<!DOCTYPE html>
<html>
<head>
 <title>Palindrome Checker</title>
</head>
<body>
 <h2>Palindrome Checker</h2>
 <form method="post">
 <input type="text" name="inputString" placeholder="Enter a string" required>
 <button type="submit">Check</button>
 </form>
 <?php
 if (isset($_POST['inputString'])) {
 $inputString = $_POST['inputString'];
 $reversedString = strrev($inputString);
 if ($inputString == $reversedString) {
 echo "<p>$inputString is a palindrome.</p>";
 } else {
 echo "<p>$inputString is not a palindrome.</p>";
 }
 }
 ?>
</body>
</html>
OUTPUT
localhost/spal.php
Palindrome Checker
Enter a string
Check
raii is not a palindrome
localhost/spal.php
Palindrome Checker
madam
madam is a palindrome
Check
