# Marinas Consulting — Web nueva (Netlify + GitHub)

Diseño base cerrado con el cliente: cabecera con logo grande a la izquierda, menú a la derecha, hero con video a pantalla completa, 5+5 tarjetas con segunda fila centrada, color #F5E7BF, grises para fondo claro.

## Archivos
- index.html -> página principal
- images/logo-oscuro.png -> logo #F5E7BF para fondos oscuros
- images/logo-claro.png -> logo grises para fondos claros
- images/COMO-CAMBIAR-FOTOS.txt -> cómo cambiar fotos y video
- posts.json -> entradas del blog (editar desde GitHub)
- admin/ -> panel para publicar en /admin/ (Decap CMS)

## 1. Subir a GitHub (Windows, desde el navegador)
1. Entra en github.com/imarinas73/imarinas-web
2. Si el repositorio está vacío, pulsa "uploading an existing file" o Add file > Upload files
3. Arrastra todos los archivos de este ZIP tal cual: index.html, posts.json, carpeta images/, carpeta admin/
4. Pulsa Commit changes

Si ya hay archivos viejos, bórralos antes o sustitúyelos con los nuevos con el mismo nombre.

## 2. Conectar Netlify (gratis)
1. Entra en netlify.com > Sign up > Sign up with GitHub (usa imarinas73) > Authorize
2. Add new site > Import an existing project > GitHub > elige imarinas-web
3. Branch: main, Build command: (vacío), Publish directory: (vacío o .)
4. Deploy site. Te dará una dirección temporal tipo imarinas-web.netlify.app
5. Cada vez que subas un cambio a GitHub, Netlify publica sola en 1 minuto.

## 3. Publicar en el blog (lo más simple)
Opción A - desde GitHub: abre posts.json > lápiz Edit > añade una entrada con título, fecha, categoría, resumen > Commit. Listo.
Opción B - desde /admin/: entra en tu-dominio.netlify.app/admin/ > New Blog > escribe > Publish. Necesita activar Netlify Identity + Git Gateway en Netlify > Site settings > Identity.

## 4. Cambiar fotos, video, textos
Ver images/COMO-CAMBIAR-FOTOS.txt

## 5. Dominio (SOLO AL FINAL)
Cuando la web temporal se vea perfecta, pide a la empresa que gestiona imarinas.es que cambie el DNS a Netlify, SIN tocar los registros MX del correo. En Netlify: Site settings > Domain management > Add a domain > imarinas.es > te dirá los registros a poner. No canceles SiteGround hasta que imarinas.es ya muestre la nueva web.

## 6. Contacto
El formulario usa Netlify Forms, funciona solo cuando está publicado en Netlify. Los mensajes llegan a Netlify > Forms.
