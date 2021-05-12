<?php
session_start();
$_SESSION['sessionid'] = hash('sha256', 'pass');
?>

<form method="post" action="<?php echo $_SERVER['PHP_SELF']; ?>">
username: <input type="text" name="user">
password: <input type="password" name="pass">
<input type="submit" value="Log in">
</form>

<?php
$db = mysqli_connect("localhost", "root", "JanMan1#", "demonstration") or die(mysqli_error());
$q = "select userid from users where username = '".addslashes($_POST['user']). "' and password = '".hash('sha256', $_POST['pass'])."'";
$res = mysqli_query($db, $q);
if ($res)
{
	if (mysqli_num_rows($res) == 1)
	{
		$row = mysqli_fetch_assoc($res);
		$sessionid = hash('sha256', time().$row['userid']);
		$q = "insert into sessions (userid, sessionid, sessiontime) values (".$row['userid'].", '$sessionid', unix_timestamp())";
		$res = mysqli_query($db, $q);
		$_SESSION['sessionid'] = $sessionid;
	}
}
mysqli_close($db);
?>

<a href="test.php">test</a>