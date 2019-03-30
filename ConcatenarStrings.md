# #Concatenar strings.

## - Mal uso
> concatena strings de forma tradicional, com . seguido de espaço antes e depois.
  
```php
$mensagem = 'E ai ' . $nome . ', você ' . $aparencia . ' hoje!'; 
```
  
-----------------------
  
## + Bom uso
> concatena strings de forma legivel usando sprintf.
  
```php
$mensagem = sprintf('E ai %s, você parece %s hoje!', $nome, $aparencia);
```
