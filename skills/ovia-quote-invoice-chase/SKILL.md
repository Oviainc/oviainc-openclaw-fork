---
name: ovia-quote-invoice-chase
description: "Follow up quotes and invoices on a steady rhythm — heads-up, polite, firm, final — with promise-to-pay handling and part-payment awareness, in English, French, and Spanish. Use when: a quote awaits an answer, an invoice is due or overdue, a client promised a payment date, or a balance remains after a part-payment. NOT for: disputes about the work itself (escalate to a human) or appointment matters (use ovia-scheduling-followup)."
metadata: { "openclaw": { "emoji": "🧾" } }
---

# Ovia quote and invoice chase

Getting paid is a rhythm, not an argument: start before the due date, stay courteous, escalate on schedule, and let the records drive every step.

## When to use

✅ **USE this skill when:**

- A quote has been sent and awaits the client's answer
- An invoice is approaching its due date, due today, or overdue
- A client gave a promise-to-pay date that needs tracking
- A part-payment landed and a balance remains

## When NOT to use

❌ **DON'T use this skill when:**

- The client disputes the work, the scope, or the amount itself → escalate to a human with the records attached
- The client asks for a discount, a refund, or new payment terms → escalate to a human
- The open item is an appointment, not a document → `ovia-scheduling-followup`

## The rhythm (invoices)

| Step | Timing | Tone |
| --- | --- | --- |
| Heads-up | 3 days before the due date | Friendly notice, payment details attached |
| Due today | On the due date | Short, factual |
| Polite | 1–7 days overdue | Assume an oversight; restate amount and details |
| Firm | 8–21 days overdue | Name the delay plainly; ask for a payment date |
| Final | 22+ days overdue | Last step in the sequence; propose agreeing a plan, or pausing further work, per the engagement's policy |

Quotes follow a shorter arc: a check-in 3 days after sending, a second at 7 days offering to adjust scope, and a closing note at 14 days that keeps the door open.

## Promise-to-pay handling

- When a client commits to a date, **record the promise** (date promised, amount, channel) on the invoice.
- **Pause the rhythm** while the promise is ahead — no reminders between the promise and its date.
- **Promise kept**: close the invoice, thank the client in one line, log the outcome.
- **Promise missed**: resume the next day at the firm step, referencing the promise factually and without reproach, and flag the client record.

## Part-payments

- Chase **only the remaining balance**, never the original total.
- The printed and sent document shows the amount paid and the balance due, so the client sees the same numbers we see.
- A payment that covers the balance closes the invoice automatically in the records.

## Rules for every message

- **Amounts, invoice numbers, and dates come from the records** — never from memory or from the client's wording.
- **Payment details ride along** on every reminder, in the document's language, so paying takes one step.
- **Client's language**: English, French, or Spanish, matching the document.
- **Log every send**: date, step, and channel go onto the invoice's chase history; the history decides the next step.
- **Never threaten.** The final step proposes a plan or a pause, in the engagement's own policy wording — nothing beyond it.

## Templates

**Heads-up — EN:** "Hello [Name], a friendly note that invoice [number] for [amount] falls due on [date]. Payment details are below for convenience. Thank you."
**FR:** « Bonjour [Nom], petit rappel amical : la facture [numéro] de [montant] arrive à échéance le [date]. Les coordonnées de paiement sont ci-dessous pour vous faciliter la tâche. Merci. »
**ES:** "Hola [Nombre], una nota amable: la factura [número] por [importe] vence el [fecha]. Los datos de pago están abajo para su comodidad. Gracias."

**Polite — EN:** "Hello [Name], invoice [number] for [amount] was due on [date] and shows as open in our records. If payment is already on its way, thank you — otherwise the details below make it quick."
**FR:** « Bonjour [Nom], la facture [numéro] de [montant] est arrivée à échéance le [date] et reste ouverte dans nos dossiers. Si le paiement est déjà en route, merci — sinon, les coordonnées ci-dessous rendent la démarche rapide. »
**ES:** "Hola [Nombre], la factura [número] por [importe] venció el [fecha] y sigue abierta en nuestros registros. Si el pago ya viene en camino, gracias; en caso contrario, los datos siguientes lo hacen rápido."

**Firm — EN:** "Hello [Name], invoice [number] for [amount] is now [days] days past its [date] due date. Please arrange payment this week, or tell us the date payment will be made so the record can be updated."
**FR:** « Bonjour [Nom], la facture [numéro] de [montant] a maintenant [jours] jours de retard sur son échéance du [date]. Merci de procéder au paiement cette semaine, ou de nous indiquer la date à laquelle il sera fait afin que nous mettions le dossier à jour. »
**ES:** "Hola [Nombre], la factura [número] por [importe] lleva [días] días de retraso sobre su vencimiento del [fecha]. Por favor realice el pago esta semana, o indíquenos la fecha en que se hará para actualizar el registro."

**Final — EN:** "Hello [Name], invoice [number] for [amount], due [date], remains open after several reminders. Please contact us this week so a payment plan can be agreed; until then, further work on the account is paused."
**FR:** « Bonjour [Nom], la facture [numéro] de [montant], échue le [date], reste ouverte après plusieurs rappels. Merci de nous contacter cette semaine afin de convenir d'un plan de paiement ; d'ici là, la suite des travaux sur le compte est en pause. »
**ES:** "Hola [Nombre], la factura [número] por [importe], vencida el [fecha], sigue abierta tras varios recordatorios. Por favor contáctenos esta semana para acordar un plan de pago; hasta entonces, el trabajo adicional en la cuenta queda en pausa."

**Promise missed — EN:** "Hello [Name], the payment of [amount] for invoice [number] was expected on [promised date] and has not arrived yet. Please arrange it today, or tell us the new date so the record stays accurate."
**FR:** « Bonjour [Nom], le paiement de [montant] pour la facture [numéro] était attendu le [date promise] et n'est pas encore arrivé. Merci de le faire aujourd'hui, ou de nous indiquer la nouvelle date afin que le dossier reste exact. »
**ES:** "Hola [Nombre], el pago de [importe] por la factura [número] se esperaba el [fecha prometida] y aún no ha llegado. Por favor realícelo hoy, o indíquenos la nueva fecha para mantener el registro exacto."
