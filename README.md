# SIRA · Proyección del sistema digestivo sobre maniquí

Aplicación web de un solo archivo (`index.html`). Funciona sin internet y sin instalar nada.

## Puesta en marcha
1. Conecta el proyector como **pantalla extendida** (no duplicada).
2. Abre `index.html` con Chrome o Firefox y arrastra la ventana a la pantalla del proyector.
3. Pulsa **F** para la pantalla completa. **Calibra siempre en pantalla completa**: las posiciones se guardan relativas a la ventana.

## Calibración (tres pasos)
| Paso | Tecla | Qué haces |
|---|---|---|
| 1 · Puntos | `P` | Arrastra cada cruz (ombligo, pezones, xifoides, caderas, hombros, pubis…) hasta su sitio real en el maniquí. Con 1 punto la imagen se desplaza, con 2 se escala y gira, con 3 o más se deforma (thin-plate spline). Usa solo los puntos que tenga tu maniquí. |
| 2 · Malla | `G` | Ajuste fino: arrastra los nodos donde la imagen no siga la curvatura. Pon la imagen «Cuadrícula» (`T`) para ver mejor la deformación. `+`/`−` cambian la densidad. |
| 3 · Máscara | `M` | Haz clic alrededor del contorno del maniquí. Lo que queda fuera se proyecta en negro. La imagen «Blanco» ayuda a ver los bordes. |

«der./izq.» se refiere al lado **del bebé**: su derecha queda a la izquierda de quien mira de frente.

La calibración se guarda sola en el navegador. Con **Exportar** la guardas en un archivo `.json` (es buena idea tener una copia) y con **Importar** la recuperas.

## Presentación
- `Espacio`: alterna entre presentación y el último modo de calibración.
- `H`: oculta el panel (también se oculta el cursor).
- `R`: recorrido guiado, que resalta cada órgano con su descripción. Avanza solo, o con `←`/`→`.
- `A`: animación del bolo alimenticio recorriendo el tubo digestivo.
- `L`: etiquetas · `1`–`0`: mostrar u ocultar cada órgano · `[` `]`: brillo.
- **Imagen propia…**: sustituye el dibujo por tu propia ilustración (PNG/JPG/SVG con fondo negro). Se deforma con la misma calibración.

## Otros atajos
`Tab` selecciona el siguiente punto · flechas: mover 1 px (`Mayús` ×10) · `Mayús`+arrastrar: mover todo · rueda: escalar todo · `Supr` o clic derecho: quitar o reiniciar el punto · `Ctrl+Z`: deshacer · `Ctrl+S`: exportar.
