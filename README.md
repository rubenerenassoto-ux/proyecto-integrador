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

He usado ChatGPT en dos momentos, y en los dos casos los cambios los he hecho yo a mano:

1. **Menú en el móvil.** Le pasé el CSS del `header` y del menú y le pregunté cómo hacer que se viera bien en pantallas pequeñas. Me propuso una media query (`@media (max-width: 600px)`) que pone el título y el menú uno debajo del otro (`flex-direction: column`), los centra y reduce el margen de los enlaces. La apliqué y además le bajé el `padding` del header a 15px, porque 30px a los lados en el móvil era mucho. Commit: "Adapta el menú a pantallas pequeñas".
2. **Revisión del formulario de contacto.** Le pasé el formulario de `contacto.html` para que lo revisara. Me dijo que no había errores graves y que los `label` ya estaban bien asociados con `for` e `id`, y me sugirió tres cosas: poner `required` en los campos, un `placeholder` en el mensaje y `autocomplete` en nombre y correo. Puse el `required` y el `placeholder`. El `autocomplete` lo dejé fuera para no complicar el formulario. Commit: "Marca como obligatorios los campos del formulario".

Antes de cada commit revisé el cambio con `git diff` para comprobar que solo entraba lo que yo quería.

## Decisiones

- Crear el `.gitignore` al principio para no subir nunca un `.env` o un log por error.
- Hacer un commit por cada parte del proyecto para que el historial se entienda.
- Hacer la página de contacto en la rama `feature/contacto` y meterla en `main` con una Pull Request, después de revisar "Files changed".

## Autoría

Rubén - 2º ASIR
