# Exemplo de Contador feito em React

Gestão de estados no React ( *State Management* )

```jsx
import { useState } from 'react'

export default function Contador({ numero = 0 }) {
  const [contador, setContador] = useState(numero)

  return (
      <div className="flex w-min border rounded-md">
      <button className="border-r font-mono hover:bg-gray-200" onClick={() => setContador(contador - 1)}>-</button>
      <span className="m-auto p-2">{contador}</span>
      <button className="border-l font-mono hover:bg-gray-200" onClick={() => setContador(contador + 1)}>+</button>
    </div>
  )
}
```

<!-- ./components/Counter.vue -->
<Counter :count="0" />

<!--
Este exemplo é só mesmo para inglês ver
-->