¡Por supuesto que puedo\! 🧠 Es crucial tener todos los módulos en un solo lugar.

Aquí tienes el archivo **README.md** actualizado y completo, incluyendo el curso para **Principiantes** (Beginner) y el curso **Avanzado** que ya resumimos.

-----

# 🚀 n8n Master Course: Automatización desde Cero hasta Enterprise

[](https://www.n8n.io/)
[](https://github.com)
[](https://www.n8n.io/)

Este es el índice de referencia y guía de estudio completa para los **Cursos de n8n para Principiantes y Avanzado**. Contiene todos los módulos para construir y gestionar flujos de trabajo escalables, fiables y modulares.

-----

## 📚 Índice General

| Curso | Módulo | Enfoque Principal |
| :--- | :--- | :--- |
| **Principiante** | **1/8** | Introducción a n8n, Terminología y Conceptos Básicos. |
| **Principiante** | **2/8** | El *Workflow* Básico, Nodos de Conexión. |
| **Principiante** | **3/8** | Manipulación de Datos (JSON, Expresiones). |
| **Principiante** | **4/8** | Lógica de Control de Flujo (IF, SWITCH, LOOPS). |
| **Principiante** | **5/8** | Subir Archivos, Credenciales y Webhooks. |
| **Principiante** | **6/8** | Nodos Avanzados de Datos (Code, Merge). |
| **Principiante** | **7/8** | Automatización de Ejemplo Completo. |
| **Principiante** | **8/8** | *Debugging* Básico y Gestión de Errores. |
| **Avanzado** | **2/8** | Nodos Técnicos (Code, HTTP Request, Loxon). |
| **Avanzado** | **3/8** | Debugging Avanzado (Pinning, Edit Output). |
| **Avanzado** | **4/8** | Sub-workflows (Modularidad y Reusabilidad). |
| **Avanzado** | **5/8** | Workflow de Errores Avanzado (Notificación al Propietario). |
| **Avanzado** | **6/8** | Ejemplo Completo Avanzado (API, Loops, Summary). |
| **Avanzado** | **7/8** | Manejo de Archivos Binarios (Compress/Decompress). |
| **Avanzado** | **8/8** | Características Empresariales (Variables, Roles, Git). |

-----

## I. 🟢 Curso para Principiantes (Módulos 1-8)

Esta sección cubre los fundamentos necesarios para construir tus primeras automatizaciones en n8n.

### Módulos 1-4: Fundamentos y Lógica Básica

| Módulo | Concepto Clave | Notas de Referencia Rápida |
| :--- | :--- | :--- |
| **1/8** | **Introducción & Terminología** | **Workflow:** El lienzo de automatización. **Nodes:** Los bloques de construcción. **Items:** Los datos que fluyen entre nodos. **Trigger:** El nodo que inicia el flujo. |
| **2/8** | **Workflow y Conexiones** | Tipos de Nodos: **Trigger** (inicio), **App** (servicios), **Core** (lógica). Conexión secuencial de nodos (A -\> B -\> C). |
| **3/8** | **Manipulación de Datos** | **JSON:** Estructura fundamental de los Items. **Expresiones (`{{ }}`):** Se usan para acceder a datos de Items anteriores (ej. `{{ $json.nombreDeCampo }}`). |
| **4/8** | **Control de Flujo** | **IF (Condicional):** Ejecución de una de dos ramas. **SWITCH:** Ejecución de múltiples ramas basadas en un valor. **Loop over Items:** Procesa cada Item de un array o lote individualmente. |

### Módulos 5-8: Integración y Robustez

| Módulo | Concepto Clave | Notas de Referencia Rápida |
| :--- | :--- | :--- |
| **5/8** | **Webhooks y Credenciales** | **Webhooks:** Disparador para recibir datos en tiempo real (URL única). **Credentials:** Almacenamiento seguro de claves API para nodos de App. |
| **6/8** | **Nodos Avanzados de Datos** | **Code:** Ejecutar código simple JS/Python para transformaciones (ej. sumas o formato). **Merge:** Combinar datos de diferentes ramas o *Items*. |
| **7/8** | **Ejemplo Práctico** | Construcción de un *workflow* de principio a fin (ej. `Webhooks -> Lógica -> Slack`). |
| **8/8** | **Debugging Básico** | **Historial de Ejecución:** Revisar el flujo de datos. **Stop and Throw Error:** Detener el flujo de manera controlada y lanzar un error. |

-----

## II. 🟦 Curso Avanzado (Módulos 2-8)

Esta sección profundiza en la escalabilidad, la modularidad y la gestión de grandes volúmenes de datos y entornos críticos.

### Módulos 2-4: Técnicas y Estructura

| Módulo | Concepto Clave | Aplicación Práctica |
| :--- | :--- | :--- |
| **2/8** | **Nodos Técnicos** | **Nodo Code:** Modos "Run Once for All" (agregación) y "Run Once for Each" (transformación por Item). **HTTP Request:** Importación de **cURL** y **Paginación** automática. **Loxon:** Uso de la librería de fechas en expresiones (`{{ $now }}`). |
| **3/8** | **Debugging Avanzado** | **Fijación de Datos (*Pinning*):** Guarda la salida de un nodo para **pruebas rápidas** sin reejecutar el Trigger/API. **Edit Output Data:** Modificar manualmente el JSON para **simular casos límite** (ej. valores nulos). |
| **4/8** | **Sub-workflows** | **Execute Workflow:** Llama a un flujo como una función. Permite la **reusabilidad** (construir una vez, usar en muchos flujos) y el **mantenimiento centralizado**. **Estandarización:** Crucial para que el Sub-workflow no falle. |

### Módulos 5-8: Fiabilidad y Enterprise

| Módulo | Concepto Clave | Aplicación Práctica |
| :--- | :--- | :--- |
| **5/8** | **Workflow de Errores** | **Error Trigger:** Disparador que captura **cualquier fallo** en la instancia. **Sistema de Notificación Inteligente:** Consulta el nodo **n8n** para obtener el **propietario** del flujo fallido y notificarle directamente. |
| **6/8** | **Ejemplo Completo Avanzado** | Demostración de **Loop over Items** con **HTTP Request** y **gestión de errores** internos (If + Stop). Uso de **Summarize** y **Slack Blocks** para notificaciones ricas. |
| **7/8** | **Manejo de Archivos** | **Datos Binarios:** Cómo los nodos manejan imágenes y ZIPs. **Compress/Decompress:** Nodos para archivar y extraer. **División de Archivos:** Uso del nodo **Code** para dividir un solo Item con múltiples archivos en *múltiples Items* separados para el procesamiento. |
| **8/8** | **Enterprise Features** | **Execution Data:** Guarda IDs clave (ej. `orderId`) para **búsqueda rápida** en el historial. **Custom Variables:** Valores diferentes para los entornos **Dev/Prod** (ej. URLs de bases de datos). **Source Control (Git):** Despliegue seguro y **versionado** de *workflows*. |

-----

> 💡 **Consejo:** Utiliza la herramienta de búsqueda de tu editor de texto o navegador (Ctrl+F o Cmd+F) para encontrar rápidamente cualquier concepto en este archivo (ej. `Pinning`, `Loxon`, `Sub-workflows`).
