# 🏷️ Generador de Etiquetas de Precios — Macropay

Una herramienta web minimalista, moderna y de alto rendimiento diseñada específicamente para la maquetación y generación de etiquetas de precios en plantillas de impresión tamaño carta. Funciona 100% de manera local y en el navegador, ofreciendo una experiencia limpia sin servidores ni dependencias externas.

---

## 🚀 Características Principales

*   **Diseño Premium**: Interfaz elegante construida sobre la tipografía *Inter*, con layouts limpios, sombras sutiles y micro-animaciones en los botones.
*   **Modo Claro / Oscuro**: Adaptación visual completa con paletas de color cuidadosamente seleccionadas (tonos Slate para el modo claro y azul marino profundo para el modo oscuro). Conserva la preferencia mediante `localStorage`.
*   **Autocalibración de Fuente**: Escala automáticamente el tamaño de la fuente para precios largos (desde `24pt` hasta un mínimo de `11pt`), garantizando que la cifra nunca se desborde del límite físico de la etiqueta.
*   **Gestión Interactiva de Etiquetas**:
    *   Ingreso rápido con validación de caracteres en tiempo real (solo acepta números, puntos, comas y `$`).
    *   Formateo automático de miles usando la configuración local (`toLocaleString`).
    *   Eliminación individual de etiquetas haciendo **doble clic** directamente sobre la etiqueta en la vista previa.
    *   Modal personalizado para confirmar el reinicio completo de la hoja, previniendo borrados accidentales.
*   **Optimización de Impresión**: Reglas `@media print` configuradas para ocultar automáticamente el panel de control y centrar la hoja de etiquetas de manera exacta.
*   **Privacidad Absoluta**: Todo el procesamiento se realiza localmente en el cliente. Ninguna información es transmitida a internet.

---

## 📐 Especificaciones de la Plantilla de Impresión

El diseño de la cuadrícula ha sido estructurado mediante CSS Grid para calzar con medidas físicas estándar:

| Elemento | Medida / Distribución |
| :--- | :--- |
| **Tamaño de Hoja** | Carta (`8.5 in x 11 in` / `21.59 cm x 27.94 cm`) |
| **Dimensiones de la Etiqueta** | `3.7 cm` (ancho) x `1.5 cm` (alto) |
| **Distribución** | Cuadrícula de 4 columnas y 10 filas |
| **Capacidad Máxima** | 40 etiquetas por página |
| **Márgenes de Hoja** | `1.0 cm` en todo el borde |

---

## 🔧 Instalación y Uso

### Ejecución Local
No requiere de servidores ni bases de datos. Simplemente clona este repositorio y abre el archivo en tu navegador web preferido:

1. Clona el repositorio:
   ```bash
   git clone https://github.com/jesushv77/Etiquetas-Macropay.git
   ```
2. Entra en el directorio:
   ```bash
   cd Etiquetas-Macropay
   ```
3. Abre [Etiquetas.html](Etiquetas.html) en tu navegador (puedes hacer doble clic sobre el archivo o arrastrarlo a una ventana abierta del navegador).

### Guía de Operación
1. Introduce un precio en el campo **"Ingresar precio"** (ej: `1234.56`). El sistema le añadirá formato de moneda automáticamente.
2. Presiona **Enter** o haz clic en **"Agregar"** para colocar la etiqueta en la hoja.
3. Si te equivocas, haz **doble clic** sobre la etiqueta que deseas remover dentro de la vista previa.
4. Para limpiar la hoja completa, usa el botón **"Reiniciar hoja"** y acepta en el modal emergente.
5. Cuando tengas tus etiquetas listas, haz clic en **"Generar PDF"**.
   * *Nota de Impresión:* En el cuadro de diálogo de tu navegador, asegúrate de configurar los **márgenes como "Ninguno" o "Predeterminado"** y la **escala al 100%** para conservar las dimensiones exactas en centímetros.

---

## 🛠️ Tecnologías Utilizadas

*   **HTML5**: Maquetación semántica y estructura del panel de control.
*   **CSS3 (Vanilla)**: Variables de diseño para temas, layouts con Flexbox y CSS Grid, y estilos optimizados para medios impresos (`@media print`).
*   **JavaScript (Vanilla)**: Gestión interactiva del DOM, validación selectiva, ajuste dinámico de tamaño de tipografías y lógica para modales interactivos.

---

## 📝 Soporte y Contacto

> [!NOTE]
> Si experimentas algún problema de alineación, rendimiento o visualización, ponte en contacto con tu **Visual asignado** de Macropay para asistencia técnica directa.

---

## 📦 Licencia

Este proyecto está bajo la Licencia MIT. Consulta el archivo de licencia para más detalles.