# Php-cia--2-program-
Practice programPalindrome Checker
<!DOCTYPE html>
<html>
<body>

<h2>Palindrome Checker</h2>

<form method="post">
    Enter Word / Username / Vehicle Number:
    <input type="text" name="text" required><br><br>

    <input type="submit" name="check" value="Check">
</form>

<?php
if (isset($_POST['check'])) {

    $text = $_POST['text'];
    $reverse = strrev($text);

    if ($text == $reverse) {
        echo "<h3>$text is a Palindrome</h3>";
    } else {
        echo "<h3>$text is Not a Palindrome</h3>";
    }
}
?>

</body>
</html>
Example Output:
Enter: MADAM

MADAM is a Palindrome
