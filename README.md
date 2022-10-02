# tailwindcss-tutorial

> Tailwind CSS Tutorial Course followed by Dave Gray

## Initial setting for Tailwind CSS

### 1. Install Node.js

https://nodejs.org/ko/download/

### 2. Check your Node.js version

Type on terminal

```
node -v
```

### 3. Install "Live Server" extension

### 4. Set and make enable "Live Server > Settings: Full Reload"

Click the gear icon on "Live Server" extension

Click "extension setting"

Type "full reload" and turn on the checkbox

### 5. Install "tailwind.config.js"

Type command line on Ternimal

```
npx tailwindcss init
```

### 6. Make directories.

Create "build" and "src" folders

Create "index.html" file in "build" folder

### 7. Tell Tailwind where HTML file

In "tailwind.config.js", find "content: []"

Type below

```
'./build/*.html'
```

### 8. Create "input.css" file in "src" folder

Paste this lines

```
@tailwind base;
@tailwind components;
@tailwind utilities;
```

\[Note\]

To remove the error "Unknown at rule @tailwind ..." on Problems, type "unknown" and find "CSS > Lint: Unknown At Rules" option.

Open the bar and set "ignore" option.

### 9. Download Tailwind CSS Styles file

Type below on Terminal

```
npx tailwindcss -i ./src/input.css -o ./build/css/style.css
```

### 10. Connect style.css to index.html

Insert link element on index.html

```
<link rel="stylesheet" href="css/style.css">
```

### 11. Set Live Server keep tracking the change of index.html, which is adjusted by Tailwind CSS

Type below on Terminal

```
npx tailwindcss -i ./src/input.css -o ./build/css/style.css --watch
```

### 12. Now you can check the HTML file, which is applied Tailwind CSS style on live.

------------------------

## Useful Tailwind CSS Extension App

### 1. Tailwind CSS IntelliSense

### 2. Inline fold
