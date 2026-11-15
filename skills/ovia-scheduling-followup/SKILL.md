---
name: ovia-scheduling-followup
description: "Run appointment confirmations, reminders, and no-show prevention sequences in English, French, and Spanish. Use when: an appointment is booked, a reminder is due, a client has not confirmed, or a no-show needs a follow-up and a rebooking offer. NOT for: general client questions (use ovia-client-conversations) or payment follow-up (use ovia-quote-invoice-chase)."
metadata: { "openclaw": { "emoji": "🗓️" } }
---

# Ovia scheduling follow-up

The reminder rhythm that keeps appointments kept: confirm early, remind twice, follow up the same day when someone does not show.

## When to use

✅ **USE this skill when:**

- An appointment has just been booked and needs confirmation
- A reminder step falls due (24 hours before, 2 hours before)
- A client has not replied to a confirmation request
- An appointment was missed and needs a follow-up with a rebooking offer

## When NOT to use

❌ **DON'T use this skill when:**

- The conversation is a general question or request → `ovia-client-conversations`
- Money is involved (deposits, balances, invoices) → `ovia-quote-invoice-chase` for invoices; escalate deposit disputes to a human

## The sequence

| Step | Timing | Purpose |
| --- | --- | --- |
| Confirmation | At booking | Fix the appointment in the client's mind; attach the calendar invite (.ics) |
| Reminder 1 | 24 hours before | Confirm attendance; offer one-tap rescheduling |
| Reminder 2 | 2 hours before | Short final reminder with place or joining details |
| No-show follow-up | Same day, within 2 hours after | Courteous check-in and a concrete rebooking offer |

## Rules

- **One message per step.** A reply from the client stops the sequence at once.
- **Client's language** throughout: English, French, or Spanish, matching the booking conversation.
- **Every message carries the essentials**: date, time, what the appointment is, and how to reschedule.
- **Rescheduling is always easy**: offer two concrete alternative times rather than an open question.
- **Record everything**: confirmation status and every reminder sent go into the client record, so the next conversation starts informed.
- **Repeated no-shows** (two or more for the same client): stop automatic rebooking offers and flag the client record for a human, who decides on deposits or booking conditions.

## Templates

**Confirmation — EN:** "Hello [Name], your appointment is confirmed for [date] at [time]: [service]. A calendar invite is attached. To reschedule, reply to this message."
**FR:** « Bonjour [Nom], votre rendez-vous est confirmé pour le [date] à [heure] : [service]. Une invitation calendrier est jointe. Pour déplacer le rendez-vous, répondez simplement à ce message. »
**ES:** "Hola [Nombre], su cita está confirmada para el [fecha] a las [hora]: [servicio]. Adjuntamos una invitación de calendario. Para cambiar la cita, responda a este mensaje."

**Reminder, 24 hours before — EN:** "Hello [Name], a reminder of your appointment tomorrow, [date] at [time]: [service]. Reply YES to confirm, or tell us if another time suits better."
**FR:** « Bonjour [Nom], petit rappel de votre rendez-vous demain, le [date] à [heure] : [service]. Répondez OUI pour confirmer, ou dites-nous si un autre moment convient mieux. »
**ES:** "Hola [Nombre], le recordamos su cita de mañana, [fecha] a las [hora]: [servicio]. Responda SÍ para confirmar, o díganos si otro horario le conviene más."

**Reminder, 2 hours before — EN:** "Hello [Name], we look forward to seeing you today at [time] for [service]. [Place or joining detail]. Safe travels."
**FR:** « Bonjour [Nom], au plaisir de vous voir aujourd'hui à [heure] pour [service]. [Lieu ou détail de connexion]. À tout à l'heure. »
**ES:** "Hola [Nombre], le esperamos hoy a las [hora] para [servicio]. [Lugar o detalle de conexión]. Hasta pronto."

**No-show follow-up — EN:** "Hello [Name], we missed you today at [time]. We hope everything is well. Two times are open to rebook: [option 1] or [option 2]. Reply with the one that suits, and the appointment is set."
**FR:** « Bonjour [Nom], nous vous avons manqué aujourd'hui à [heure]. Nous espérons que tout va bien. Deux moments sont libres pour reprendre rendez-vous : [option 1] ou [option 2]. Répondez avec celui qui vous convient, et le rendez-vous est fixé. »
**ES:** "Hola [Nombre], hoy le echamos de menos a las [hora]. Esperamos que todo esté bien. Hay dos horarios libres para reagendar: [opción 1] u [opción 2]. Responda con el que prefiera y la cita queda fijada."
