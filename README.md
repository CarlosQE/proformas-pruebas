# Proformas — versión de pruebas

**Descarga:** [última versión (zip para Windows)](https://github.com/CarlosQE/proformas-pruebas/releases/latest) → en *Assets*, `proformas-pruebas-…-windows-amd64.zip`.

Requisitos: Windows 10/11 de 64 bits y un navegador (Chrome o Edge). No requiere instalar nada ni conexión a internet.

Sirve para recorrer el sistema y opinar sobre la interfaz antes de instalarlo en la tienda.
Los datos son **ficticios** (empresas, clientes, productos y unas 30 proformas de los últimos dos meses)
y se guardan solo en esta PC, en la carpeta `datos-demo` junto al programa. Lo impreso lleva la marca
**PRUEBA** y no tiene validez.

## Abrir

1. Descomprimir el zip en cualquier carpeta (por ejemplo, el Escritorio).
2. Doble clic en **Iniciar pruebas.bat**. Se abre una ventana negra (no cerrarla mientras se prueba)
   y luego el navegador en http://127.0.0.1:8090.
   - Si Windows muestra "Windows protegió su PC": **Más información → Ejecutar de todas formas**
     (el programa aún no está firmado digitalmente).
3. Ingresar con:

   | Usuario    | Contraseña            | Puede                                                    |
   |------------|-----------------------|----------------------------------------------------------|
   | `admin`    | `proformas-demo-2026` | todo: anular, catálogos, empresas, usuarios y auditoría  |
   | `vendedor` | `proformas-demo-2026` | crear y emitir proformas, registrar clientes             |

Para cerrar, cerrar la ventana negra. Para volver a los datos iniciales: **Reiniciar datos de prueba.bat**.

No interfiere con una instalación real: usa otro puerto (8090) y otra base de datos.

## Qué revisar

- **Proformas**: buscar por número, cliente (sin tildes: "nuflo" encuentra "Ñuflo"), código de producto
  (p. ej. `FA-100`), empresa, fechas y estado. Abrir una vigente, una vencida, una anulada y una con R2.
- **Nueva proforma**: elegir empresa y cliente (o crear uno), agregar filas desde el catálogo escribiendo
  el código o la descripción, filas libres, reordenar (arrastrando o con Alt+↑/↓), mostrar u ocultar
  columnas, cambiar la vigencia y emitir.
- **Editar una emitida**: genera la revisión siguiente (R2) con el mismo número.
- **Imprimir / Guardar PDF**: probar en la impresora de la tienda, en Carta y A4 (cada empresa tiene uno).
- **Catálogos** (como `admin`): empresas con logo y sello, productos, clientes y plantillas de columnas.
- **Anular** (como `admin`) y comprobar que el vendedor no puede.

## Comentarios

Anotar para cada observación: pantalla, qué se hizo, qué se esperaba y, si se puede, una captura
(tecla Impr Pant). Todo comentario sirve: textos, orden de columnas, tamaños, colores, atajos.

