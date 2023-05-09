## Goal of the Project:
- Use borders and box-shadow utility classes.
- Working of hover modifier in <a href="https://tailwindcss.com/" target="_blank" rel="noopener noreferrer"> Tailwind CSS.</a>
- Build a simple web page with flexbox utility classes.

## Additional Goal:
- Hosting through the Firebase platform

<img width="671" alt="Screenshot 2023-05-09 at 8 39 13 PM" src="https://github.com/Swap-Nova/Tailwind-CSS_Features/assets/92979885/9b7e4673-961c-4969-93bf-26b88539ef92">

### Setting up the workplace:
```bash
npm -y init
```

- Now, we will install the tailwind CLI tool as a devDependency, which means that the Tailwind CLI tool is a package only required during the development. Enter the following command in your terminal.
```bash
npm install -D tailwindcss
```
- The terminal will load the installation of the packages. Now, open your package.json file and check that 'tailwindcss' appears as a devDependency, which you should find in lines 12 and 13.
- Now that the Tailwind CLI tool is installed, we can run it by entering the following command in your terminal.
```bash
npx tailwindcss init
```
- In the tailwind.config.js file, update the “content” property in line 3 with the following code:
```bash
content: ["./src/**/*.{html,js}"],
```
- Finally, enter the following code in the input.css file. 
```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```
- How to start Tailwind:
We need to build the utility classes using the Tailwind CLI Tool. Open the terminal and enter the following command:
```bash
npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch
```

PS: The terminal will now rebuild only the utility classes used in your code every time you save new changes. Thereafter, leave your terminal open during your development.
