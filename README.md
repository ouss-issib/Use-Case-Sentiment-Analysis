# 🤖 Activité Pratique : Prompt Engineering - Sentiment Analysis

Ce dépôt contient l'implémentation d'un cas d'utilisation concret du **Prompt Engineering** appliqué à l'**Analyse de Sentiment**. L'objectif est d'explorer différentes stratégies de prompting pour extraire et classifier les émotions à partir d'un dataset, en utilisant l'écosystème LangChain et OpenAI.

---

## 🎯 Objectifs Pédagogiques
- ✅ **Chargement & Analyse de Dataset** : Manipuler des données textuelles pour l'analyse.
- 🧩 **Stratégies de Prompting** : Comparer Zero-Shot, Few-Shot et Chain of Thought (CoT).
- 🧠 **Optimisation des Réponses** : Utiliser des "Gold Examples" pour améliorer la précision.
- 📊 **Évaluation** : Mesurer la performance des différents types de prompts.

---

## 🛠️ Technologies Utilisées
- **Python 3.11+**
- **LangChain** : Pour la gestion des Prompt Templates.
- **OpenAI API** : Modèles GPT pour l'inférence.
- **Pandas** : Pour l'analyse du dataset.
- **UV** : Gestionnaire de paquets ultra-rapide.

---

## 📚 Ressources
- 🎥 **Support Vidéo** : [Prompt Engineering Use Case - Mr. YOUSSFI](https://www.youtube.com/watch?v=wckvmfDESP8)
- 📝 **Guide Prompt Engineering** : [OpenAI Best Practices](https://platform.openai.com/docs/guides/prompt-engineering)

---

## 🧠 Concepts de Prompting Explorés

1. **Zero-Shot Prompting** : Demander au modèle de classifier le sentiment sans aucun exemple préalable.
2. **Few-Shot Prompting** : Fournir quelques exemples (paires entrée-sortie) pour orienter le modèle sur le format et le style attendus.
3. **Chain of Thought (CoT)** : Inciter le modèle à "réfléchir" étape par étape en décomposant son raisonnement avant de donner la classification finale.
4. **Gold Examples** : Utilisation d'exemples de référence parfaitement annotés pour servir de base de comparaison et d'évaluation.

---

## 🚀 Exécution du Projet

### 🧪 Étape 1 : Analyse et Expérimentation (Notebook)
Le notebook principal contient toute la logique de test des prompts :
1. **Chargement du Dataset** : Importation des données de test.
2. **Tests de Prompts** : Exécution successive des approches Zero-Shot, Few-Shot et CoT.
3. **Évaluation** : Comparaison des résultats obtenus par rapport aux étiquettes réelles.

### 🌐 Étape 2 : Lancement de l'Application
### 1. Initialisation du projet
```bash
# Entrer dans le répertoire
cd RAG-MULTIMODAL-EXPLO...

# Créer et activer l'environnement virtuel avec UV
uv venv
source .venv/bin/activate  # Sur Windows: .venv\Scripts\activate
```
### 2. Installation des dépendances
```bash
uv add langchain langchain-openai streamlit python-dotenv chromadb pypdf tiktoken
```
### 3. Configuration de la clé API
```bash
# Créez un fichier .env à la racine du projet :
OPENAI_API_KEY=votre_cle_api_ici
```
