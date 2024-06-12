---
marp: true
---

# Configuration

## `setup.py`

### Avantages
- **Historique** : Longue utilisation, largement adopté.
- **Flexible** : Permet des configurations dynamiques via Python.

### Faiblesses
- **Complexité** : Peut devenir complexe pour les grands projets. (Difficile à lire)
- **Non-Standardisé** : Pas de structure standardisée (mais possible d'en définir une)

---

## `pyproject.toml`

### Avantages
- **Standardisé** : PEP 518 offre une structure standard
- **Clair** : TOML, syntaxe plus lisible
- **Compatible** : Supporte divers outils modernes comme `poetry`, `hatch`.

### Faiblesses
- **Nouvelle Adoption** : Techno plus récente, moins éprouvée et documentée
- **Limitations** : Statique donc impossible d'utiliser Python dans le fichier. 

---

## OpenAlea

### Choix : `pyproject.toml`

- **Standardisation** : Facilite l'interopérabilité entre les outils.
- **Lisibilité** : Configuration plus claire et plus facile à maintenir.
- **Compatibilité Future** : Supporte les outils modernes et les futures évolutions du packaging Python.
- **Usage** : On peut utiliser pyproject.toml en plus de setup.py
