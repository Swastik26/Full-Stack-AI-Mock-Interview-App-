# React + TypeScript + Vite

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

# Fullstack AI Mock Interview App

## Overview
The **Fullstack AI Mock Interview App** is a web-based application designed to simulate real-world interview experiences using AI. The platform provides users with an interactive and personalized mock interview experience, helping them improve their skills and confidence before facing real interviews.

## Live Demo
Explore the application at: [AI Mock Interview App](https://ai-mockup-inter.web.app/)

## Features
- **AI-Driven Mock Interviews**: Get real-time, AI-powered interview simulations based on your selected domain.
- **Personalized Feedback**: Receive detailed feedback and analysis on your performance.
- **Multi-Domain Support**: Covers technical, behavioral, and HR interview scenarios.
- **User-Friendly Interface**: Intuitive and easy-to-use interface for seamless navigation.
- **Real-Time Evaluation**: AI assesses responses and provides immediate insights.
- **Interview Preparation Resources**: Access useful tips, sample questions, and best practices.

## Technologies Used
- **Frontend**: React.js, Tailwind CSS
- **Backend**: Node.js, Express.js
- **Database**: Firebase Firestore
- **AI Processing**: OpenAI API (or equivalent AI-based model)
- **Authentication**: Firebase Authentication
- **Hosting**: Firebase Hosting

## Installation & Setup
To run the application locally:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/ai-mock-interview.git
   cd ai-mock-interview
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Create a `.env` file and add your Firebase and AI API keys.
4. Start the development server:
   ```bash
   npm start
   ```

## Deployment
- The app is deployed on Firebase Hosting. To deploy a new version:
  ```bash
  firebase deploy
  ```

## Future Enhancements
- Adding more AI models for deeper analysis.
- Expanding question banks across more industries.
- Introducing mock coding interviews with real-time code execution.

## Contributing
Contributions are welcome! Feel free to fork the repo and submit pull requests.

## License
This project is licensed under the MIT License.



