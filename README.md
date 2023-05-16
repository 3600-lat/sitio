# Sitio 3600.lat

htts://3600.lat

## Instalación

```
git clone https://github.com/3600-lat/sitio.git
cd sitio
git submodule init
git submodule update
```

## Desarrollar

### Simple

Para personalizar JS y CSS, tocar:

- [static/css/custom.css](static/css/custom.css)
- [static/js/custom.js](static/js/custom.js)

Y para ver los cambios, en una terminal:

```
hugo server
```

### Avanzado

Para usar SCSS, se requiere recompilar el CSS:

```
cd themes/minimo
npm install
npm run build
```

Y para ver los cambios, en otra terminal:

```
npm run-script watch
```

