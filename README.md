# Contador Zoneless en Angular

Aplicación sencilla de contador con Angular y Signals. La detección de cambios se configura con `provideZonelessChangeDetection()`.

## Requisitos
- Node.js compatible con Angular CLI 20
- npm

## Ejecutar
En la carpeta del proyecto:

```bash
npm install
npm start
```

Abre la dirección que indique Angular CLI (normalmente http://localhost:4200).

## Compilar
```bash
npm run build
```

## Funcionalidad
- `+`: incrementa el contador.
- `−`: disminuye el contador.
- `Reiniciar contador`: vuelve a cero.

## Conceptos
- **Zoneless:** Angular no depende de Zone.js para programar la detección de cambios.
- **Signals:** `signal()` crea un estado reactivo; `update()` lo modifica y `set()` establece un valor.

**Nota:** este proyecto demuestra Zoneless y Signals. No configura SSR ni hidratación incremental. Para demostrar hidratación incremental habría que añadir renderizado del lado del servidor y configurar `@defer` con las opciones de hidratación correspondientes.
