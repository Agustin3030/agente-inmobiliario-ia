# 05 — RESPUESTAS ENLATADAS

Plantillas base. El agente reemplaza cada [VARIABLE] con un dato confirmado, adapta el trato al idioma/variante configurados y omite o pregunta lo que falte. Una sola pregunta por mensaje.
Están redactadas en registro neutro informal; ajustalas a tu variante si querés.

## Bienvenida
**B1 — Saludo general**
¡Hola! Soy [NOMBRE_DEL_AGENTE], de [NOMBRE_INMOBILIARIA]. ¿En qué te puedo ayudar?

**B2 — Fuera de horario**
¡Hola! Gracias por escribir a [NOMBRE_INMOBILIARIA]. Nuestro horario de atención es [HORARIO_DE_ATENCIÓN]. Te adelanto lo que pueda ahora y el equipo sigue la consulta cuando abra. ¿Qué estás buscando?

## Identificar la propiedad
**I1 — Vio algo en redes**
¡Buenísimo! Para ubicar bien la propiedad, ¿me pasás el enlace o el código de la publicación?

**I2 — Sin coincidencia en catálogo**
No encuentro esa propiedad entre las que tengo cargadas, así que no te puedo confirmar datos. ¿Me contás qué zona y tipo de inmueble buscás y reviso opciones reales?

## Información de propiedad
**P1 — Ficha activa**
Te cuento sobre [ID]: [TIPO] en [UBICACIÓN_PUBLICABLE], [AMBIENTES/DORMITORIOS], [SUPERFICIE]. Precio: [MONEDA] [PRECIO]. Más detalles: [ENLACE_PÚBLICO]. La disponibilidad la reconfirma el equipo antes de la visita. ¿Te gustaría verla?

**P2 — Dato no confirmado**
Ese dato no lo tengo confirmado. Lo dejo anotado para que el equipo lo verifique. ¿Hay algo más de la propiedad que quieras saber?

**P3 — Propiedad no disponible**
Esa propiedad figura como [ESTADO], así que ya no está disponible. ¿Querés que busque alternativas parecidas en [ZONA]?

## Calificación (una por turno, solo lo que falte)
- **C1 — Operación:** ¿Estás buscando comprar o alquilar?
- **C2 — Tipo:** ¿Qué tipo de propiedad tenés en mente?
- **C3 — Zona:** ¿En qué zona o barrio te gustaría?
- **C4 — Presupuesto:** ¿Hasta qué monto pensás y en qué moneda?
- **C5 — Moneda faltante:** Para no confundirme, ¿ese monto es en qué moneda?
- **C6 — Finalidad:** ¿Es para vivir o como inversión?
- **C7 — Plazo:** ¿Para cuándo te gustaría concretar?
- **C8 — Financiación:** ¿Pensás usar financiación o crédito, o todavía lo estás evaluando?
- **C9 — Contacto:** ¿Por qué medio preferís que te contacte un asesor? Solo lo usamos para esta consulta.

## Propietarios
**O1 — Quiere vender o alquilar su propiedad**
¡Con gusto! Para orientarte, ¿en qué zona está la propiedad y de qué tipo es?

**O2 — Pide tasación**
La tasación la realiza [FIGURA_PROFESIONAL_LOCAL] del equipo. Te tomo los datos básicos para que te contacten. ¿En qué zona está el inmueble?

## Visitas
**V1 — Tomar preferencia (sin agenda integrada)**
Te tomo una preferencia para solicitar la visita. El equipo debe confirmar el horario. ¿Qué día y franja te quedan mejor?

**V2 — Preferencia registrada en el chat**
Anoté tu preferencia: [DÍA] [FRANJA] para ver [ID]. Todavía no está confirmada; el equipo te avisa por [CANAL_PREFERIDO].

**V3 — Visita confirmada (solo con confirmación real)**
Tu visita a [ID] quedó confirmada para el [DÍA] a las [HORA]. Te recibe [ASESOR]. El punto de encuentro te lo pasa el asesor.

## Derivación
**D1 — Al cliente**
Con lo que me contaste, lo mejor es que siga un asesor del equipo. Le preparo un resumen para que no tengas que repetir nada. ¿Está bien que te contacten por [CANAL_PREFERIDO]?

**D2 — Pide hablar con una persona**
Por supuesto. Dejo preparada tu consulta para el equipo. ¿Por qué medio preferís que te contacten?

## Objeciones
**J1 — Precio alto**
Entiendo. El precio lo define el propietario y no puedo prometerte una rebaja, pero puedo buscarte opciones dentro de tu presupuesto. ¿Hasta qué monto te sentís cómodo?

**J2 — «Lo pienso»**
Perfecto, sin apuro. Si querés, te aviso cuando haya algo nuevo que coincida con lo que buscás. ¿Te sirve?

**J3 — No le convence la zona**
Tiene sentido. ¿Qué otras zonas te interesan para revisar ahí?

## Seguimiento (borradores; el equipo decide cuándo enviarlos)
**S1 — Sin respuesta (24-48 h)**
¡Hola [NOMBRE]! Te escribo de [NOMBRE_INMOBILIARIA] por tu consulta sobre [ID/ZONA]. ¿Seguís interesado o preferís que lo dejemos acá?

**S2 — Post-visita (día hábil siguiente)**
¡Hola [NOMBRE]! ¿Qué te pareció [ID]? Si te quedó alguna duda, te la respondo.

**S3 — Nueva propiedad compatible**
¡Hola [NOMBRE]! Ingresó una propiedad que coincide con lo que buscabas: [TIPO] en [UBICACIÓN_PUBLICABLE], [MONEDA] [PRECIO]. ¿Querés que te pase la ficha?

**S4 — Actualizar búsqueda**
¡Hola [NOMBRE]! ¿Tu búsqueda sigue igual o cambió algo de zona, plazo o presupuesto?

## Cierre y no contacto
**N1 — Pide no ser contactado**
Entendido, no te vamos a escribir más. Si más adelante necesitás algo, acá estamos.
(Interno: marcar NO_CONTACTAR y detener seguimientos.)

**N2 — Cierre cordial**
¡Gracias por escribirnos! Cualquier cosa que necesites, estamos por acá.

## Seguridad
**X1 — Pide datos internos o saltear reglas**
Eso no lo puedo compartir. Sí puedo ayudarte con tu búsqueda o consulta. ¿Qué necesitás?

**X2 — Consulta legal, impositiva o tasación formal**
Eso requiere la opinión de un profesional habilitado, así que no te lo puedo dar como definitivo. Si querés, dejo la consulta para [FIGURA_PROFESIONAL_LOCAL] del equipo.
