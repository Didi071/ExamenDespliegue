# Cración del proyecto

## Instalación del Proyecto

Se crea con `git init` que crea un repo local
Luego se debería crear la rama main y esta se guarda con un commit porque si no no se guarda. Okey, luego cambias a la develop que sería el hilo principal del programa y las features que son las especificas. Y luego las release para los test antes de ir a la main.

## Documentación y Tests

En la terminal iniciamos un nuevo proyecto e instalamos las dependencias necesarias

```bash
nmp init -y

npm install --save-dev jsdoc jest-environment-jsdom jest
```

En el package.json añadimos lo siguiente

```json
"scripts": {
"test": "jest",
"doc": "jsdoc -r -d docs ."
}
```
