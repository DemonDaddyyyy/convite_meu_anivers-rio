Comandos pra dar nos pcs que editarem o código:
npm init --yes
npm install --save-dev parcel

quando acionar o parcel, colocar ele no script do package.json:
"dev": "parcel src/index.html src/styles/main.scss src/scripts/main.js",

npm run dev -> vai surgir uma pasta chamada .parcel-cache e outra chamada dist.

Hotreload ao invés de usar o liveserver. É só pegar o link que a linha de comando devolve depois de digitar npm run dev e lá vai estar o site.

sharp.config.json pra comprimir as imagens. Depois de colocar o comando no sharp, rodar na linha de comando o npm run dev. As imagens só serão comprimidas sob demanda.
{
    "png": {
        "quality": 75
    }
}

Para importar o sass pelo parcel não é preciso compilar, ou seja, não é preciso criar um main.scss que depois compilado vira main.scss. Coloca logo no head do html o main.scss.

ANTES DO PRIMEIRO COMMIT CRIAR .GITIGNORE: 
.parcel-cache
dist
node-modules

QUICK GIT SETTINGS FOR EASY PC'S CHANGE:

git init
git add .
git commit -m "commit inicial"
git remote add origin https://github.com/DemonDaddyyyy/convite_meu_anivers-rio.git
git branch -M main
git push -u origin main

Esse é o setup, agora é só construir o site.    <3