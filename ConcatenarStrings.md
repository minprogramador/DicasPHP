# #Concatenar strings.

## - Mal uso
> concatena strings de forma tradicional,com . seguido de espaço antes e depois.
  
```php
$mensagem = 'E ai ' . $nome . ', você ' . $aparencia . ' hoje!'; 
```
<br>

## + Bom uso
> concatena strings de forma legivel usando sprintf.

<br>

```php
$mensagem = sprintf('E ai %s, você parece %s hoje!', $nome, $aparencia);
```
