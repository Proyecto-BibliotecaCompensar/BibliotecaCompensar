# Casos de prueba

Probados por: Cristian Vargas · Fecha: 21/10/2026

Entorno: Opera GX con Live Server (rama develop) y GitHub Pages (rama main, versión 1.0.0).

| # | Caso | Cómo se prueba | Resultado esperado | Resultado |
|---|---|---|---|---|
| 1 | La página carga | Abrir index.html con Live Server | Se ve el nombre del proyecto, sin mensajes en rojo | Pasa |
| 2 | Datos del proyecto | Revisar el encabezado | Nombre, descripción y versión coinciden con datos/equipo.json | Pasa |
| 3 | Integrantes completos | Contar las tarjetas | Hay una tarjeta por cada integrante del README | Pasa |
| 4 | Enlaces a GitHub | Clic en cada @usuario | Abre el perfil correcto | Pasa (después de corregir #9) |
| 5 | JSON válido | Abrir datos/equipo.json en VS Code | VS Code no marca errores en rojo | Pasa |
| 6 | Vista en celular | F12 > modo dispositivo móvil | Las tarjetas se acomodan en una columna | Pasa (probado a 396 px) |
| 7 | Página publicada | Abrir la URL de GitHub Pages | Se ve igual que en Live Server | Pasa |

Página publicada: https://proyecto-bibliotecacompensar.github.io/BibliotecaCompensar/

## Errores encontrados

| Issue | Problema | Corrección | Estado |
|---|---|---|---|
| #9 | Tres usuarios de GitHub mal escritos en datos/equipo.json (And119, zoebalagay, micha7128) daban error 404 | PR #11 | Corregido y verificado |
| #10 | El título de la pestaña decía "Biblioteca Johana" | PR #12 | Corregido y verificado |

Si un caso falla: abrir un Issue con la etiqueta `bug`, explicar qué pasó y asignarlo a quien corresponda.