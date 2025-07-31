# Conteúdo de Javascript

```javascript
const pessoas = [
  { nome: 'Ana', idade: 20 },
  { nome: 'Maria', idade: 16 },
  { nome: 'João', idade: 30 }
];

// ["Ana", "Maria", "João"]
console.log("Nomes das pessoas", pessoas.map(p => p.nome));

// ["Ana", "João"]
console.log("Nomes dos maiores de idade", pessoas.filter(p => p.idade >= 18).map(p => p.nome));

console.log("Quantidade de caracteres por nome:");
var cfunction = pessoas.map(function(s){ return s.nome.length });
var afunction = pessoas.map( s => s.nome.length );

console.log(cfunction); // [3, 5, 4]
console.log(afunction); // [3, 5, 4]
```

<!-- 
Haskell my beloved, who makes you suffer so much?
-->