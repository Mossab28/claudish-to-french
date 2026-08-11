---
name: writing-french-prose
description: >-
  Retire les tics d'écriture IA du français. À utiliser pour rédiger, corriger,
  relire ou réécrire du texte en français (essais, posts, docs, e-mails, README).
  Remplace le glossaire IA et les anglicismes creux par un français fluide,
  concret, avec sujets réels, verbes forts et rythme varié.
---

# Écrire en prose française

Écrire un français qui sonne comme un bon rédacteur humain, pas comme un modèle. Deux échecs comptent comme du « slop ». Le premier est le vernis IA classique : formules d'ouverture, contrastes binaires, intensifs vides, vocabulaire signature, phrases affiche. Le second est la surcorrection : prose compressée en slogans de six mots jusqu'à ressembler à un post LinkedIn. La cible est entre les deux : français courant et précis (bon blog d'ingénierie, article de presse soigné, note claire), avec sujets concrets, vrais verbes, et un rythme qui varie parce que les idées l'exigent.

Adaptation française du skill anglais [writing-english-prose](https://github.com/qiaeru/skill-english-prose) (fork de [stop-slop](https://github.com/hardikpandya/stop-slop) par Hardik Pandya / qiaeru).

## Quand appliquer

Appliquer aux essais, posts, documentation, README, e-mails, annonces, et toute prose professionnelle en français. Ignorer fiction, poésie, textes juridiques et citations directes, où ces règles aplatiraient une voix volontaire. Registre cible : français magazine clair, conversationnel mais précis. Les contractions orales (« c'est », « on ») sont normales à l'écrit informel ; les garder quand le registre le permet.

## Processus

Pour une réécriture complète :

1. Lire tout le texte avant de corriger ; rythme, répétitions et cadence ne se voient que sur plusieurs paragraphes.
2. Appliquer les règles centrales ; ouvrir les références au besoin.
3. Passer les contrôles rapides.
4. Noter sur les cinq axes ; réécrire sous 35/50.
5. Relire sa propre sortie avec les mêmes contrôles. Le texte corrigé doit passer les règles qu'il impose.

Pour un texte court (e-mail, message, un paragraphe), appliquer les règles sans la grille de score.

## Cas particulier : chaînes d'interface

Un fichier d'UI mélange deux registres ; traiter par unité, pas par fichier.

**Micro-libellés** : boutons, onglets, menus, labels, titres courts, notifications d'une ligne. Ce sont des fragments, pas des phrases : les règles de rythme et de contraste ne s'appliquent pas. Vérifier seulement vocabulaire et conventions. Capitalisation cohérente dans tout le produit (souvent majuscule initiale seule sur le web).

**La règle 15 s'inverse sur les micro-libellés.** En prose on varie le lexique ; dans une interface, la même action garde le même mot partout. Si un bouton dit « Supprimer », ne pas alterner avec « Effacer » ou « Retirer » ailleurs.

**Chaînes longues** : descriptions, aide, corps de confirmation, erreurs explicatives. Dès qu'il y a une vraie phrase, appliquer tout le skill.

## Règles centrales

1. **Des phrases qui coulent.** La plupart portent une idée en environ 12 à 25 mots et se relient aux voisines. Une phrase courte sert l'emphase une fois par passage, pas en défaut. Les fragments empilés (« Zéro friction. Zéro jargon. Juste le résultat. ») sont aussi un tic que le bloat. Voir [references/structures.md](references/structures.md).

2. **Couper les formules vides.** Ouvertures qui s'éclaircissent la gorge, béquilles d'emphase, accroches marketing, formules d'e-mail, artefacts de chat. Voir [references/phrases.md](references/phrases.md).

3. **Des mots simples.** Préférer le mot court et courant au latinisme ou à l'anglicisme creux : « utiliser » plutôt que « mobiliser » / « leverage », « commencer » plutôt que « s'engager dans », « examiner » plutôt que « plonger au cœur de ». La liste IA (« seamless », « robuste » en automatique, « paysage », « débloquer le potentiel ») est dans [references/phrases.md](references/phrases.md).

4. **Casser les structures formulaires.** Contrastes binaires, listes négatives, balanciers, questions rhétoriques immédiatement répondues, queues en participe présent, cadences ternaires. Voir [references/structures.md](references/structures.md).

5. **Préférer la voix active.** Trouver l'acteur et le mettre devant. Le passif reste légitime quand l'acteur est inconnu ou secondaire (« il a été arrêté en mai ») ; le tic est le passif pour éviter de nommer qui a fait quoi.

6. **Pas de fausse agency.** Les plaintes ne deviennent pas des correctifs, les décisions n'émergent pas, les données ne parlent pas. Nommer la personne ; sinon « vous » / « on ».

7. **Être précis.** Pas de déclaratifs vagues (« les implications sont majeures »). Nommer l'implication, avec un chiffre ou un objet concret quand il existe.

8. **Mettre le lecteur dans la pièce.** « Vous » / « on » bat « les gens », une scène bat une généralité, la voix du conférencier à distance (« Cela s'explique par... ») part.

9. **Couper intensifs vides et hedges empilés.** « Vraiment », « profondément », « fondamentalement », « incroyablement » n'ajoutent rien. Garder les adverbes qui changent le sens (« lentement », « deux fois », « rarement »). Un hedge volontaire est de l'honnêteté ; trois réflexes sont le tic. Le menu des deux côtés (« d'un côté... de l'autre », « cela dépend ») pour éviter une position est la même esquive : prendre une position, puis nommer le vrai trade-off.

10. **Tuer le méta-commentaire.** Pas de panneau indicateur (« Dans cet article, nous allons... »), pas d'auto-narration (« Entrons dans le vif »), pas d'autorisation (« Et c'est OK »). Entrer dans le point directement.

11. **Pas de béquilles typographiques.** Pas de tiret cadratin ni demi-cadratin ; virgule, point ou parenthèses. Pas de gras pour l'emphase en pleine prose, pas de libellés gras (« **Vitesse :** ... ») qui déguisent une liste en prose, pas d'emoji en prose. Point-virgule seulement pour équilibrer deux propositions liées ; deux-points seulement pour introduire quelque chose de réel.

12. **Ne pas répondre à ses propres questions rhétoriques.** « Le résultat ? Des builds plus rapides. » est une transition déguisée. Dire : « Les builds sont devenus plus rapides. »

13. **Faire confiance au lecteur.** Affirmer directement ; couper « il est important de noter », « inutile de le dire », et toute phrase qui annonce ce que le lecteur va comprendre.

14. **Couper les phrases affiche.** Si ça sonne comme une citation LinkedIn ou un titre de slide, en faire une phrase de travail.

15. **Varier ce qui se répète.** Longueurs de phrases, fins de paragraphes, nombres d'éléments dans les listes, ouvertures. Trois longueurs identiques d'affilée, ou chaque paragraphe qui finit en punchline, sonne machine.

16. **Suivre les conventions françaises.** Espaces fines avant `?` `!` `:` `;` (ou espace normale selon la maison d'édition, mais cohérent). Guillemets français « ... » en prose soignée ; guillemets droits acceptables en docs techniques si le projet les utilise déjà. Pas de Title Case à l'américaine sur des noms communs (« notre équipe marketing », pas « notre Équipe Marketing »). Orthographe française correcte ; ne pas importer l'orthographe US.

17. **Préférer les verbes aux nominalisations, et raccourcir les connecteurs.** « Décider » plutôt que « prendre une décision », « analyser » plutôt que « procéder à une analyse ». « Pour » plutôt que « afin de pouvoir », « parce que » plutôt que « du fait que », « peut » plutôt que « est en mesure de ». Réécrire les ouvertures « Il y a / Il existe » autour d'un vrai sujet. Voir [references/phrases.md](references/phrases.md).

18. **Ne pas sur-bullet.** Réserver les listes aux items vraiment parallèles (étapes, paramètres, inventaire). Deux ou trois idées liées par un raisonnement vont dans un paragraphe relié.

19. **Traiter les anglicismes.** Un emprunt technique stable (« commit », « cache », « build ») peut rester en contexte eng/docs. L'anglicisme marketing creux (« leverage », « mindset », « seamless », « game-changer », « deep dive ») se remplace par le français concret, ou par le fait mesurable.

## Peser les tics

La plupart des tics portent sur la densité, pas l'occurrence isolée. Un seul « robuste », un « naviguer », un hedge : les humains écrivent ainsi ; le même mot quatre fois dans un paragraphe est le signal. Les mots forts (« plonger au cœur », « tapestry » / « riche tapisserie », « seamless », « débloquer le potentiel ») partent à vue. Exception en une seule occurrence : tiret cadratin / demi-cadratin, et reste d'assistant (« En tant qu'IA... »).

## Contrôles rapides

### Flux et rythme

- Trois fragments courts d'affilée, ou chaque phrase sous dix mots ? Reconstruire.
- Phrase tordue pour éviter un tiret, ou « lol » / faute volontaire collés ? Surcorrection ; écrire la phrase plainte.
- Trois phrases de même longueur ? En casser une.
- Cadence ternaire partout (« clair, concis et convaincant ») ? Varier ; souvent deux ou un suffit.
- Même mot ou même ouverture à courte distance ? Varier.

### Lexique

- Intensif vide (« très », « vraiment », « profondément », « extrêmement ») ? Couper. Adverbe utile ? Garder.
- Nominalisation (« prendre une décision », « procéder à une analyse ») ? Verbe.
- « Afin de », « du fait que », « préalablement à », « est en mesure de » ? « Pour », « parce que », « avant », « peut ».
- Hedges empilés ? Au plus un.
- Menu des deux côtés pour éviter une position ? Prendre position, puis le trade-off.
- Vocabulaire IA / anglicismes creux ? Remplacer.
- « De plus, » « En outre, » « Par ailleurs, » en ouverture de chaque phrase ? Au plus un connecteur par paragraphe.

### Acteurs et voix

- « Il y a / Il existe » en ouverture ? Réécrire autour d'un sujet réel.
- « Il est essentiel / important de... » sans acteur ? Nommer qui doit agir.
- Passif qui cache un acteur connu ? Le nommer.
- Chose inanimée avec verbe humain (« la décision émerge ») ? Nommer la personne.

### Structures formulaires

- « Pas X. Mais Y. » / « ce n'est pas seulement X ; c'est Y » ? Dire Y.
- « Moins de X, plus de Y » / « Pensez X, pas Y » ? Phrase complète.
- Liste négative (« Ce n'est pas A. Ce n'est pas B. C'est C. ») ? Dire C.
- Question rhétorique aussitôt répondue (« Le hic ? ... ») ? Affirmer.
- Pseudo-cleft (« Ce qui rend cela difficile, c'est... ») ? Nommer la contrainte.
- Queue en participe (« , permettant de... », « , garantissant... ») ? Finir la phrase ; donner à la conséquence sa propre phrase et son acteur, ou couper.

### Ouvertures, fins, boilerplate

- Ouverture qui s'éclaircit la gorge (« Voici la chose », « Soyons honnêtes ») ? Aller au point.
- Accroche marketing (« Dans un monde où », « Que vous soyez X ou Y ») ? Couper ou nommer le vrai public.
- Fin cliché (« En conclusion », « Au final », « X est là pour durer ») ? Finir sur du concret.
- Formules d'e-mail (« J'espère que ce message vous trouve en bonne santé », « N'hésitez pas à ») ? Ouvrir sur la raison ; fermer sur l'étape suivante.
- Artefacts d'assistant (« En tant qu'IA », « Excellente question », « Souhaitez-vous que je... ») ? Tout supprimer.

### Substance

- Déclaratif vague ? Nommer l'implication précise.
- Paragraphe qui reformule le prompt sans rien perdre à la suppression ? Affirmer ou supprimer.
- Phrase affiche ? Phrase de travail.

### Typographie et conventions

- Tiret cadratin / demi-cadratin ? Virgule, point ou parenthèses.
- Gras ou emoji en prose ? Retirer ; réécrire si le mot doit peser.
- Libellé gras, séparateur `---`, emoji comme puce ? Paragraphes et marqueurs simples.
- Point-virgule là où un point coule mieux ? Remplacer.
- Deux-points purement annonceurs (« Voici l'insight clé : ») ? Couper l'annonce.
- Liste à puces qui porte un argument ? Paragraphe relié.
- Titre listicle (« 7 façons de », « 5 signes que ») ou squelette intro / trois corps / « en résumé » ? Laisser la forme suivre l'argument.
- Title Case US ou calque d'orthographe anglaise ? Corriger au français.

## Scoring

Noter de 1 à 10 sur chaque axe.

| Axe | Question |
| --- | --- |
| Flux | Les phrases se relient et respirent, ou s'empilent en fragments / en bloat ? |
| Directness | Des affirmations, ou des annonces et des mises en scène ? |
| Concret | Acteurs nommés, chiffres, objets précis ? |
| Authenticité | Ça sonne comme quelqu'un qui écrit bien, pas un modèle ou une marque ? |
| Économie | Quelque chose de coupable sans casser le rythme ? |

Sous 35/50 : réviser.

## Exemples

Voir [references/examples.md](references/examples.md) pour des avant/après.

## Licence et attribution

MIT dans l'esprit du skill source. Structure et méthode adaptées de [qiaeru/skill-english-prose](https://github.com/qiaeru/skill-english-prose) / [hardikpandya/stop-slop](https://github.com/hardikpandya/stop-slop).
