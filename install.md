- npm init -y

- npm install -D tailwindcss

- npx tailwindcss init
gera o arquivo tailwind.config.js

- No tailwind.config.js <- identificar o arquivo html
content: ["./public/*.html"],

- Criar os arquivos STYLE.CSS e TAILWIND.CSS
    color no STYLE.CSS   
        @tailwind base;
        @tailwind components;
        @tailwind utilities;

- identifica o caminho dos arquivos css e fica observando eles
npx tailwindcss -i ./public/css/style.css -o ./public/css/tailwind.css --watch 

- Em PACKAGE.JSON ir em  "scripts"  <--E alterar para-->
"scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
        <--E alterar para-->
"scripts": {
    "dev": "npx tailwindcss -i ./public/css/style.css -o ./public/css/tailwind.css --watch"
  },

- ir no INDEX.HTML e fazer o link com os arquivos CSS

- instalar a extensão do VS 
Tailwind CSS IntelliSense