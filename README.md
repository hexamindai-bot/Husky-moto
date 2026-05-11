# GNMF Championship Detail Page

ჩემპიონატის დეტალების გვერდი — Facebook Messenger ბოტისთვის.

## როგორ მუშაობს
Manychat Gallery → "დეტალები" ღილაკი → ეს გვერდი იხსნება `?id=recXXX` პარამეტრით → Airtable-დან ინფო გამოჩნდება.

## კონფიგურაცია (`detail.html`)
```javascript
const API_KEY = 'patXXXXX...';
const BASE_ID = 'appXXXXXX';
const TABLE   = 'championships';
```

## Deploy
```bash
vercel --prod
```

## Make.com ღილაკი
```json
{
  "type": "url",
  "caption": "დეტალები",
  "url": "https://your-site.vercel.app/detail.html?id={{2.ID}}"
}
```
