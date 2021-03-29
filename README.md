# common-server
##### Simple Http Server redirected with send_me parameter .
##### if send_me parameter is true

``` php
<?php
if($_GET["send_me"] == true){
    header("Status: 301 Moved Permanently");
    header("Location: https://google.com?".$_SERVER['QUERY_STRING']); 
    exit;
    }
?>

```
save that script on your file e.g `redirect.php`
run the code as ...

``` sh

$ php -S localhost:3000 

```
