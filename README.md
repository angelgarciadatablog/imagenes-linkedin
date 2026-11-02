# imagenes-linkedin

Imágenes que genera el bot de LinkedIn de Ángel García (repo privado `proyecto-linkedin-publicaciones-angel`).
Cada noticia tiene su imagen en `noticias/<id>.png`; el Google Sheet del bot guarda su link en la columna `imagen`:
`https://raw.githubusercontent.com/angelgarciadatablog/imagenes-linkedin/main/noticias/<id>.png`.

## Por qué un repo aparte

El bot sube las imágenes solo, desde un servidor, con un token de GitHub. Ese token tiene
permiso de escritura **únicamente sobre este repo**. Si se filtrara, no podría tocar las
imágenes de la web, que viven en [`imagenes`](https://github.com/angelgarciadatablog/imagenes)
y que ningún programa automático puede modificar.

## Reglas

- **Nunca se usa para la web.** Las imágenes de angelgarciadatablog.com van en `imagenes`.
- **Es público a propósito:** el link del Sheet tiene que abrirse sin iniciar sesión, y estas
  imágenes igual terminan públicas en LinkedIn.
- **Solo escribe el bot.** Si una imagen está mal, se corrige en el Sheet y el bot la vuelve a generar.
