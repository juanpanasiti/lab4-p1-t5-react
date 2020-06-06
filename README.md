# Preparación del proyecto
Esta etapa es común a todos los proyectos, es opcional y no depende de qué es lo que se vaya a desarrollar.  

## Creación del proyecto
`npx create-react-app`

## Instalar librerías
-  **Boostrap:** Para utilizar componentes de [React Bootstrap](https://react-bootstrap.github.io/components/alerts)
`$ npm install react-bootstrap bootstrap`
-  **Router DOM:** Para manejar las rutas dentro de la app
`$ npm install react-router-dom`

## Preparar la estructura del proyecto
### Crear carpetas (dentro de `src`)
- `components` para colocar todos los componentes
- `assets/images` para colocar las imágenes estáticas
- `assets/css` para las hojas de estilo
- `assets/json` para los archivos JSON (solo en caso de necesitar trabajar con estos archivos, sino no hace falta)
### Eliminar archivos innecesarios
- `App.test.js`
- `logo.svg`
- `setupTest.js`
### Mover archivos
- Mover `App.css` y `index.css` a `assets/css`
### Corregir errores producidos
Los archivos eliminados o cambiados de lugar han dejado errores en el código, por lo tanto hay que corregirlos:
- En `App.js`:
  - Cambiar el import del css por `import './assets/css/App.css';`
  - Eliminar el import del logo (`import logo from './logo.svg';`)
  - De paso, borrar todo el contenido del div principal para que quede asi:
```
  <div className="App">
    Acá va al contenido de la app  
  </div>
```
- En `index.js`:
  - Cambiar el import del css por `import './assets/css/index.css';`
- En `App.css` borrar todo el contenido de estilos

***Hecho esto ya queda todo el esqueleto de la app listo para empezar casi cualquier proyecto***

# Resolviendo el ejercicio
