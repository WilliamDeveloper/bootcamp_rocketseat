# nlw3_trilha_omnistack
nlw3_trilha_omnistack

#---------------------------------
# markdown passos
#---------------------------------

#---------------------------------
#  criando projeto react
#---------------------------------
cd /c/nlw
yarn create react-app web --template typescript
# ou npx vem com node instalado
npx create-react-app web --template typescript

cd /c/nlw/web
code .

#  adicionando icones no react
cd /c/nlw/web
yarn add react-icons

#  adicionando rotas no react - modulo react-router-dom
cd /c/nlw/web
yarn add react-router-dom
yarn add @types/react-router-dom -D

# adicionando mapas na aplicacao
yarn add leaflet react-leaflet
yarn add @types/leaflet -D
yarn add @types/react-leaflet -D


# criar arquivo .env ( apos modificar o .env de restart na aplicacao "yarn start" )
# https://www.mapbox.com/
# https://docs.mapbox.com/mapbox-gl-js/api/map/
cd /c/nlw/web
touch .env
REACT_APP_MAPBOX_TOKEN=pk.eyJ1IjoiZ3Rhc2t3aWxsIiwiYSI6ImNrZ3BkdXlhNzE2djUyeHA5bHE1NzkwbTUifQ.gZxYxgpF0M6pG8C2JBu1zQ

# adicionar no .gitignore
.env

#---------------------------------
#  limpando projeto react
#---------------------------------
rm /c/nlw/web/public/*.png
rm /c/nlw/web/public/*.txt
rm /c/nlw/web/public/*.json
rm /c/nlw/web/public/*.ico

rm /c/nlw/web/src/App.test.tsx
rm /c/nlw/web/src/*.css
rm /c/nlw/web/src/*.svg
rm /c/nlw/web/src/serviceWorker.ts
rm /c/nlw/web/src/setupTests.ts

#---------------------------------
#  subindo o projeto
#---------------------------------
cd /c/nlw/web
yarn start