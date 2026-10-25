# Assignment 1.2 — Solution: Development Environment Setup

## 1. Install Visual Studio Code
1. Go to https://code.visualstudio.com and download the installer for your OS.
2. Run the installer. On Windows, tick **"Add to PATH"** and **"Open with Code"** options.
3. Launch VS Code to confirm it opens.

## 2. Install Node.js (LTS)
1. Go to https://nodejs.org and download the **LTS** version.
2. Run the installer with the default options (this also installs **npm**).
3. Restart the terminal/VS Code after installation.

## 3. Install VS Code Extensions
1. Open VS Code and click the **Extensions** icon (or press `Ctrl + Shift + X`).
2. Search **Live Server** (by Ritwick Dey) → **Install**.
3. Search **Prettier - Code formatter** → **Install**.
4. (Optional) Enable *Format On Save* in Settings and set Prettier as the default formatter.

## 4. Create the Project Folder
Create a folder named `web-development-practice` and open it in VS Code (**File → Open Folder**).

Or via terminal:
```bash
mkdir web-development-practice
cd web-development-practice
code .
```

## 5. Create the Files
Inside the folder create `index.html`, `style.css`, `script.js`:

```bash
touch index.html style.css script.js      # macOS/Linux
type nul > index.html & type nul > style.css & type nul > script.js   # Windows (cmd)
```

**index.html**
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Web Development Practice</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <h1>Hello, World!</h1>
    <p>My development environment is set up successfully.</p>
    <script src="script.js"></script>
  </body>
</html>
```

**style.css**
```css
body {
  font-family: Arial, sans-serif;
  text-align: center;
  margin-top: 50px;
  background-color: #f4f4f4;
}

h1 {
  color: #2c3e50;
}
```

**script.js**
```javascript
console.log("Hello from script.js — environment is working!");
```

## 6. Run with Live Server
1. Open `index.html` in VS Code.
2. Right-click in the editor → **Open with Live Server** (or click **Go Live** in the bottom-right status bar).
3. The browser opens at `http://127.0.0.1:5500/index.html`. Edit and save the file to see it auto-reload.

## 7. Verify Node.js and npm
Open the terminal in VS Code (`Ctrl + ` `) and run:
```bash
node -v
npm -v
```
Expected output: version numbers such as `v22.x.x` and `10.x.x` (yours will depend on the installed LTS).

## Submission Screenshots
- 📸 **VS Code** showing the `web-development-practice` folder with the three files open
- 📸 **Terminal** showing the output of `node -v` and `npm -v`
- 📸 **Browser** showing the page running via Live Server (`127.0.0.1:5500`)
