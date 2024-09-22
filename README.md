# React + TypeScript + Vite + FastAPI

### Installation

1. Clone the repository:

```bash
git clone https://github.com/anubhavtripathi0509/AIMathsTutor.git
```

2. Navigate to the frontend directory:

```bash
cd frontend
```

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type aware lint rules:

- Configure the top-level `parserOptions` property like this:

```js
export default tseslint.config({
  languageOptions: {
    // other options...
    parserOptions: {
      project: ['./tsconfig.node.json', './tsconfig.app.json'],
      tsconfigRootDir: import.meta.dirname,
    },
  },
})
```

- Replace `tseslint.configs.recommended` to `tseslint.configs.recommendedTypeChecked` or `tseslint.configs.strictTypeChecked`
- Optionally add `...tseslint.configs.stylisticTypeChecked`
- Install [eslint-plugin-react](https://github.com/jsx-eslint/eslint-plugin-react) and update the config:

```js
// eslint.config.js
import react from 'eslint-plugin-react'

export default tseslint.config({
  // Set the react version
  settings: { react: { version: '18.3' } },
  plugins: {
    // Add the react plugin
    react,
  },
  rules: {
    // other rules...
    // Enable its recommended rules
    ...react.configs.recommended.rules,
    ...react.configs['jsx-runtime'].rules,
  },
})
```

3. Install the dependencies:

```js
npm install
```

4. Run the Frontend

```js
npm run dev
```



### Backend

### Key Features

- **FastAPI** for building high-performance RESTful APIs.
- **Gemini API** integration to handle specific operations.
- **Python** with dependencies managed via `requirements.txt`.

### Getting Started

Follow these steps to set up and run the backend locally.

### Prerequisites

Ensure you have **Python** and **pip** installed.

### Installation
1. Open one more powershell for backend

2. Navigate to the backend directory:

```bash
cd backend
```

### Environment Setup

1. Create a `.env` file in the `backend` directory:

```bash
touch .env
```

2. Add your **Gemini API Key** to the `.env` file:

```plaintext
GEMINI_API_KEY=your_gemini_api_key_here
```

Replace `your_gemini_api_key_here` with your actual API key.

### Install Dependencies

Install the necessary Python packages by running:

```bash
pip install -r requirements.txt
```

### Running the Backend

To start the FastAPI server, run:

```bash
python main.py
```

This will launch the server at `http://localhost:8000`.


## Contact

For any questions or inquiries, feel free to contact the repository owner [Anubhav Tripathi](https://github.com/anubhavtripathi0509) 8104083562.
```


## AIMathsTutor