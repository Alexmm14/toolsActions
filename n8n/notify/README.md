# 📪 Notify n8n Action

Envîa cualquier objeto JSON a n(n mediante Webhook.

## ⛤ Inputs

| Nombre | Descripción | Requerido |
| :--- | :--- | :--- |
| `endpoint` | URL del webhook de n8n. | Sí |
| `json_body` | Cuerpo del mensaje JSON. | Sí |

## 💔 Ejemplo dinámico

```yaml
- name: Notificar
  uses: Alexmm14/toolsActions/notify-n8n@master
  with:
    endpoint: ${{ secrets.N8N_URL }}
    json_body: |
      {
        "project": "${{ steps.vars.outputs.project_name }}",
        "status": "OK"
      }
```