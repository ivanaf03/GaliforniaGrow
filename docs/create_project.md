# Create the project
Node version: **v24.13.0**

## Project Setup
To scaffold the project and start the development server, run the following commands:

```
node --version
npm create vite@latest galiforniagrow -- --template react
cd galiforniagrow
npm install
npm run dev
```

## Clear and prepare github project
Once the project is running on localhost:5173, feel free to remove the boilerplate files and structure the project according to your needs.

```
// main.js

import { createRoot } from "react-dom/client";

import App from "./App.jsx";

createRoot(document.getElementById("root")).render(<App />);
```

```
// App.js

const App = () => {
  return (
    <div className="App">
      <h1>Galifornia Grow - In development...</h1>
    </div>
  );
};

export default App;
```

 Next step is prepare the GitHub repository. Run the following commands:

```
git config --global init.defaultBranch main
git init
gt add .
git commit -m "config: create initial commit"
git remote add origin https://github.com/ivanaf03/GaliforniaGrow.git
git push -u origin main
```

## Prepare Vercel project
Go to Vercel and create a new project. Select the repository and choose Vite as the framework. Once the project is imported, click on the "Deploy" button. 