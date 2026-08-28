# Hellfest Revente

Service de revente de billets Hellfest avec paiement par virement bancaire et
validation des justificatifs via Telegram.

## Organisation

- `artifacts/hellfest-revente/public/` contient le frontend Hellfest livré avec
  ses assets et les scripts de formulaire/paiement.
- `artifacts/api-server/` contient l’API Express et le traitement Telegram.
- `lib/db/` contient le schéma PostgreSQL Drizzle.

Le frontend fourni par la version précédente est un bundle statique. Le build
copie volontairement `public/` vers `dist/` afin de ne pas le remplacer par le
composant placeholder généré par l’outil de prototypage.

## Installation

Voir [MANUEL-INSTALLATION.md](./MANUEL-INSTALLATION.md) pour les variables
d’environnement et le déploiement Render.

Ne jamais versionner les secrets (`DATABASE_URL`, `SESSION_SECRET`,
`TELEGRAM_BOT_TOKEN`, `TELEGRAM_CHAT_ID` ou clés de stockage).
