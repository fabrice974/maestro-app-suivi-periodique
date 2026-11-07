# maestro-app-suivi-periodique

Application **Suivi périodique** (simulée) de la PoC Maestro : collecte mensuelle de l'information
financière, plans d'action, et signalement au backbone des faits métier qui terminent le suivi
(`remboursement-complet`, `decision-desinvestir`).

Elle ne connaît ni Camunda ni le BPMN : elle parle uniquement à la passerelle du backbone
([maestro-v2](https://github.com/fabrice974/maestro-v2)) via le SDK
[`@maestro/sdk`](https://github.com/fabrice974/maestro-sdk-ts).

## Lancer

```bash
npm install
cp .env.example .env     # facultatif
npm start                # http://localhost:4104
```

Prérequis : la passerelle de maestro-v2, ou `npm run ecosysteme -- demarrer` depuis maestro-v2.
