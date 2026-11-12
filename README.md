# Agente Inmobiliario Comercial IA

Un asistente comercial para inmobiliarias que funciona dentro de Claude y de Codex. Al abrir esta carpeta con cualquiera de los dos, la herramienta se convierte en el agente: atiende consultas, informa propiedades, califica y clasifica prospectos, toma pedidos de visita, prepara la ficha para el asesor y redacta seguimientos.

Cada persona lo usa con su propia cuenta de Claude o de ChatGPT.

## Usarlo con Claude

**Claude Code en la web o en la app de escritorio:** elegí este repositorio (o esta carpeta) como proyecto y empezá a escribir.

**Claude Code en la terminal:**

```bash
git clone https://github.com/Agustin3030/agente-inmobiliario-ia.git agente-inmobiliario
cd agente-inmobiliario
claude
```

Claude lee `CLAUDE.md`, que carga las instrucciones de `AGENTS.md`.

## Usarlo con Codex

**Codex en la web (chatgpt.com/codex):** conectá este repositorio y empezá a escribir.

**Codex en la terminal:**

```bash
git clone https://github.com/Agustin3030/agente-inmobiliario-ia.git agente-inmobiliario
cd agente-inmobiliario
codex
```

Codex lee `AGENTS.md`.

## Qué escribirle

- `Hola, busco un terreno de 200 metros cuadrados` para hablarle como cliente.
- `Hacé la demo` para ver una conversación completa de ejemplo.
- `Demo en vivo` para que el agente espere cada respuesta.
- `¿Qué podés hacer?` para ver sus funciones.
- `RESUMEN DEL PROSPECTO` para ver la ficha del interesado.
- `NUEVA PROPIEDAD: ...` o `PROPIEDAD DEMO-003 VENDIDA` para cambiar el catálogo. El agente muestra el cambio, pide confirmación y lo guarda en el archivo.

## Qué contiene

- `AGENTS.md`: instrucciones del agente (las lee Codex).
- `CLAUDE.md`: carga las mismas instrucciones para Claude.
- `conocimiento/01_PROMPT_MAESTRO.md`: reglas y flujos del agente.
- `conocimiento/02_CONFIGURACION_INMOBILIARIA.md`: datos de la inmobiliaria, para completar.
- `conocimiento/03_CATALOGO_PROPIEDADES.md`: catálogo. Viene con diez propiedades ficticias de demostración.
- `conocimiento/04` a `07`: preguntas frecuentes, plantillas de mensajes, ficha de prospectos, capacidades y demo.

## Para usarlo con datos reales

1. Completar `conocimiento/02_CONFIGURACION_INMOBILIARIA.md`.
2. Reemplazar la tabla de `conocimiento/03_CATALOGO_PROPIEDADES.md` por las propiedades reales y quitar el aviso de modo demostración de ese archivo y de `AGENTS.md`.
3. Completar las respuestas de `conocimiento/04_FAQ_Y_POLITICAS.md`.

## Límites

- No está conectado a WhatsApp, Instagram ni Facebook: no envía mensajes, no agenda y no deriva por su cuenta.
- Las propiedades con código `DEMO-` son ficticias.
- Claude Code y Codex son herramientas pensadas para programar: sirven para usar y ajustar el agente, no para atender al público.
