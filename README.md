>> Tailwind-css installation


>> Terminal 
```

npm init -y
```

npm install -D tailwindcss postcss autoprefixer vite
```

npx tailwindcss init -p
```


>> Add this code CSS file /style.css
```
@tailwind base;
@tailwind components;
@tailwind utilities;
```

>> Change tailwind.config.js
>> Add * from content / that means all cover all file
```
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ['*'],
  darkMode: 'class',
  theme: {
    extend: {},
  },
  plugins: [],
}
```

>> Add script packege.json file
```
  "scripts": {
    "start": "vite",
    "build": "tailwindcss -i ./css/tailwind.css -o ./css/style.min.css --minify",
    "watch": "tailwindcss -i ./css/tailwind.css -o ./css/style.min.css --watch",
    "dev": "vite build"
  },
```


>> Terminal 
..........

>> Run Projects from vit
```
npm run start
```
>> Build Custom CSS Folder
```
npm run build
```

>> Build Projcts Form Vite / dist folder
```
npm run dev
```

>> Watch Custom CSS Folder
```
npm run watch
```