# ECHO — n8n Automation Workflows

**EN:** A collection of automation workflows built with n8n. Each workflow solves a specific business problem and is documented in English and German.

**DE:** Eine Sammlung von Automatisierungs-Workflows, erstellt mit n8n. Jeder Workflow löst ein konkretes Geschäftsproblem und ist auf Englisch und Deutsch dokumentiert.

---

## 01 — Webhook Receiver

**EN:** Receives POST requests with a name and message, processes them in a Code node, and returns a personalized greeting in German.

**DE:** Empfängt POST-Anfragen mit Name und Nachricht, verarbeitet sie in einem Code-Knoten und gibt eine personalisierte Begrüßung auf Deutsch zurück.

**Stack:** n8n · JavaScript · REST API  
**Status:** ✅ Published and live

### Workflow Structure

![n8n workflow canvas](./screenshots/workflow-canvas.png)

Webhook → Code (JavaScript) → Respond to Webhook

### Try It Live

**Production URL:** `https://franklin-ajuorah.app.n8n.cloud/webhook/echo-receiver`  
**Method:** `POST`  
**Content-Type:** `application/json`

**Example request body:**
```json
{
  "name": "Franklin",
  "message": "Grüße aus Nigeria"
}
### Import This Workflow

1. Download the workflow: https://github.com/Franklin-Ajuorah/echo-workflows/raw/main/01-webhook-receiver.json
2. In n8n, click **Import from File**
3. Select the downloaded JSON
4. Update the webhook path if desired
5. Activate the workflow
