# Módulo 4: Investigación en Salud y Emergencias en Argentina (2020–2025)

Este repositorio contiene el entorno académico integrado para compilar el **Artículo Científico** sobre vulnerabilidades en el sistema de emergencias médicas, fragmentación sanitaria, la industria farmacéutica y protocolos de triage hospitalario en la República Argentina. 

El entorno utiliza la plantilla profesional **Distill** de R Markdown (`distill::distill_article`), configurada para generar un menú flotante lateral interactivo (`toc_float: true`), gráficos estadísticos avanzados (`ggplot2`) y tablas analíticas elegantes (`kableExtra`).

---

## 📁 Estructura del Proyecto

Para que el informe compile correctamente en **Posit Cloud (RStudio)**, tu panel de archivos (`Files`) debe verse estructurado de la siguiente manera:

```text
📂 MiProyectoR/
 ├── 📄 Investigación Triage Emergencia.Rmd  <-- Tu hoja de trabajo principal (Código R Markdown)
 ├── 📄 investigacion_salud_emergencias.json  <-- El archivo de datos subido con los textos redactados
 └── 📄 README.md                             <-- Esta guía de instalación y uso rápido
```

---

## 🛠️ Requisitos e Instalación de Librerías

Antes de presionar el botón **Knit**, es indispensable asegurarse de tener instaladas todas las dependencias necesarias en la consola de tu sesión de R. Ejecuta el siguiente comando para garantizar que no existan errores de paquetes faltantes:

```R
# Ejecuta esta línea directamente en la "Console" de Posit Cloud si falta algún paquete:
install.packages(c("distill", "jsonlite", "tidyverse", "knitr", "kableExtra"))
```

---

## 🚀 Instrucciones de Uso Rápido (Paso a Paso)

Si experimentaste fallas técnicas previas (como errores de tipos o listas crudas), sigue rigurosamente esta secuencia de restablecimiento operativo:

1. **Limpieza Absoluta:** Abre tu archivo principal `Investigación Triage Emergencia.Rmd` en Posit Cloud. Selecciona todo el texto (desde la línea 1 hasta el final) y bórralo por completo. La hoja debe quedar vacía.
2. **Inyección de Código Corregido:** Copia el bloque completo estructurado con la cabecera YAML (los tres guiones `---`) y la función adaptativa de aplanamiento de listas (`imprimir_texto`). Asegúrate de que los primeros guiones comiencen exactamente en la **Línea 1**.
3. **Validación del JSON:** Verifica que el archivo `investigacion_salud_emergencias.json` esté cargado en el mismo directorio de trabajo y con el nombre idéntico (todo en minúsculas y separado por guiones bajos).
4. **Compilación Mágica:** Haz clic en el botón 🧶 **Knit** ubicado en la barra superior de herramientas de RStudio. El entorno leerá el JSON de manera segura, vinculará los párrafos sin trabas técnicas y desplegará tu informe interactivo con el menú flotante lateral.

---

## 📊 Componentes Especiales Incluidos

* **Menú Lateral Autogestionado:** Indexación dinámica y flotante (`toc`) de secciones y subsecciones en base al formato estándar de artículos académicos.
* **Controlador Adaptativo de Datos (`imprimir_texto`):** Rutina programada en R para procesar de forma automatizada objetos estructurados complejos o listas de caracteres anidadas dentro del JSON, evitando errores de renderizado en `cat()`.
* **Visualización de Datos:** Gráfico de barras horizontales optimizado cromáticamente en escala de azules utilizando capas geométricas de `ggplot2`.
* **Presentación Tabular:** Renderizado adaptativo mediante Bootstrap y estilos de cebra (`striped`) para maximizar la legibilidad de la infraestructura sanitaria analizada.

---
*Desarrollado para el análisis avanzado de políticas públicas sanitarias y gestión de emergencias asistenciales.*
