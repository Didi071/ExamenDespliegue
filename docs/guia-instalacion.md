# Cración del proyecto

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
