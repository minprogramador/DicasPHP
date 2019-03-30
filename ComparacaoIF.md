
# Exemplos de boas e más comparações:

### Operadores de Comparação

>Operadores de comparação, como os seus nomes implicam, permitem que você
compare dois valores.

>Você pode se interessar em ver as tabelas de comparação
de tipos, que tem exemplo das várias comparações entre tipos relacionadas.`

-----------------------------------------------------------------------------
| Exemplo     | Resultado   												                        |
| :-----------|------------------------------------------------------------:|
| $a == $b	  | Igual	Verdadeiro (TRUE) se $a é igual a $b. 				        |
| $a === $b	  | Idêntico	Verdadeiro (TRUE) se $a é igual a $b. 			      |
| $a != $b	  | Diferente	Verdadeiro se $a não é igual a $b. 				        |
| $a <> $b	  | Diferente	Verdadeiro se $a não é igual a $b. 				        |
| $a !== $b	  | Não idêntico	Verdadeiro de $a não é igual a $b. 			      |
| $a < $b     | Menor que	Verdadeiro se $a é estritamente menor que $b. 	  |
| $a > $b     | Maior que	Verdadeiro se $a é estritamente maior que $b. 	  |
| $a <= $b	  | Menor ou igual	Verdadeiro se $a é menor ou igual a $b. 	  |
| $a >= $b	  | Maior ou igual	Verdadeiro se $a é maior ou igual a $b. 	  |
| $a <=> $b	  | Spaceship Um integer menor que, igual a ou maior que zero.	|
-----------------------------------------------------------------------------

# #Comparar strings if/else
  
## - Mal uso
>Verifica se `var` é igual a `false`, e se `var2` é diferente de `algo`.
  
```php
if ($var == false && $var2 != 'algo')
```
  
-----------------------------------------------
  
## + Bom uso
>Verifica se `var` é igual a `false` e se `var2` é diferente de `algo`.
  
```php
if ($var == false and $var2 != 'algo')
```

-----------------------------------------------

## - Mal uso
>Verifica se `var` existe ?/!.

```php
if ($template)
```

-----------------------------------------------

## + Bom uso
>Verifica se `var` existe ?/!.

```php
if (isset($template))
if ($template !== NULL)
if ($template !== '')
```

-----------------------------------------------

## - Mal uso
>Verifica se tem mais que `0 caracteres`.

```php
if (strlen($template) > 0)
```

## + Bom uso
>Verifica se é `string`, e se tem mais que `0 caracteres`.

```php
if (is_string($template) && strlen($template) > 0)
```

-----------------------------------------------

## - Mal uso
>Comparar `vars`, `evitar, comparaçōes verdadeiras!`.

```php
if ($foo == $bar)
if ($foo != $bar)
```

-----------------------------------------------

## + Bom uso
>Comparar `vars`, `evitar, comparaçōes verdadeiras !`.

```php
if ($foo === $bar)
if ($foo !== $bar)
```

*to be continue...*
