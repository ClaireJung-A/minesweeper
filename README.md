### **📝 Minesweeper Game Implementation**

![Minesweeper Thumbnail](https://github.com/eeeyooon/portfolio/assets/112360210/ec1aa987-c406-44e3-9752-58b0a84be1ce)

---

## **📌 Project Setup & Execution**

To run this project, open the directory and execute the following commands:

```bash
npm install
yarn install
```

```bash
npm run start
yarn start
```

---

## **📌 Project Overview**
📢 **Project Theme**: A fully implemented **Minesweeper game**.  
📆 **Project Duration**: **Dec 7, 2023 - Dec 11, 2023**  
🍊 **[Try the Minesweeper Game](https://yoon-minesweeper.vercel.app/)**  

---

## **📌 Tech Stack**

<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=TypeScript&logoColor=white"/> <img src="https://img.shields.io/badge/React-61DAFB?style=flat&logo=React&logoColor=white"/> <img src="https://img.shields.io/badge/Redux-764ABC?style=flat&logo=Redux&logoColor=white"/> <img src="https://img.shields.io/badge/ReduxToolkit-764ABC?style=flat&logo=Redux&logoColor=white"/> <img src="https://img.shields.io/badge/styledcomponents-DB7093?style=flat&logo=styled-components&logoColor=white"/>

📌 The folder structure and libraries used can be found at the bottom of this README.

---

## **📌 Features Implemented**

### **🎮 Starting the Minesweeper Game**
![Minesweeper Start](https://github.com/eeeyooon/portfolio/assets/102462534/2005c3c6-7241-4d9b-bccc-69c8b1b45486)

- The game begins when the first empty tile is opened.
- **No mines will be triggered** on the first move.
- A **timer starts** when the game begins and stops when the game ends.
- The **remaining mine count** is displayed. Placing flags reduces the count, assuming all flags are correctly placed.
- If a **tile with no adjacent mines is opened**, all surrounding tiles will automatically open using a recursive algorithm.

---

### **🚩 Right-Click to Place Flags / Question Marks**
![Flag & Question Mark](https://github.com/eeeyooon/portfolio/assets/102462534/df2b5347-b141-494e-b5bf-c51e5e3cdb8d)

- **Right-clicking a tile places a flag**.
- **Right-clicking again changes it to a question mark**.
- **A third right-click resets it to an empty tile**.

---

### **🏆 Winning the Minesweeper Game**
![Game Victory](https://github.com/eeeyooon/portfolio/assets/102462534/ae3b9186-c8ab-41d9-ad59-927b7e1674a4)

- The game is **won when all non-mine tiles are opened**.
- Flags and question marks do not count as opened tiles.

---

### **⚙️ Changing Difficulty & Losing the Game**
![Difficulty & Game Over](https://github.com/eeeyooon/portfolio/assets/102462534/76a31f35-5958-44a6-aea4-e5466745a773)

- Difficulty levels: **Beginner, Intermediate, Expert**.
- The **board size and number of mines** change depending on the selected difficulty.
- **Opening a tile with a mine results in a loss**.

---

### **🛠️ Custom Difficulty Mode**
![Custom Difficulty](https://github.com/eeeyooon/portfolio/assets/102462534/d8825f54-9779-4bee-b2f1-ffab105e9ee1)

- Users can **set custom board dimensions** and **number of mines**.
- The **max grid size is 100x100**, with mines **limited to one-third of total tiles**.

---

### **🔄 Saving Difficulty Data (Persists After Refresh)**
![Save Difficulty Settings](https://github.com/eeeyooon/portfolio/assets/102462534/35e6adb1-ec53-4cf3-9d07-10e168c7d4ab)

- **`redux-persist`** is used to store **Redux state** in **localStorage**.
- Even after refreshing the browser, **the selected difficulty settings remain**.

---

## **📂 Folder Structure**

```
📦src
┣ 📂components
┃ ┣ 📂Board
┃ ┃ ┣ 📜index.tsx
┃ ┃ ┗ 📜styles.ts
┃ ┣ 📂Cell
┃ ┃ ┣ 📜index.tsx
┃ ┃ ┗ 📜styles.ts
┃ ┣ 📂Header
┃ ┃ ┣ 📜index.tsx
┃ ┃ ┗ 📜styles.ts
┃ ┣ 📂Menu
┃ ┃ ┣ 📜index.tsx
┃ ┃ ┗ 📜styles.ts
┃ ┗ 📜index.ts
┣ 📂lib
┃ ┣ 📜constants.ts
┃ ┣ 📜findAroundMine.ts
┃ ┗ 📜initialBoard.ts
┣ 📂slices
┃ ┗ 📜gameSlice.ts
┣ 📂store
┃ ┗ 📜index.ts
┣ 📂style
┃ ┣ 📜global.ts
┃ ┗ 📜theme.ts
┣ 📜App.tsx
┣ 📜index.tsx
┗ 📜react-app-env.d.ts
```

---

## **📦 Libraries Used**

```
"dependencies": {
  "@reduxjs/toolkit": "^2.0.1",
  "@testing-library/jest-dom": "^5.17.0",
  "@testing-library/react": "^13.4.0",
  "@testing-library/user-event": "^13.5.0",
  "@types/jest": "^27.5.2",
  "@types/node": "^16.18.67",
  "@types/react": "^18.2.42",
  "@types/react-dom": "^18.2.17",
  "@types/react-redux": "^7.1.32",
  "react": "^18.2.0",
  "react-dom": "^18.2.0",
  "react-redux": "^9.0.2",
  "react-scripts": "5.0.1",
  "redux": "^5.0.0",
  "redux-persist": "^6.0.0",
  "styled-components": "^6.1.1",
  "styled-reset": "^4.5.1",
  "typescript": "^4.9.5",
  "web-vitals": "^2.1.4"
}
```

---

🚀 **This Minesweeper project provides a fully interactive and customizable gameplay experience, with state persistence and difficulty settings, ensuring an engaging and dynamic user experience.** 🎮🔥
