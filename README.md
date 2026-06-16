# 🧠 Gemini Mindmap

An interactive, AI-powered mind-mapping application built with **React 19**, **Vite**, and **React Flow**. Generate real-time, branched learning maps from your questions using cutting-edge Large Language Models (LLMs).

Una aplicación interactiva de mapas mentales impulsada por IA, desarrollada con **React 19**, **Vite** y **React Flow**. Genera mapas de aprendizaje ramificados en tiempo real a partir de tus preguntas usando Modelos de Lenguaje (LLMs) de última generación.

---

## 🚀 Key Features / Características Clave

### 🤖 Multi-Provider LLM Integration / Integración Multiproveedor de LLM
- **Google Gemini**: Integrates the `@google/generative-ai` SDK, supporting models like `Gemini 1.5 Flash`, `Gemini 2.5 Flash`, and `Gemini 3.5 Flash`.
- **Anthropic Claude**: Integrates the `@anthropic-ai/sdk`, supporting models like `Claude 3.5 Sonnet` and others.
- **Local Credentials**: API keys are securely stored in your browser's `localStorage` and never sent to any intermediary server.
- *Español*: Soporte nativo para Google Gemini y Anthropic Claude. Las API keys se guardan de forma segura en el almacenamiento local del navegador (`localStorage`).

### 🎨 Matrix Hack-Terminal Aesthetic / Estética Matrix Dark Mode
- Built with a curated green/black monospace theme. Features glowing panels, custom-styled handles, and custom animations.
- *Español*: Tema monospace con detalles en verde neón y paneles de vidrio semitransparente (glassmorphism).

### 🗺️ Smart Canvas Routing / Enrutamiento Inteligente en Lienzo
- **MAIN Path (↓ Down)**: Focuses the AI on drilling deeper into the current core topic (spawns a child node at `y + 500px`).
- **BRANCH Path (→ Right)**: Directs the AI to explore lateral concepts or secondary questions (spawns a child node at `x + 450px`).
- **Clean Connections**: Custom React Flow handles prevent cyclic loops. The root node has its inputs hidden, forcing a clean hierarchical growth.
- *Español*: Ruta **MAIN ↓** para profundizar y **BRANCH →** para temas secundarios. Conectores dinámicos para evitar cruces y líneas diagonales desordenadas.

### 📸 High-Resolution Image Export / Exportación de Imagen en Alta Resolución
- Captures the complete map using `html-to-image`.
- **Overflow Expansion**: Automatically expands scrollable/cropped node text content (`max-height: 250px` to full height) during capture, and hides canvas controls, handle dots, and editing inputs for a clean production export.
- *Español*: Exporta todo el lienzo a PNG. Expande automáticamente el texto con scroll para que salga completo en la imagen y oculta botones, controles y conectores.

### ⚙️ Quick Configuration & Code Rendering / Ajustes Rápidos y Renderizado de Código
- Easily swap providers, API keys, or models at any time using the quick settings gear icon (`⚙️`).
- Built-in Markdown parser with syntax-highlighted multi-line code boxes and instant "Copy" buttons.
- *Español*: Panel de configuración flotante para cambiar de modelo o proveedor, y formateador automático de código Markdown con botón de copiado rápido.

---

## 📁 Project Structure / Estructura del Proyecto

```text
├── src/
│   ├── main.jsx              # React application entry point / Entrada de React
│   ├── App.jsx               # Canvas state, layout, and UI modals / Estado del lienzo y UI
│   ├── App.css               # Modal transitions, camera effects, UI overrides / Estilos generales
│   ├── index.css             # Matrix color palette (CSS variables), typography / Variables CSS de temas
│   ├── components/
│   │   ├── ChatNode.jsx      # Custom React Flow Node, handles prompting / Nodo personalizado
│   │   └── ChatNode.css      # Monospace styling, scrollbars, export overrides / Estilos del nodo
│   └── services/
│       ├── aiService.js      # Multi-provider factory abstraction / Abstracción del servicio de IA
│       └── providers/
│           ├── geminiProvider.js     # Google Gemini SDK connection / Conexión a Gemini
│           └── anthropicProvider.js  # Anthropic Claude SDK connection / Conexión a Claude
├── TECHNICAL_DOCUMENT.md     # In-depth architectural documentation / Documentación técnica detallada
└── USER_MANUAL.md            # Detailed configuration & troubleshooting guide / Guía de usuario
```

---

## 🛠️ Getting Started / Primeros Pasos

### Prerequisites / Requisitos Previos
Make sure you have [Node.js](https://nodejs.org/) installed (v18+ recommended) and a valid API key from [Google AI Studio](https://aistudio.google.com/) or [Anthropic Console](https://console.anthropic.com/).

Asegúrate de tener instalado [Node.js](https://nodejs.org/) (v18 o superior) y una API Key activa de [Google AI Studio](https://aistudio.google.com/) o [Anthropic Console](https://console.anthropic.com/).

### Installation / Instalación

1. **Clone the repository / Clonar el repositorio:**
   ```bash
   git clone https://github.com/juanitoisback6/MindMap-Antigravity.git
   cd MindMap-Antigravity
   ```

2. **Install dependencies / Instalar dependencias:**
   Using `npm`:
   ```bash
   npm install
   ```
   Or using `pnpm`:
   ```bash
   pnpm install
   ```

3. **Run the development server / Iniciar servidor de desarrollo:**
   ```bash
   npm run dev
   ```
   Open your browser and navigate to `http://localhost:5173` (or the port shown in your terminal).

4. **Build for production / Compilar para producción:**
   ```bash
   npm run build
   ```

---

## 📖 Learn More / Aprende Más

- **[User Manual (Manual de Usuario)](file:///c:/Users/Juan/OneDrive/Documentos/Proyectos/mindmapantigravity/USER_MANUAL.md)**: A complete guide on how to configure your API keys, use the main/branch options, and troubleshoot connection issues.
- **[Technical Document (Documento Técnico)](file:///c:/Users/Juan/OneDrive/Documentos/Proyectos/mindmapantigravity/TECHNICAL_DOCUMENT.md)**: Deep dive into the architecture, custom React Flow handle layouts, markdown parsing, and the capture engine stylesheet logic.

---

*Developed for visual, AI-augmented research and exploration. / Desarrollado para investigación y exploración visual aumentada con Inteligencia Artificial.*
