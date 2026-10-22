# Limpieza y Depuración de Base de Datos para Flujo n8n

## 📌 Descripción del Proyecto
Este repositorio contiene un pipeline de datos desarrollado en **Python** para la limpieza, estandarización y depuración de una base de datos. El objetivo principal es preparar los datos en formato **JSON** para que puedan ser consumidos de manera rápida y eficiente por un flujo de trabajo automatizado en **n8n**.

## 🛠️ Tecnologías Utilizadas
*   **Python** (Lenguaje principal)
*   **Pandas** (Manipulación y limpieza de datos)
*   **Google Colab** (Entorno de desarrollo y ejecución)
*   **GitHub** (Control de versiones)
*   **n8n** (Destino final de los datos limpios)

## ⚙️ ¿Qué hace el script?
El script realiza las siguientes tareas de depuración:
1.  **Extracción:** Lectura de la base de datos (CSV/SQL) alojada en Google Drive.
2.  **Estandarización:** Limpieza de nombres de columnas (minúsculas, sin espacios) y eliminación de espacios en blanco en campos de texto.
3.  **Calidad de Datos:** Eliminación de registros duplicados y manejo de valores nulos en columnas clave.
4.  **Conversión de Tipos:** Formateo de fechas y valores numéricos para evitar errores en el flujo.
5.  **Exportación:** Generación de un archivo `datos_limpios_n8n.json` listo para ser inyectado en n8n.

## 🚀 Cómo usar este proyecto
1.  Abre el archivo `.ipynb` de este repositorio directamente en **Google Colab**.
2.  Monta tu Google Drive (`drive.mount('/content/drive')`).
3.  Ajusta la ruta del archivo de origen en la primera celda de código.
4.  Ejecuta las celdas en orden.
5.  Descarga el archivo JSON generado o envíalo directamente a tu webhook de n8n.

---
*Proyecto desarrollado como demostración de habilidades en automatización, limpieza de datos y control de versiones.*
