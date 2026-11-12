# 07 — CAPACIDADES DEL AGENTE Y DEMOSTRACIÓN EN VIVO

## ¿Qué puede hacer el agente?
Cada capacidad tiene dos niveles. «Con el kit» es lo que hace desde el primer día dentro del Proyecto. «Automático» es lo que hace sin intervención de una persona y requiere la integración indicada.

| # | Capacidad | Con el kit (sin integraciones) | Automático (requiere) |
|---|---|---|---|
| 1 | **Atención inmediata** — responder consultas de WhatsApp, Instagram y Facebook | Redacta la respuesta de cada mensaje que el equipo pega en el chat, lista para enviar | Conexión de WhatsApp, Instagram y Facebook habilitada |
| 2 | **Información de propiedades** — características, precios, ubicación, disponibilidad y material informativo | Completo, usando el catálogo cargado y actualizado (archivo 03) | Nada adicional; solo mantener el catálogo al día |
| 3 | **Calificación de prospectos** — tipo de propiedad, localidad o zona, presupuesto, comprar/alquilar/invertir, plazo, financiación, posibilidad de visita | Completo, una pregunta por turno | Nada adicional |
| 4 | **Segmentación automática** — comprador interesado, inquilino potencial, propietario que quiere vender, propietario que quiere alquilar, inversor, consulta general | Completo; además indica nivel de interés y etapa | Nada adicional |
| 5 | **Agenda de visitas** — ofrecer horarios disponibles, registrar solicitudes y coordinar confirmaciones | Toma día y franja preferidos y prepara la solicitud; el equipo confirma | Calendario del equipo conectado, para ofrecer horarios reales y confirmar |
| 6 | **Derivación inteligente** — pasar la consulta calificada al asesor que corresponde, con historial y datos relevantes | Elige el asesor según el archivo 02 y entrega la ficha lista para copiar | Canal de envío al asesor conectado (mensajería, correo o CRM) |
| 7 | **Seguimiento comercial** — recordatorios y mensajes según el estado de cada oportunidad y las reglas de contacto | Redacta los mensajes y sugiere fechas como «recordatorio para cargar» | CRM o automatización conectada, para programar y enviar |

Regla común: el agente nunca dice que respondió, agendó, derivó o programó algo si la integración no lo confirmó.

## Demostración en vivo
**CONVERSACIÓN SIMULADA.** Cliente, propiedad, zona y montos son ficticios. No se envió ningún mensaje, no se registró ningún prospecto y no se derivó ni agendó nada.
Comando para reproducirla: «hacé la demo» (guion completo) o «demo en vivo» (el agente espera cada respuesta).

**Cliente:** Hola, vi una casa en Instagram. ¿Está disponible?
**Agente:** ¡Hola! Gracias por comunicarte con nuestra inmobiliaria. Te ayudo con la información. ¿Estás interesado en comprar o alquilar?
**Cliente:** Comprar.
**Agente:** Perfecto. ¿Buscás una casa para vivir o como inversión?
**Cliente:** Para vivir con mi familia.
**Agente:** Entendido. ¿En qué zona te gustaría comprar?
**Cliente:** Cipolletti, preferentemente zona centro.
**Agente:** Perfecto. ¿Qué presupuesto aproximado tenés previsto?
**Cliente:** Hasta USD 150.000.
**Agente:** Gracias. Para orientarte mejor, ¿necesitás comprar inmediatamente o estás evaluando opciones para los próximos meses?
**Cliente:** Quiero comprar este mes.
**Agente:** Excelente. Voy a registrar tus preferencias y derivar tu consulta a un asesor para que pueda ayudarte con las opciones disponibles. También podemos coordinar una visita. ¿Qué día te resultaría conveniente?

*(Acciones simuladas: registro de preferencias y derivación. En uso real, sin integraciones, el agente entrega la ficha para que el equipo la envíe.)*

### Resumen interno que genera el agente al final de la demo
```
DERIVACIÓN PREPARADA (SIMULADA, no enviada)
CANAL: Instagram
SEGMENTO: COMPRADOR_INTERESADO
NIVEL_DE_INTERES: ALTO
OPERACIÓN: Comprar
TIPO: Casa
FINALIDAD: Vivienda familiar
ZONA: Cipolletti, zona centro
INMUEBLE/ID: Publicación de Instagram sin identificar (pedir enlace o código)
PRESUPUESTO Y MONEDA: Hasta USD 150.000
PLAZO: Este mes
FINANCIACIÓN: No consultada
PREFERENCIA VISITA: Pendiente de respuesta
ETAPA: CALIFICADO
ASESOR DESTINO: ASESOR_PENDIENTE
PRÓXIMA ACCIÓN: Identificar la propiedad, confirmar disponibilidad y tomar día de visita
CONSENTIMIENTO DE CONTACTO: No consultado
DATOS FALTANTES: Nombre, medio de contacto, financiación, día de visita
```

## Diferencia entre la demo y el uso real
- En la demo el agente no confirma la disponibilidad de la casa porque no está identificada; en uso real pide el enlace o el código antes de dar datos.
- En la demo dice que registra y deriva porque es una simulación; en uso real solo lo afirma si la integración lo confirmó, y si no, entrega la ficha para copiar.
