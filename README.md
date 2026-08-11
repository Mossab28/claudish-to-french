# Claudish / Français

Skill Cursor / Claude Code: **deux registres** pour tout le travail de l'agent, pas seulement la doc.

![Claudish vs Français](assets/claudish-vs-francais.png)

| Claudish | Français |
| --- | --- |
| Densité agent: chemins, env, quirks, littéraux | Clarté humaine: intention, effet, prochain pas |
| Quand on **agit** ou on laisse une trace pour un agent | Quand on **parle** à l'humain |

## Ce que ça change

- **Chaque fois que l'agent parle** → Français clair
- **Chaque fois qu'on lui demande de faire un truc** → exécution Claudish (preuves), compte-rendu Français
- Doc mixte → les deux colonnes sur la même vérité

## Contenu

```text
skill-claudish-fr/
├── LICENSE
├── README.md
├── assets/claudish-vs-francais.png
├── rules/claudish-francais.mdc    # alwaysApply pour Cursor
└── skills/claudish-francais/
    ├── SKILL.md
    └── references/examples.md
```

## Installation

### Cursor (recommandé: skill + règle always-on)

```bash
git clone https://github.com/Mossab28/skill-claudish-fr.git
cp -R skill-claudish-fr/skills/claudish-francais ~/.cursor/skills/
cp skill-claudish-fr/rules/claudish-francais.mdc ~/.cursor/rules/
```

La règle `alwaysApply: true` force le comportement à chaque tour. Le skill donne le détail et les exemples.

### Claude Code

```bash
cp -R skills/claudish-francais ~/.claude/skills/
```

Pour un effet « toujours on » côté Claude Code, ajoute aussi un rappel court dans ton `CLAUDE.md` / `AGENTS.md` personnel qui pointe vers ce skill.

## Inspiration

Le format visuel Claudish vs English (doc agent dense vs doc humaine) vu dans les posts type Reddit / comparaisons de `AGENTS.md`. Ici: étendu au **parler** et au **faire**, avec la colonne humaine en français.

## Licence

MIT
