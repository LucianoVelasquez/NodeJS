## Iniciando Projecto
~~~
npm i typescript -D
~~~
Copilador de typescript: (Crea un archivo para configurar ts)
~~~
npx tsc --init
~~~
__tsconfig.json:__
* outDir: __"./dist"__
* rootDir: __"./src"__
## Otas dependencias
__express__
~~~
npm i express 
~~~
__Instalando typos de datos para TS (los tipos se instalan siempre en desarrollo)__
~~~
npm i @types/express -D
~~~
__(Antes de instalar otras dependencias ejecutar npx tsc)__
__dependencias para escuchar el archivo de JS y TS__ (concurrently sirve para ejecutar multyples comandos)
~~~
npm i nodemon concurrently -D
~~~
__Configuracion:__
* __"dev"__: "concurrently \"tsc --watch\" \"nodemon dist/index.js\""
(tsc --watch va estar atento a los cambios de los archivos ts)
## Estructura de carpeta
* __src__
 * 