## Swagger generatror sample

Este es un ejemplo de uso de swagger generator. Hay unos scripts npm para generar un servidor node y clientes de javascript y typescript.

Usando un fichero swagger.json en la carpeta raiz del repo se puede generar el servidor y los clientes.

Esto se puede usar para compartir tus APIs con otros equipos de desarrollo que no tienen acceso físico a las mismas, de forma que el equipo remoto puede incorporar tu api en sus aplicación usando el cliente generado por este ejemplo y probar sus aplicaciones usando el servidor node generado.

### Cómo usar

1. Clonamos este repo con git.
1. Ponemos el fichero `swagger.json` en el raiz del repo, junto al fichero  `package.json`
1. Ejecutar los scripts:
    * `npm run generate-server` genera el servidor node listo para levantarlo y probarlo.
    * `npm run generate-javascript-client` genera el cliente javascript. 
    * `npm run generate-typescript-client` genera el cliente typescript.  
    Ambos, el cliente javascript y typescript, se generan como packages npm pero se puede extraer el cliente api y sus dependencias para incorporarlo a tu proyecto.

### Ampliaciones

Por supuesto que se puede ampliar, se pueden añadir o cambiar los scripts, en la url https://github.com/swagger-api/swagger-codegen/wiki/API-client-generator-HOWTO puedes ver la lista completa de clientes disponibles que se pueden generar.
