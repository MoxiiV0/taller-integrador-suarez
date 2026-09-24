# Taller Integrador — Buenas Prácticas de Desarrollo de Software

**Nombre completo:** Santiago Alberto Suarez Escamilla
**Grupo:** 25493

Este repositorio contiene la auditoría y corrección de una calculadora de
promedio de tres notas, siguiendo las buenas prácticas de nomenclatura,
limpieza de código y control de versiones vistas en el curso.

## Tabla de hallazgos de la auditoría

| # | Defecto encontrado | Por qué era un problema | Cómo lo corregí |
|---|---|---|---|
| 1 | Nombre de archivo `Mi Pagina De Notas.HTML` | Espacios, mayúsculas mezcladas y extensión en mayúscula; rompe convenciones y complica rutas | Renombrado a `index.html` |
| 2 | Nombre de archivo `Estilos Del Sitio.CSS` | Mismo problema que el anterior | Renombrado a `styles.css` |
| 3 | Variable `x = 3` | Nombre no describe qué representa; valor mágico sin significado | Renombrada a `CANTIDAD_NOTAS` y declarada como `const` |
| 4 | Variables `a`, `b`, `c` | No indican qué almacenan; obligan a leer todo el código para entenderlo | Renombradas a `nota1`, `nota2`, `nota3` |
| 5 | Variable `TempValue2` | Nombre sin significado, mezcla de convenciones, sufijo numérico arbitrario | Renombrada a `promedio` |
| 6 | Variable `data1 = []` | Se declaraba pero nunca se usaba en el código | Eliminada |
| 7 | Función `calc()` | El nombre no describe la acción que realiza | Renombrada a `calcularPromedio()` |
| 8 | IDs HTML `n1`, `n2`, `n3`, `r`, `r2` | No describen su contenido ni su propósito | Renombrados a nombres descriptivos |
| 9 | `<title>pagina</title>` | No describía el contenido en la pestaña del navegador | Cambiado a `Calculadora de Promedio` |
| 10 | Llamados `console.log(...)` | Código de depuración olvidado, sin función para el usuario final | Eliminados |
| 11 | Bloque comentado `calcularAntiguo` | Código muerto sin uso, ensuciaba el archivo | Eliminado |

## Sitio publicado

 https://resplendent-kashata-9e6408.netlify.app/


# Calculadora de Promedio

Página web simple para calcular el promedio de tres notas y determinar si el estudiante aprueba o reprueba (promedio ≥ 3.0).

## Funcionalidad

- Ingreso de tres notas (valores numéricos con un decimal)
- Cálculo automático del promedio
- Resultado: "Aprobado" si el promedio es ≥ 3.0, "Reprobado" en caso contrario

## Tecnologías

- HTML5
- CSS3
- JavaScript (vanilla)

## Estructura del proyecto

```
.
├── index.html      # Página principal
├── styles.css      # Estilos
└── README.md       # Este archivo
```

## Uso

1. Abre `index.html` en un navegador
2. Ingresa las tres notas
3. Haz clic en "Calcular"

## Despliegue

El sitio está desplegado en Netlify desde la rama `main`.
