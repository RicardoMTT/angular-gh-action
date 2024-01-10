


Explicación workflow de github actions
1.uses: actions/checkout@v2: Hace checkout del código fuente de la rama actual. Obtenemos el código para poder construirlo.

2.uses: actions/setup-node@v3: Configura Node.js en la versión 14 para poder ejecutar npm.

3.run: npm install: Ejecuta npm install para instalar todas las dependencias definidas en el package.json.

4.run: npm run deploy: Ejecuta el script deploy definido en los scripts de npm en package.json

5.uses: AhsanAyaz/angular-deploy-gh-pages-actions@v1.3.1: Utiliza una acción de GitHub hecha específicamente para desplegar apps Angular a GitHub Pages.los despliega a la rama gh-pages para que queden disponibles en GitHub Pages.
