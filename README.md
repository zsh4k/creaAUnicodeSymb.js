# creaAUnicodeSymb.js

Crear Array de Simbolos Unicode

Este es un pequeño código en JavaScript que genera un array de caracteres Unicode a partir de un carácter inicial y una longitud dada.

## Código

```javascript
const creaAUnicodeSymb = (caracterI, length) => {
    return Array.from({ length }, (_, index) => String.fromCharCode(caracterI.charCodeAt() + index));
};
```

## Modos de uso

```javascript
let letras = creaAUnicodeSymb("A", 26);
console.log(letras);
```
Output
[
    "A",
    "B",
    "C",
    "D",
    "E",
    "F",
    "G",
    "H",
    "I",
    "J",
    "K",
    "L",
    "M",
    "N",
    "O",
    "P",
    "Q",
    "R",
    "S",
    "T",
    "U",
    "V",
    "W",
    "X",
    "Y",
    "Z"
]

```javascript
let numeros = creaAUnicodeSymb("0", 10);
console.log(numeros);
```

Output
[
    "0",
    "1",
    "2",
    "3",
    "4",
    "5",
    "6",
    "7",
    "8",
    "9"
]

```javascript
let letrasRusas = creaAUnicodeSymb("А", 32);
console.log(letrasRusas);
```

Output
[
    "А",
    "Б",
    "В",
    "Г",
    "Д",
    "Е",
    "Ж",
    "З",
    "И",
    "Й",
    "К",
    "Л",
    "М",
    "Н",
    "О",
    "П",
    "Р",
    "С",
    "Т",
    "У",
    "Ф",
    "Х",
    "Ц",
    "Ч",
    "Ш",
    "Щ",
    "Ъ",
    "Ы",
    "Ь",
    "Э",
    "Ю",
    "Я"
]
