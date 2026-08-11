# Skill French prose

`writing-french-prose` est une skill Cursor / Claude Code qui retire les tics d'écriture IA du français (le « slop ») : glossaire creux, anglicismes vides, structures formulées, sujets abstraits, rythme monotone.

Elle vise un français fluide et concret : sujets réels, verbes forts, rythme varié. Les règles vivent dans [SKILL.md](skills/writing-french-prose/SKILL.md) ; les catalogues sont dans `skills/writing-french-prose/references/`.

## Inspiration

Inspirée et adaptée de :

- [qiaeru/skill-english-prose](https://github.com/qiaeru/skill-english-prose)
- [hardikpandya/stop-slop](https://github.com/hardikpandya/stop-slop)

Même idée (anti-slop), transposée aux tics et au registre du français.

## Structure

```text
skill-french-prose/
├── LICENSE
├── README.md
└── skills/
    └── writing-french-prose/
        ├── SKILL.md
        └── references/
            ├── phrases.md
            ├── structures.md
            └── examples.md
```

## Installation

### Cursor

Copiez le dossier [skills/writing-french-prose/](skills/writing-french-prose/) vers `~/.cursor/skills/writing-french-prose/` :

```bash
cp -R skills/writing-french-prose ~/.cursor/skills/
```

Redémarrez Cursor (ou rechargez les skills) pour la détecter.

### Claude Code

Copiez le même dossier vers les skills globaux ou ceux d'un projet :

```bash
# global
cp -R skills/writing-french-prose ~/.claude/skills/

# ou dans un projet
cp -R skills/writing-french-prose /chemin/du/projet/.claude/skills/
```

Redémarrez Claude Code. Pour une mise à jour, re-copiez le dossier (le contenu n'est pas hot-reloadé).

## Usage

La skill se déclenche quand vous demandez de rédiger, corriger ou relire du texte en français. Vous pouvez aussi l'invoquer explicitement par son nom (`writing-french-prose`).

## Licence

MIT, voir [LICENSE](LICENSE).
