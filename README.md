# Proyecto Node-RED — módulo 6

Dashboard educativo de un motor simulado con imagen SVG integrada,
botones MARCHA/PARADA y LED de estado. No acciona equipos reales.

## Abrir como proyecto de Node-RED

1. Tener Node.js, Node-RED y Git instalados.
2. En el `settings.js` del directorio de usuario, habilitar:

   ```js
   editorTheme: { projects: { enabled: true } }
   ```

3. Reiniciar Node-RED. En el menú Projects > New, elegir clonar un
   repositorio e introducir la URL de este repositorio.
4. Instalar `node-red-dashboard` 3.6.5, definido en `package.json`.
   Este proyecto utiliza el dashboard clásico del ejercicio.
5. Abrir el proyecto, pulsar Deploy y visitar `/ui` en el servidor.

## Comprobación

- Estado inicial: DETENIDO, LED gris.
- MARCHA: estado EN MARCHA, LED verde y eje animado.
- PARADA: estado DETENIDO, LED gris y eje quieto.
- Al conectar un navegador, el flujo sincroniza el estado vigente.

Se verificaron el JSON, las conexiones y la lógica del nodo Function
en JavaScript. La ejecución completa y la clonación desde la interfaz
Projects de Node-RED aún deben comprobarse en una instalación local.

## Archivos y credenciales

`flows.json` es el archivo de flujos. `package.json` declara la dependencia
y los nombres de los archivos del proyecto. No se incluyen credenciales,
tokens ni configuraciones de una instalación personal. La configuración
de usuarios del ejercicio 1 se entrega por separado a la plataforma.

Documentación: https://nodered.org/docs/user-guide/projects/
