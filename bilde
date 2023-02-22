<!DOCTYPE html>
<html>
<head>
	<title>Min bildedelingsside</title>
</head>
<body>

	<h1>Velkommen til min bildedelingsside!</h1>
	
	<p>På denne siden kan du laste opp og dele bilder med venner og familie.</p>
	
	<form action="upload.php" method="POST" enctype="multipart/form-data">
		<input type="file" name="fileToUpload" id="fileToUpload">
		<input type="submit" value="Last opp bilde" name="submit">
	</form>

	<div>
		<h2>Dine opplastede bilder:</h2>
		<?php
			$dir = "uploads/";
			$files = scandir($dir);
			foreach($files as $file) {
				if($file !== '.' && $file !== '..') {
					echo '<img src="' . $dir . $file . '" width="300px" height="300px">';
				}
			}
		?>
	</div>

</body>
</html>
