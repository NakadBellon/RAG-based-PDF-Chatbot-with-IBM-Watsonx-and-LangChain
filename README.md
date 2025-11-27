# 🤖 Chatbot IA - RAG avec IBM Watsonx

Un chatbot intelligent basé sur l'architecture RAG (Retrieval-Augmented Generation) permettant d'interagir avec vos documents PDF en temps réel.

## ✨ Fonctionnalités

- **📄 Traitement de documents PDF** - Charge et analyse vos fichiers PDF
- **🔍 Recherche sémantique** - Trouve les informations les plus pertinentes dans vos documents
- **💬 Réponses contextuelles** - Génère des réponses précises basées sur le contenu de vos PDF
- **🛡️ IBM Watsonx** - Utilise des modèles de langage puissants et sécurisés
- **🎯 Interface intuitive** - Interface Gradio simple et conviviale

## 🚀 Architecture Technique

Ce projet implémente une architecture RAG complète :

```
Document PDF → Chargement → Découpage → Embeddings → Base vectorielle → LLM → Réponse
```

### Composants principaux

- **LangChain** - Orchestration du pipeline
- **ChromaDB** - Base de données vectorielle
- **IBM Watsonx** - Modèles de langage (Mixtral 8x7B) et embeddings
- **Gradio** - Interface utilisateur web

## 📦 Installation

```bash
# Cloner le projet
git clone <votre-repo>
cd chatbot-ia

# Installer les dépendances
pip install -r requirements.txt
```

### Dépendances principales

```python
ibm-watsonx-ai
langchain
langchain-ibm
chromadb
gradio
pypdf
```

## 🎯 Utilisation

1. **Lancez l'application** :
```python
python rag_chatbot.py
```

2. **Dans l'interface Gradio** :
   - Uploader votre fichier PDF
   - Poser votre question dans la zone de texte
   - Obtenir une réponse contextuelle instantanée

## 🔧 Configuration

Le projet utilise par défaut :
- **Modèle LLM** : `mistralai/mixtral-8x7b-instruct-v01`
- **Modèle d'embedding** : `ibm/slate-125m-english-rtrvr`
- **Project ID** : "skills-network" (IBM Cloud)

## 🏗️ Structure du code

```python
# Pipeline principal
document_loader()    # Chargement PDF
text_splitter()      # Découpage en chunks
watsonx_embedding()  # Génération d'embeddings
vector_database()    # Stockage vectoriel
retriever_qa()       # QA chain avec RAG
```

## 🌟 Points forts

- **Précision** : Réponses basées uniquement sur le document fourni
- **Performance** : Utilisation de modèles state-of-the-art
- **Simplicité** : Interface plug-and-play
- **Évolutivité** : Architecture modulaire facile à étendre

## 📊 Exemples d'utilisation

- **Recherche documentaire** - Interroger des rapports techniques
- **Support client** - Répondre à partir de manuels d'utilisation
- **Éducation** - Questions/réponses sur du matériel pédagogique
- **Recherche** - Analyse de documents académiques

## 🔮 Améliorations futures

- [ ] Support multi-documents
- [ ] Historique de conversation
- [ ] Export des réponses
- [ ] Interface mobile
- [ ] Personnalisation des modèles

## 🤝 Contribution

Les contributions sont les bienvenues ! N'hésitez pas à :
- Signaler des bugs
- Proposer des nouvelles fonctionnalités
- Améliorer la documentation

## 📄 Licence

Ce projet est open-source et disponible sous licence MIT.

---

*Développé avec ❤️ en utilisant IBM Watsonx, LangChain et Gradio*
