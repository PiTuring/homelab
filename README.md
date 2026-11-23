# 🏠 Homelab

> Le journal de bord de mon homelab d'étudiant : je monte une infra from scratch pour apprendre, casser, réparer, et documenter tout ça en public.

🌐 **Site :** https://<ton-user>.github.io/homelab/

> [!WARNING]
> 🚧 **Projet en cours de construction.** Le homelab, la documentation et ce repo évoluent en permanence : des pages sont vides ou incomplètes, certaines informations peuvent être obsolètes, et la structure peut changer sans préavis. Reviens régulièrement ou suis les [issues](../../issues) pour voir l'avancement.

## 🎯 Pourquoi ce projet ?

Je suis étudiant et je construis mon homelab pour apprendre en pratiquant, pas seulement en lisant des cours. Ce repo sert à deux choses :

- **Documenter** : ce que j'installe, comment, et surtout pourquoi j'ai fait tel choix.
- **Raconter** : les erreurs, les impasses et les déclics. Une partie du contenu est écrite comme un blog, avec les galères incluses.

## 📚 Ce que j'y apprends

| Domaine | Exemples de sujets |
|---|---|
| **Infrastructure** | Virtualisation, conteneurs, stockage, réseau (VLANs, DNS, DHCP), sauvegardes |
| **Services** | Auto-hébergement d'applications, reverse proxy, supervision, gestion de logs |
| **Sécurité** | Durcissement des systèmes, gestion des accès, segmentation réseau, gestion des secrets, mises à jour |

## 🧱 Contenu du site

```
docs/
├── index.md            # Vue d'ensemble et schéma global
├── blog/               # Articles et retours d'expérience
├── infrastructure/     # Matériel, réseau, stockage
├── services/           # Une page par service
├── operations/         # Sauvegardes, mises à jour, procédures de restauration
├── decisions/          # Pourquoi tel choix technique (ADR)
└── changelog.md        # Évolutions de l'infra, datées
```

## 🛠️ Stack de la documentation

- [MkDocs](https://www.mkdocs.org/) avec le thème [Material](https://squidfunnel.github.io/mkdocs-material/)
- Diagrammes en [Mermaid](https://mermaid.js.org/), versionnés avec le texte
- Déploiement automatique sur GitHub Pages via GitHub Actions

## 🚀 Lancer la doc en local

```bash
git clone git@github.com:<ton-user>/homelab.git
cd homelab
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
mkdocs serve
```

Le site est ensuite disponible sur http://127.0.0.1:8000.

## 🔒 Règles de publication

Le repo est public, donc :

- Aucun mot de passe, token, clé ou certificat, même ancien ou révoqué.
- Aucune IP publique ni domaine réellement exposé : j'utilise des valeurs fictives ou des placeholders.
- Un détecteur de secrets tourne avant chaque commit.

Si tu repères une information sensible dans ce repo, ouvre une issue ou contacte-moi directement.

## 🗺️ Roadmap

*État actuel : démarrage du projet, mise en place du repo et du site.*

- [x] Création du repo et choix de la stack de documentation
- [ ] Documenter le matériel
- [ ] Documenter le réseau et le plan d'adressage
- [ ] Mettre en place et documenter l'hyperviseur
- [ ] Premier service complet, utilisé comme modèle de page
- [ ] Sauvegardes et test de restauration
- [ ] Supervision et alerting
- [ ] Durcissement et revue de sécurité

L'avancement détaillé est suivi dans les [issues](../../issues).

## 🤝 Contributions

Ce projet reste avant tout personnel, mais les remarques sont les bienvenues : une erreur, une meilleure pratique, une alternative à tester. Ouvre une issue ou une pull request.

## 📄 Licence

Distribué sous licence [MIT](LICENSE).
