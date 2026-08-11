# Exemples Claudish / Français

## 1. Réponse chat (parler)

**Demande:** « Y a-t-il une vraie auth ? »

**Français (oui):**
> Pas encore. Un middleware te connecte automatiquement avec un utilisateur mock. Pour une vraie sécurité, il faudra un `protectedProcedure` et arrêter d'écrire le mot de passe en dur.

**Claudish collé dans le chat (non):**
> Auth - deliberate gap: `middleware/autoLogin.ts` on every request; `MOCK_USER_EMAIL` → cookie HttpOnly 7d; `user.create` writes literal `'hashed_password_here'`; all routes stay `publicProcedure` in `server/trpc.ts`.

## 2. Pendant une tâche (faire)

**Demande:** « Corrige le chemin du design system. »

**Travail Claudish (outils / notes):**
- Lu `components.json`: aliases pointent vers `/ui/`
- Design system réel: `/obra/`
- Aussi faux dans `CLAUDE.md` L12
- Fix: retarget aliases + sync doc agent

**Message final Français:**
> Les aliases pointaient vers `/ui/` alors que le design system est dans `/obra/`. J'ai corrigé `components.json` et la mention dans `CLAUDE.md`.

## 3. Même vérité, deux docs

**Claudish:**
> Running & deploying: five modes (`docker-compose.local.yaml`, `.dev.yaml`, `.prod.yaml`, `.ecs.yaml`, bare npm). Schema-relative `DATABASE_URL` resolved by `scripts/ensure-*.mjs`. Prod quirk: ALB targets 5173 (Vite) while Express listens 3001.

**Français:**
> Cinq façons de lancer (npm, Docker, Devcontainer, prod compose, ECS). Toutes partagent la même logique de chemin de base. En prod AWS, l'ALB parle au serveur Vite (5173), pas à Express (3001).

## 4. Compte-rendu après debug

**Français:**
> Les listes n'étaient pas paginées côté API, même si l'UI a des filtres. J'ai ajouté `limit`/`cursor` sur la query `items.list` dans `server/routers/items.ts`.

**À ne pas faire:** un pavé de stack trace sans conclusion, ou « j'ai amélioré la performance des listes » sans fichier.
