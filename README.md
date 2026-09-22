# Tarjeta digital — Paola Andrea Criollo Gámez · Grupo Indufrial

Misma base que la tarjeta de Adrián, con tres diferencias: sin LinkedIn,
solo 5 catálogos, y el logo va **repujado** (grabado en la superficie) en
lugar de plano sobre el fondo azul.

## ⚠️ DOS ARCHIVOS QUE DEBES REEMPLAZAR ANTES DE PUBLICAR

Los que vienen en este paquete son **placeholders** — funcionan para que la
página no se rompa, pero no sirven para producción:

| Archivo | Qué hacer |
|---|---|
| `assets/img/logo-white.png` | **Copiar el real desde el repo de Adrián** (`vCard/assets/img/logo-white.png`). El que viene aquí es texto genérico, no el logo de Indufrial. |
| `assets/img/avatar.jpg` | Reemplazar por la foto de Paola. Cuadrada, mínimo 400×400 px, buena luz, fondo simple. |

## Estructura

```
/
├── index.html
├── style.css
├── assets/
│   ├── PaolaCriollo.vcf      ← contacto descargable
│   ├── img/
│   │   ├── logo-white.png    ← REEMPLAZAR (copiar del repo de Adrián)
│   │   └── avatar.jpg        ← REEMPLAZAR (foto de Paola)
│   └── catalogos/
│       ├── refrigeracion.pdf
│       ├── congelacion.pdf
│       ├── importados.pdf
│       ├── vending.pdf
│       ├── maquinas-cafe.pdf
│       └── one-pager-corporativo.pdf
```

## Catálogos — nombres exactos

Súbelos a `assets/catalogos/` con estos nombres (minúsculas, sin tildes,
sin espacios). Son los mismos archivos del repo de Adrián, así que puedes
descargarlos de allá y volverlos a subir aquí.

| Botón | Nombre del archivo |
|---|---|
| Refrigeración | `refrigeracion.pdf` |
| Congelación | `congelacion.pdf` |
| Importados | `importados.pdf` |
| Vending | `vending.pdf` |
| Máquinas de café | `maquinas-cafe.pdf` |
| Perfil corporativo | `one-pager-corporativo.pdf` |

**Ojo con la carpeta duplicada:** la ruta correcta es `assets/catalogos/`,
no `assets/catalogos/catalogos/`. Si al crear la carpeta ya estás dentro de
`assets`, escribe solo `catalogos/.gitkeep`, no `assets/catalogos/.gitkeep`.

## Sobre el logo repujado

El efecto está en `style.css`, clase `.identity__logo`. Se logra bajando la
opacidad del logo blanco y aplicando dos sombras: una oscura arriba (hueco)
y una clara abajo (relieve). Si lo quieres más o menos marcado, ajusta el
valor de `opacity` (actualmente `0.46`) — más bajo lo hace más sutil, más
alto lo hace más presente.

Este mismo bloque de CSS lo puedes copiar tal cual a la tarjeta de Adrián
cuando quieras aplicarle el mismo tratamiento.

## Publicación

Mismo proceso que la tarjeta de Adrián: repo nuevo en GitHub → subir los
archivos → Settings → Pages → Source: `main` / `(root)` → Save.

Recuerda que al subir archivos hay que **bajar hasta el final y darle clic
al botón verde "Commit changes"** — sin ese paso no se guarda nada.
