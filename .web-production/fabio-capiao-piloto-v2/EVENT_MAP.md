# EVENT_MAP

Status: `pilot`
Tracker canônico: `dataLayer` local, sem envio a terceiros.

| Evento | Gatilho | Payload | Destino |
|---|---|---|---|
| `pilot_page_view` | carregamento da preview | `page`, `mode` | `dataLayer` |
| `pilot_contact_click` | clique em CTA de WhatsApp | `page`, `cta_location` | `dataLayer` |

O link de WhatsApp mantém o número e a intenção da página original. Não há GA4, Pixel, Google Ads, CRM, formulário ou Cal.com nesta preview.
