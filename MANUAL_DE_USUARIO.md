# Manual de usuario — Agente Inmobiliario IA

Este manual explica, paso a paso y sin conocimientos previos, cómo instalar el agente en Claude o en Codex y cómo usarlo.

## 1. Qué es el agente

Es un asistente comercial con inteligencia artificial para inmobiliarias. Se le escribe como a una persona y responde como lo haría alguien del equipo:

- Atiende consultas al instante.
- Informa las propiedades del catálogo: características, precio, zona y disponibilidad.
- Averigua qué busca cada persona: tipo de propiedad, zona, presupuesto, si quiere comprar, alquilar o invertir, en qué plazo y si necesita financiación.
- Clasifica a cada contacto: comprador, inquilino, propietario que vende o alquila, inversor o consulta general.
- Toma pedidos de visita.
- Prepara la ficha del interesado para el asesor.
- Redacta los mensajes de seguimiento.

El agente no inventa datos. Si algo no está cargado, responde «No lo tengo confirmado».

## 2. Qué necesitás

- Una computadora con Windows, Mac o Linux, y conexión a internet.
- Una cuenta paga de **Claude** (para usar Claude Code) o de **ChatGPT** (para usar Codex). Con una de las dos alcanza.
- La dirección del agente: `https://github.com/Agustin3030/agente-inmobiliario-ia`

Hay dos formas de instalarlo. Elegí una:

- **Opción A, desde el navegador:** no se instala nada en la computadora. Es la más simple.
- **Opción B, en la computadora:** requiere instalar tres programas, una sola vez.

## 3. Opción A: usarlo desde el navegador

Paso 1. Entrá a github.com e iniciá sesión. Si no tenés cuenta, creá una: es gratuita.

Paso 2. Abrí la dirección del agente y tocá el botón **Fork**, arriba a la derecha. Después tocá **Create fork**. Esto crea una copia del agente en tu cuenta, que es la que vas a usar.

Paso 3. Abrí la herramienta que tengas:

- Con Claude: entrá a claude.ai/code.
- Con Codex: entrá a chatgpt.com/codex.

Paso 4. La primera vez te va a pedir conectar tu cuenta de GitHub. Aceptá y dale acceso al repositorio `agente-inmobiliario-ia`.

Paso 5. Elegí el repositorio `agente-inmobiliario-ia` como proyecto.

Paso 6. Escribí tu primer mensaje. Seguí en la sección 5.

## 4. Opción B: instalarlo en la computadora

### 4.1. Instalar los programas (una sola vez)

Paso 1. Instalá **Node.js** desde nodejs.org. Elegí la versión que dice LTS y aceptá las opciones que vienen marcadas.

Paso 2. Instalá **Git** desde git-scm.com. Aceptá las opciones que vienen marcadas.

Paso 3. Abrí la terminal:

- En Windows: abrí el menú Inicio, escribí `PowerShell` y abrilo.
- En Mac: abrí Spotlight, escribí `Terminal` y abrilo.

Paso 4. Instalá la herramienta que vayas a usar. Copiá el comando, pegalo en la terminal y apretá Enter.

Para Claude:

```bash
npm install -g @anthropic-ai/claude-code
```

Para Codex:

```bash
npm install -g @openai/codex
```

### 4.2. Descargar el agente (una sola vez)

Paso 5. Copiá este comando, pegalo en la terminal y apretá Enter:

```bash
git clone https://github.com/Agustin3030/agente-inmobiliario-ia.git agente-inmobiliario
```

Esto crea una carpeta llamada `agente-inmobiliario` con todo el agente adentro.

### 4.3. Abrir el agente (cada vez que lo quieras usar)

Paso 6. Entrá a la carpeta del agente:

```bash
cd agente-inmobiliario
```

Paso 7. Abrí la herramienta. Escribí una de estas dos palabras y apretá Enter:

```bash
claude
```

```bash
codex
```

Paso 8. La primera vez te pide iniciar sesión. Se abre el navegador, entrás con tu cuenta y volvés a la terminal. Si pregunta si confiás en la carpeta, respondé que sí.

Listo. Ya podés escribirle.

Las próximas veces solo hacés el paso 3 (abrir la terminal), el 6 y el 7.

## 5. Cómo usarlo

Se usa como un chat: escribís un mensaje, apretás Enter y el agente responde.

### 5.1. Primera prueba

Escribí estos mensajes, uno por vez, en este orden:

1. `Hola, busco un terreno de 200 metros cuadrados`
   El agente busca en el catálogo y te ofrece lo que coincide.

2. `Quiero comprar, tengo hasta USD 30.000 y quiero resolverlo este mes`
   Registra tus datos y pregunta solo lo que le falta.

3. `Quiero visitarlo el sábado a la mañana`
   Toma tu preferencia y aclara que el equipo debe confirmar el horario.

4. `Sí, que me contacte un asesor por WhatsApp`
   Prepara la derivación con tus datos.

5. `RESUMEN DEL PROSPECTO`
   Muestra la ficha del cliente, como la vería el equipo.

6. `SEGUIMIENTO PARA DEMO-001`
   Redacta los mensajes para volver a escribirle al cliente.

### 5.2. Ver una demostración completa

- `Hacé la demo`: muestra una conversación completa de ejemplo.
- `Demo en vivo`: el agente hace de agente y espera cada respuesta tuya, para que hagas de cliente.

### 5.3. Preguntarle qué sabe hacer

- `¿Qué podés hacer?`
- `¿Qué propiedades tenés cargadas?`
- `MOSTRÁ ESTADO DE INTEGRACIONES`

