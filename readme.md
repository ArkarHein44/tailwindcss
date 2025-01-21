# Install Tailwind
firstly you need to install node.js and npm in your system.
Install tailwindcss via npm, and create your tailwind.config.js file.
```shell
# node_modules
npm install -D tailwindcss

# tailwind.config.js
npx tailwindcss init
```

# in tailwind.config.js
```javascript
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js,jsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

# run tailwind watcher
```shell
npx tailwindcss -i ./src/input.css -o ./src/output.css --watch
```

`npx tailwindcss` means tailwindcss cli run on npm
<br/>

`-i` i flag for input directory
<br/>

`-o` o flag for output directory
<br/>

`--watch` watch flag tells the tailwind cli for changes in your input