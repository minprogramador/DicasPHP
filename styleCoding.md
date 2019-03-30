# #Exemplos de boas e más comparações:
## #IF/ELSE
>Uma estrutura if se parece com o seguinte.

```php
if ($expr1) {
    // code
} elseif ($expr2) {
    // code
} else {
    // code
}
```

>Observe o posicionamento dos parênteses, espaços e chaves; e que else e elseif estão na mesma linha que a chave de fechamento do corpo anterior.

-------------------------------------------------------------------------------

>Expressões entre parênteses PODEM ser divididas em várias linhas, onde cada
linha subseqüente é recuada pelo menos uma vez.
Ao fazer isso, a primeira condição DEVE estar na próxima linha.

```php
if (
    $expr1
    && $expr2
) {
  // code
} elseif (
    $expr3
    && $expr4
) {
  // code
}
```

>O parêntese de fechamento e a chave de abertura DEVEM ser colocados juntos
em sua própria linha com um espaço entre eles. Os operadores booleanos entre
as condições DEVEM sempre estar no começo ou no final da linha, não uma mistura de ambos.

-------------------------------------------------------------------------------

## #Switch
>Uma estrutura de switch é semelhante à seguinte.

```php
switch ($expr) {
    case 0:
        echo 'Primeiro casa, com um parada';
        break;
    case 1:
        echo 'Segundo casa, sem parada';
        // no break
    case 2:
    case 3:
    case 4:
        echo 'Terceiro casa, retorna em vez de parar';
        return;
    default:
        echo 'Casa padrao';
        break;
}
```

>Ou em code style expressivo.

```php
switch (
    $expr1
    && $expr2
) {
    // code
}
```

## #While
>Observe o posicionamento dos parênteses, espaços e chaves.
A instrução de caso deve ser recuada uma vez de alternar e a palavra-chave de quebra (ou outras palavras-chave de terminação) devem ser recuados no mesmo nível como o corpo do caso.
Deve haver um comentário como // no break quando o fall-through é intencional em um corpo de caso não vazio.

```php
while ($expr) {
    // code
}

//Ou

while (
    $expr1
    && $expr2
) {
    // code
}
```

```php

do {
    // code
} while ($expr);

//ouu

do {
    // code
} while (
    $expr1
    && $expr2
);
```

## #For
```php

for ($i = 0; $i < 10; $i++) {
    // code
}

//OU expressivo..

for (
    $i = 0;
    $i < 10;
    $i++
) {
    // code
}

```

## #Foreach
```php

foreach ($iterable as $key => $value) {
    // foreach body
}

//ou expressivo..

foreach (
    $iterable as $key => $value
) {
    // foreach body
}

```

## #Try/Catch
```php
try {
    // try body
} catch (FirstThrowableType $e) {
    // catch body
} catch (OtherThrowableType $e) {
    // catch body
} finally {
    // finally body
}
```

-------------------------------------------------------------------------------

## #Closure

```php
$closureWithArgs = function ($arg1, $arg2) {
    // body
};

$closureWithArgsAndVars = function ($arg1, $arg2) use ($var1, $var2) {
    // body
};

$closureWithArgsVarsAndReturn = function ($arg1, $arg2) use ($var1, $var2): bool {
    // body
};

//Ou expressivo...

$longArgs_noVars = function (
    $longArgument,
    $longerArgument,
    $muchLongerArgument
) {
   // body
};

$noArgs_longVars = function () use (
    $longVar1,
    $longerVar2,
    $muchLongerVar3
) {
   // body
};

$longArgs_longVars = function (
    $longArgument,
    $longerArgument,
    $muchLongerArgument
) use (
    $longVar1,
    $longerVar2,
    $muchLongerVar3
) {
   // body
};

$longArgs_shortVars = function (
    $longArgument,
    $longerArgument,
    $muchLongerArgument
) use ($var1) {
   // body
};

$shortArgs_longVars = function ($arg) use (
    $longVar1,
    $longerVar2,
    $muchLongerVar3
) {
   // body
};

$foo->bar(
    $arg1,
    function ($arg2) use ($var1) {
        // body
    },
    $arg3
);
```

-------------------------------------------------------------------------------

### #Classe anonima.

```php
$instance = new class {};

// Brace on the same line
$instance = new class extends \Foo implements \HandleableInterface {
    // Class content
};

// Brace on the next line
$instance = new class extends \Foo implements
    \ArrayAccess,
    \Countable,
    \Serializable
{
    // Class content
};
```

-------------------------------------------------------------------------------
