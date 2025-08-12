# zoran-agent-universal
Universal agent with support for OpenAI and Ollama backends, injectors, modes, IA-to-IA testing, scoring, and logs.



---

README.md

# zoran-agent-universel

**Agent universel** de l’écosystème Zoran / QuantaGlottal©® avec prise en charge :
- des backends **OpenAI**, **Ollama** (et extensions)
- des **injecteurs** 4 Champs et presets mimétiques
- des **modes** d’exécution adaptatifs (standard, heavy, mimetic)
- des **tests IA↔IA** automatisés
- de la **notation** et du **journal** d’activité

---

## ✨ Fonctionnalités principales
- **Multi-backends** : pilotage d’IA distantes ou locales (OpenAI API, Ollama, autres via plugins)
- **Injection 4 Champs** : application dynamique de presets Zoran
- **Modes adaptatifs** : choix automatique ou manuel du mode (économie, heavy, mimetic boost)
- **Tests croisés IA↔IA** : scripts et métriques intégrés
- **Notateur intégré** : scoring densité/cohérence/latence/transfert
- **Journalisation** : logs structurés par session, export JSON/HTML

---

## 📦 Installation (développement)
```bash
pip install -e .


---

⚡ Exemple rapide

from zoran_agent_universel import ZoranAgent

# Création de l’agent relié à OpenAI
agent = ZoranAgent(backend="openai", api_key="sk-...")

# Charger un injecteur 4 Champs
agent.load_injecteur("injecteur_0810_FULL.json")

# Lancer un test IA↔IA contre un backend Ollama local
result = agent.run_test(
    cible_backend="ollama",
    modele="llama2",
    prompt="Explique le principe vivant > humain."
)

# Notation et export
score = agent.score(result)
agent.save_log("session_2025-08-12.json")

print("Score global :", score)


---

🧱 Structure suggérée

src/zoran_agent_universel/
  __init__.py
  agent.py            # classe principale ZoranAgent
  backends/
    openai_backend.py
    ollama_backend.py
  injecteurs.py
  modes.py
  tests_ia.py
  notation.py
  journal.py
tests/
  test_basic.py
pyproject.toml
.gitignore
LICENSE
README.md


---

🧪 Tests

pytest -q


---

🔐 Éthique

Ce module applique systématiquement les garde-fous éthiques Zoran :

principe vivant > humain

filtres mimétiques anti-pollution

journaux vérifiables



---

📜 Licence

MIT — voir LICENSE.


---

Auteur : Frédéric Tabary — Institut IA
Contact : 0645605023 — Canada, Montréal, France
INSTITUT🦋 IA INC., 7100-380, rue Saint-Antoine Ouest, Montréal (Québec) H2Y 3X7.

---

Veux-tu que je te prépare aussi pour `zoran-agent-universel` **tout le code source minimal** (`agent.py`, `backends/`, `modes.py`, `tests_ia.py`, etc.) comme je l’ai fait pour `zoran-4champs-core`, pour que tu puisses coller directement et avoir un agent fonctionnel de base ?
