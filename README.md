I have Used Tailwind CSS In This Project......
If SomeOne wants To Use CSS TRY THis....

1. install The Node.js...
2. if you have Node.js then Open Terminal... and Run this command------
3. Create a Folder.. this command create a folder on desktop...
```
mkdir "Your Folder Name"
```
4.it will config the Tailwind CSS on that folder 
```
npx tailwindcss init

```
5.create a Src folder on the previous folder and create a file input.css and paste the below properties.
```
@tailwind base;
@tailwind components;
@tailwind utilities;
```

6. Create a dist Folder on your Previous Folder and Create two File....
```
index.html
```
```
output.css
```
7. link a css in html file...
```
<link rel="stylesheet" href="./output.css">
```
8. Now go to tailwind.config.js and give a path the where is your html on the component tag...

```
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./dist/*.html"],
  theme: {
    extend: {},
  },
  plugins: [],
}

```
9. After this Run One More Command On Terminal....
```
npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch
```

10. Now you can use tailwind css on your html ..... ex---
```
<h1 class"bg-red-200">This is The Proper Way To Use Tailwind CSS</h1>
```

---------------------------------------------------------------------------------------------------------------