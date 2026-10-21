# TecnoRepara

Web sencilla de una tienda de reparación de ordenadores (inventada). Es la práctica integradora de Git y GitHub de IAW, 2º ASIR.

## Archivos

- `index.html`: página principal con los servicios.
- `contacto.html`: página de contacto con un formulario (se hizo en la rama `feature/contacto`).
- `estilos.css`: estilos de todas las páginas.
- `.gitignore`: ignora los archivos `.env` y los `.log`.

## Requisitos

Solo un navegador web. No hace falta servidor ni base de datos.

## Instalación y ejecución

```
git clone https://github.com/rubenerenassoto-ux/proyecto-integrador.git
cd proyecto-integrador
```

Después abrir `index.html` con el navegador.

## Uso de IA

He usado ChatGPT en dos momentos:

1. **Estilos del menú.** Le pregunté cómo hacer que el menú de arriba se viera bien en el móvil. Me propuso usar `display: flex` con `flex-wrap: wrap` en el header y eso es lo que usé, pero los colores, márgenes y tamaños los elegí yo.
2. **Revisión de contacto.html.** Antes de hacer el commit le pasé el `git diff` del formulario para que lo revisara y me diera ideas para el mensaje del commit. Me dijo que las etiquetas `label` no tenían el atributo `for`, lo corregí yo y el mensaje del commit lo elegí yo.

## Decisiones

- Crear el `.gitignore` al principio para no subir nunca un `.env` o un log por error.
- Hacer un commit por cada parte del proyecto para que el historial se entienda.
- Hacer la página de contacto en la rama `feature/contacto` y meterla en `main` con una Pull Request, después de revisar "Files changed".

## Autoría

Rubén - 2º ASIR
