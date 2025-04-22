# Proyecto1

Este proyecto es un servidor MCP (Model Context Protocol) que permite la comunicación entre un cliente y un servidor utilizando herramientas definidas. El archivo principal es `main.ts`, que contiene la configuración y definición del servidor.

## Funcionalidades principales

1. **Creación del servidor**: 
   - Se utiliza la clase `McpServer` para manejar la comunicación entre el cliente y el servidor.

2. **Definición de herramientas**:
   - Actualmente, el servidor incluye una herramienta llamada `fetch-weather` que permite obtener información meteorológica de una ciudad específica.
   - La herramienta utiliza la API de Open-Meteo para buscar la ubicación de la ciudad y obtener el pronóstico del clima.

3. **Transporte**:
   - El servidor escucha las conexiones del cliente a través de un transporte de entrada/salida estándar local (`StdioServerTransport`).

## SDK Utilizado

Este proyecto utiliza el SDK de MCP (Model Context Protocol) para TypeScript, el cual proporciona herramientas y clases necesarias para implementar servidores MCP de manera eficiente.

## Cómo usar

1. Instalar las dependencias necesarias especificadas en `package.json`.
2. Ejecutar el archivo `main.ts` para iniciar el servidor MCP.
3. Interactuar con el servidor utilizando un cliente MCP compatible.

## Dependencias principales

- `@modelcontextprotocol/sdk/server/mcp.js`
- `@modelcontextprotocol/sdk/server/stdio.js`
- `zod`

## Ejemplo de uso

La herramienta `fetch-weather` puede ser utilizada para obtener información meteorológica de una ciudad proporcionando el nombre de la ciudad como parámetro.