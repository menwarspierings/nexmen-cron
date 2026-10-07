# nexmen-cron

Roept elk half uur (werkdagen) `https://beheer.nexmen.nl/api/cron/mail` aan voor automatisch mailen.
Vercel Hobby draait cron maar één keer per dag, daarom via GitHub Actions.

Geheim: `MAIL_CRON_SECRET` (zelfde waarde als in Vercel, project nexmen-beheer).
Uitzetten: in beheer → Instellingen → Gmail en automatisch mailen, of deze workflow uitschakelen.
