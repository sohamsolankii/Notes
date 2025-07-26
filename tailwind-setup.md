## How to setup Tailwind CSS

Step 1: Run the following commands

``` 
npm install -D tailwindcss
npx tailwindcss init
```

Step 2: Update tailwind.conf.js file to include this line:
```
content: ["*.{js,ts,jsx,tsx}"],
```

Step 3: create src/input.css to include:
```
@tailwind base;
@tailwind components;
@tailwind utilities;
```

Step 4: Include the src/output.css file to your html

Step 5: Run the following command:
```
npx tailwindcss -i ./src/input.css -o ./src/output.css --watch
```

-> Behalf of running step-5 i can add sctipr in package.json

```
"script":{
    "bulild": "npx tailwindcss -i ./src/input.css -o ./src/output.css --watch"
}

now run this in terminal: npm run build
```