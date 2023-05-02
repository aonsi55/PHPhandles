# PHPhandles


I am making this lazy code for creating multiple files with the name Assignment$i.php =)) , such that each files having the same php opening tag at the first line, as the following I wanted to make 8 files from 1 to 8, the code is as follows, 


# Code


```
<?php

for ($i=1; $i<=8; $i++) {
    $file = fopen("Assignment$i.php", "w");
    $txt = "<?php\n\n";
    fwrite($file, $txt);
    fclose($file);
}

?>
