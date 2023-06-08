```php
<?php

$nome = $_POST["nome"] ?? NULL;
$sql= "ex6";

$consulta = $_PDO-> prepare($sql);
$consulta -> execute();

$dados = $consulta->fetch(PDO::FETCH_OBJ);

?>