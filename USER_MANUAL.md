# User Manual / Manual de Usuario - Gemini Mindmap

Welcome to the **Gemini Mindmap** user manual. This bilingual guide will help you configure, run, and master your interactive AI-powered mind-mapping application.

Bienvenido al manual de usuario de **Gemini Mindmap**. Esta guía bilingüe te ayudará a configurar, ejecutar y dominar tu aplicación interactiva de mapas mentales impulsada por IA.

---

## Table of Contents / Índice

1. [English Guide](#english-guide)
   - [Overview](#1-overview)
   - [Configuration & API Setup](#2-configuration--api-setup)
   - [How to Use (Mind-Mapping)](#3-how-to-use-mind-mapping)
   - [Key Features](#4-key-features)
   - [Troubleshooting](#5-troubleshooting)
2. [Guía en Español](#guía-en-español)
   - [Descripción General](#1-descripción-general)
   - [Configuración y Ajuste de API](#2-configuración-y-ajuste-de-api)
   - [Modo de Uso (Mapas Mentales)](#3-modo-de-uso-mapas-mentales)
   - [Características Clave](#4-características-clave)
   - [Solución de Problemas](#5-solución-de-problemas)

---

# English Guide

## 1. Overview
**Gemini Mindmap** is a visual learning tool that generates real-time, interactive mind maps from your questions using artificial intelligence. It helps you break down complex concepts into hierarchical or lateral branches.

## 2. Configuration & API Setup
When launching the application for the first time, you will be greeted by the **AI Configuration Dialog**:

1. **Choose your AI Provider:** Toggle between **Gemini** (Google) and **Claude** (Anthropic).
2. **Select the AI Model:** Pick a model from the dropdown (e.g., `Gemini 3.5 Flash` or `Claude Sonnet 4`).
3. **Enter your API Key:** Paste the corresponding key:
   - For Gemini, it begins with `AIzaSy...`
   - For Claude, it begins with `sk-ant-...`
4. **Launch:** Click **"Comenzar la experiencia"** (Start the experience). The app will perform a fast connection test query to ensure your key is valid and has active permissions.

> [!NOTE]
> Your keys are saved locally in your browser's `localStorage` (`GEMINI_API_KEY` or `ANTHROPIC_API_KEY`). You do not need to re-enter them on every launch, but the setup screen will display on startup to let you confirm or switch models/providers.

## 3. How to Use (Mind-Mapping)
The workspace starts with a single **Root Node** labeled: **"🧠 ¿Qué deseas aprender hoy?"** (What do you want to learn today?).

To build your mind map:
- **Type a question:** Click the input box on any node and type what you want to expand or explore.
- **MAIN Path (↓ Down):** Press the `MAIN ↓` button or hit `Enter`. The AI will generate a response, creating a new node directly below (`y + 500px`) linked by a **bright neon-green animated line**.
- **BRANCH Path (→ Right):** Press the `BRANCH →` button. The AI will generate a response, creating a new node to the right (`x + 450px`) linked by a **medium emerald-green animated line**.

> [!TIP]
> Use the **MAIN** direction to drill down deeper into the core timeline or steps of a topic, and the **BRANCH** direction to explore lateral concepts, side questions, or vocabulary terms.

## 4. Key Features
- **Monospace Matrix Aesthetic:** Centralized color variables (`index.css`) deliver a full hacker-terminal layout with glowing green typography and dark glassmorphic panels.
- **Dynamic Render Controls:** The Root Node has target and branch handles hidden to preserve layout clarity.
- **Code Block Formatter:** Whenever the AI returns code snippets (within markdown backticks \`\`\`), they are formatted inside clean code-container boxes showing the syntax language and a **"COPIAR" (Copy)** button for easy clipboard extraction.
- **Canvas Zoom & Pan:** Drag to pan the screen, and use your mouse wheel or React Flow panel controls to zoom in and out.
- **Quick Settings:** Tap the settings icon (`⚙️`) at the top left to return to the setup screen and change providers or models at any time.

## 5. Troubleshooting
- **"La API Key ingresada es inválida o no tiene permisos":** Double-check that you copied the key correctly and did not include leading spaces. Ensure your account has remaining billing credits/quota.
- **Response Errors:** If a node shows a connection alert, check your network status or ensure the selected model is currently supported by your API key.

---

# Guía en Español

## 1. Descripción General
**Gemini Mindmap** es una herramienta de aprendizaje visual que genera mapas mentales interactivos en tiempo real a partir de tus preguntas usando inteligencia artificial. Te ayuda a desglosar conceptos complejos en ramificaciones jerárquicas o laterales.

## 2. Configuración y Ajuste de API
Al abrir la aplicación por primera vez, verás el **Diálogo de Configuración de IA**:

1. **Elige tu Proveedor de IA:** Alterna entre **Gemini** (Google) y **Claude** (Anthropic).
2. **Selecciona el Modelo de IA:** Elige un modelo del menú desplegable (ej. `Gemini 3.5 Flash` o `Claude Sonnet 4`).
3. **Ingresa tu API Key:** Pega la clave correspondiente:
   - Para Gemini, suele comenzar con `AIzaSy...`
   - Para Claude, suele comenzar con `sk-ant-...`
4. **Comenzar:** Haz clic en **"Comenzar la experiencia"**. La aplicación realizará una prueba rápida de conexión para verificar que la clave sea válida y tenga permisos activos.

> [!NOTE]
> Tus claves se guardan localmente en el `localStorage` de tu navegador (`GEMINI_API_KEY` o `ANTHROPIC_API_KEY`). No necesitas ingresarlas de nuevo en cada sesión, pero la pantalla inicial aparecerá al cargar para que confirmes o cambies de modelo/proveedor.

## 3. Modo de Uso (Mapas Mentales)
El lienzo de trabajo inicia con un único **Nodo Raíz** titulado: **"🧠 ¿Qué deseas aprender hoy?"**.

Para construir tu mapa mental:
- **Escribe una pregunta:** Haz clic en el cuadro de texto de cualquier nodo e ingresa el tema que quieras explorar.
- **Camino MAIN (↓ Abajo):** Presiona el botón `MAIN ↓` o pulsa la tecla `Enter`. La IA generará la respuesta creando un nodo nuevo directamente abajo (`y + 500px`) conectado por una **línea animada verde neón brillante**.
- **Camino BRANCH (→ Derecha):** Presiona el botón `BRANCH →`. La IA creará un nuevo nodo a la derecha (`x + 450px`) conectado por una **línea animada verde esmeralda**.

> [!TIP]
> Utiliza la dirección **MAIN** para profundizar cronológicamente o ir al núcleo del tema, y la dirección **BRANCH** para abrir subtemas, preguntas alternativas o conceptos relacionados.

## 4. Características Clave
- **Estética Monospace Matrix:** Los colores están centralizados en variables globales CSS (`index.css`), ofreciendo un diseño de terminal hacker con tipografía brillante y paneles semitransparentes.
- **Control Dinámico de Conectores:** El Nodo Raíz tiene los conectores superior y lateral ocultos para mantener limpio el inicio del mapa.
- **Formateador de Bloques de Código:** Si la respuesta de la IA incluye código (delimitado por comillas triples \`\`\`), se renderizará en un bloque especial indicando el lenguaje y un botón funcional de **"COPIAR"** para llevarlo al portapapeles.
- **Zoom y Desplazamiento:** Arrastra el lienzo para moverte y usa la rueda del ratón o el panel de controles de React Flow en la esquina inferior para cambiar el zoom.
- **Configuración Rápida:** Haz clic en el botón de engranaje (`⚙️`) en la parte superior izquierda en cualquier momento para volver a la pantalla de API y cambiar de modelo o proveedor.

## 5. Solución de Problemas
- **"La API Key ingresada es inválida o no tiene permisos":** Revisa que hayas copiado la clave completa y sin espacios extra. Asegúrate de que tu cuenta de desarrollador tenga saldo/créditos de uso activos.
- **Errores de Respuesta:** Si un nodo alerta un fallo de red, verifica tu conexión a internet o comprueba si el modelo seleccionado está disponible para tu nivel de suscripción de API.
