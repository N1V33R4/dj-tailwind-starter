Tailwind will build and output to a CSS file. Add that to base.html and call it a day.  

Of course, you need to configure:
- Where tailwind styles are being used. 
- Where output file will stay. 

Install: `npm install -D tailwindcss`  
Init: `npx tailwindcss init`  
Create input/output files: static/css/tailwind-input.css,tailwind-output.css  
Reference in `package.json`:  
Add @tailwind to input:   
Run dev script: `npm run dev`  
```json
"scripts": {
  "dev": "tailwindcss -i static/css/tailwind-input.css -o static/css/tailwind-output.css --watch"
},
```
Add html files path in `tailwind.config.js`: `content: ["./templates/**/*.html"],`  

Enjoy building with tailwind :)  
How do I deploy this though?  

We can extend the base tailwind classes with our own colors and stuff.  
Flowbite has prebuilt tailwind components?!  

