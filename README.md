# 🏆 Polla Mundialista 2026 — Ceiscol & RD

Mini app de la polla mundialista interna para clientes de **Ceiscol** y **RD**,
Copa Mundial de la FIFA 2026, desde cuartos de final hasta la gran final.

## Qué incluye

- Registro único (Ceiscol/RD, laboratorio, datos de contacto, departamento → ciudad en cascada).
- Calendario oficial FIFA convertido a hora de Colombia, con cierre automático de pronósticos
  30 minutos antes de cada partido.
- Sistema de puntos por marcador exacto / resultado correcto, con multiplicador por fase
  (cuartos y tercer puesto x1, semifinal x2, final x3).
- Clasificación pública 100% anónima (alias + avatar, sin datos personales).
- Panel de organizador para cargar resultados oficiales.
- Backend en Google Apps Script: cada inscripción se guarda en un Google Sheet y dispara
  correo de confirmación al participante y notificación a `ceiscol.concursos@gmail.com`.

## Publicar (GitHub Pages)

Settings → Pages → Source: **Deploy from a branch** → Branch: **main** / **/(root)** → Save.
El sitio queda disponible en `https://biocolombiaplus-max.github.io/polla-mundial-ceiscol-rd/`.

## Backend (Google Sheets + correo)

El endpoint de Apps Script se configura en la constante `SHEETS_ENDPOINT` dentro de
`index.html`. El código fuente del backend (`Code.gs`) se entregó aparte para desplegar
en el Google Sheet de registros.
