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