### 5.4. Usarlo como ayudante del equipo

Podés pegarle el mensaje de un cliente y pedirle la respuesta:

`Un cliente me escribió por WhatsApp: "Hola, ¿tienen casas en zona norte hasta 100 mil dólares?". Redactame la respuesta.`

El agente redacta el mensaje para que lo copies y lo envíes vos.

## 6. Cómo cargar tus propios datos

En esta versión los cambios quedan guardados en los archivos del agente. El agente siempre muestra el cambio y pide confirmación antes de guardar. Si la herramienta te pide permiso para modificar un archivo, aceptalo.

### 6.1. Datos de la inmobiliaria

Escribí, por ejemplo:

- `CONFIGURAR LOCAL: NOMBRE_INMOBILIARIA = Inmobiliaria Ejemplo`
- `CONFIGURAR LOCAL: LOCALIDADES_Y_ZONAS = Cipolletti y Neuquén`
- `CONFIGURAR LOCAL: MONEDAS_DE_OPERACIÓN = USD para venta, ARS para alquiler`

### 6.2. Propiedades

- Agregar: `NUEVA PROPIEDAD: casa de 3 dormitorios en zona sur, 110 m² cubiertos, USD 120.000, en venta`
- Cambiar un dato: `ACTUALIZAR PROPIEDAD DEMO-001: precio USD 30.000`
- Marcar como vendida o alquilada: `PROPIEDAD DEMO-003 VENDIDA`

### 6.3. Respuestas y asesores

- Enseñarle una respuesta: `APRENDÉ ESTA RESPUESTA: ¿Aceptan mascotas? => Depende de cada propiedad; te confirmo en cada caso.`
- Agregar un asesor: `NUEVO ASESOR: Laura Pérez, zona centro, ventas`
- Dar una regla nueva: `A PARTIR DE AHORA: las visitas son de lunes a viernes de 9 a 18`

### 6.4. Pasar de la demostración a datos reales

El agente viene con diez propiedades ficticias, con códigos que empiezan con `DEMO-`, y avisa que son ejemplos. Para usarlo con clientes reales:

1. Pedile: `Eliminá todas las propiedades DEMO del catálogo`.
2. Cargá tus propiedades con `NUEVA PROPIEDAD`.
3. Pedile: `Quitá el aviso de modo demostración del catálogo y de las instrucciones`.

## 7. Qué no hace

- No envía mensajes por WhatsApp, Instagram ni Facebook. Redacta las respuestas para que una persona las envíe.
- No reserva visitas en un calendario. Toma la preferencia y el equipo confirma.
- No recuerda conversaciones anteriores. Cada vez que abrís la herramienta empieza una conversación nueva; lo que sí queda guardado son los datos cargados en los archivos.
- No reemplaza el asesoramiento legal, impositivo ni una tasación profesional.

## 8. Problemas frecuentes

**«npm no se reconoce como un comando» o «git no se reconoce como un comando».**
Falta instalar Node.js o Git. Si ya los instalaste, cerrá la terminal y volvé a abrirla.

**El agente responde como un programador y no como un asistente inmobiliario.**
No estás dentro de la carpeta del agente. Cerrá la herramienta, escribí `cd agente-inmobiliario` y volvé a abrirla. En el navegador, revisá que el proyecto elegido sea `agente-inmobiliario-ia`.

**Dice que no tiene propiedades.**
Preguntale `¿Qué propiedades tenés cargadas?`. Si responde que ninguna, pedile `Leé el archivo conocimiento/03_CATALOGO_PROPIEDADES.md`.

**Pide un plan pago.**
Claude Code y Codex requieren una suscripción de Claude o de ChatGPT.

**Pide permiso para ejecutar o modificar algo.**
Para leer y editar los archivos del agente, aceptá. Si pide ejecutar comandos o instalar programas, rechazá: el agente no los necesita.

**Quiero volver a los datos originales.**
En la terminal, dentro de la carpeta del agente, escribí `git checkout .` y apretá Enter. Se pierden todos los cambios que hayas cargado.

## 9. Preguntas frecuentes

**¿Mis datos los ve otra persona?**
No. Cada persona trabaja con su propia copia del agente y con su propia cuenta.

**¿Puedo usarlo en el celular?**
Con la opción A, desde el navegador, sí. La opción B es para computadora.

**¿Tiene costo?**
El agente no. Lo que se paga es la suscripción de Claude o de ChatGPT de cada persona.

**¿Puedo probarlo sin instalar nada y sin cuenta?**
Sí, pedí el link de la página de demostración a quien te envió este manual.

## 10. Qué contiene la carpeta del agente

- `AGENTS.md` y `CLAUDE.md`: las instrucciones que leen Codex y Claude.
- `conocimiento/01_PROMPT_MAESTRO.md`: las reglas del agente.
- `conocimiento/02_CONFIGURACION_INMOBILIARIA.md`: los datos de la inmobiliaria.
- `conocimiento/03_CATALOGO_PROPIEDADES.md`: el catálogo de propiedades.
- `conocimiento/04_FAQ_Y_POLITICAS.md`: preguntas frecuentes y políticas.
- `conocimiento/05_RESPUESTAS_ENLATADAS.md`: plantillas de mensajes.
- `conocimiento/06_FICHA_Y_REGISTRO_PROSPECTOS.md`: formato de la ficha del cliente.
- `conocimiento/07_CAPACIDADES_Y_DEMO.md`: capacidades y guion de la demostración.
