# nexmen-cron

Klok voor automatisch mailen: roept elke 20 minuten `https://beheer.nexmen.nl/api/cron/mail` aan (Vercel Hobby draait
cron maar één keer per dag). Eén lange run tikt ruim 5,5 uur en start zichzelf daarna opnieuw; elke 3 uur staat er een
geplande run als reserve. De logs tonen alleen de HTTP-statuscode.

Geheim: `MAIL_CRON_SECRET` (zelfde waarde als in Vercel, project nexmen-beheer).
Uitzetten: in beheer → Instellingen → Gmail en automatisch mailen (dan verstuurt het beheer niets), of deze workflow
uitschakelen in GitHub (Actions → Automatisch mailen → Disable workflow).
