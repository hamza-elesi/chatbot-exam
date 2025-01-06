# Assistant IA Multi-Modèles

Un chatbot intelligent utilisant plusieurs modèles d'IA (Google Gemini Pro et Groq Mixtral) avec une interface utilisateur Streamlit et un système avancé de détection d'intentions.

## 📋 Prérequis

- Python 3.9 ou supérieur
- Un compte Google AI Studio (pour l'API Gemini)
- Un compte Groq (pour l'API Groq)

## 🚀 Installation

1. Clonez le repository :
```bash
git clone <votre-repo>
cd <votre-dossier-projet>
```

2. Créez un environnement virtuel (recommandé) :
```bash
# Avec conda
conda create -n chatbot python=3.9
conda activate chatbot

# Ou avec venv
python -m venv env
source env/bin/activate  # Pour Linux/Mac
.\env\Scripts\activate   # Pour Windows
```

3. Installez les dépendances :
```bash
pip install streamlit google-generativeai groq python-dotenv
```

4. Créez un fichier `.env` à la racine du projet avec vos clés API :
```
GOOGLE_API_KEY=votre_clé_google_api
GROQ_API_KEY=votre_clé_groq_api
```

## 💻 Utilisation

1. Lancez l'application :
```bash
streamlit run app.py
```

2. Ouvrez votre navigateur à l'adresse indiquée (généralement http://localhost:8501)

3. Fonctionnalités :
   - Sélection du modèle d'IA (Gemini ou Groq)
   - Chat en temps réel avec détection d'intentions
   - Historique des conversations
   - Bouton pour effacer l'historique

## 🎯 Caractéristiques

- Interface utilisateur intuitive avec Streamlit
- Support multilingue (principalement français)
- Gestion des erreurs robuste
- Historique des conversations
- Système intelligent de détection d'intentions :
  * Salutations automatiques
  * Réponses aux remerciements
  * Gestion des demandes d'aide
  * Réponses aux questions d'humeur
  * Messages d'au revoir personnalisés

## 🤖 Capacités de Détection d'Intentions

Le chatbot peut reconnaître et répondre automatiquement à plusieurs types d'intentions :

1. **Salutations** :
   - Détecte : "bonjour", "salut", "hello", "hi"
   - Répond de manière appropriée et amicale

2. **Questions sur l'humeur** :
   - Comprend : "comment vas-tu", "ça va"
   - Fournit des réponses personnalisées

3. **Demandes d'aide** :
   - Reconnaît : "aide", "help", "sos"
   - Propose des suggestions d'assistance

4. **Remerciements** :
   - Identifie : "merci", "thanks"
   - Répond poliment

5. **Messages d'au revoir** :
   - Détecte : "au revoir", "bye", "à bientôt"
   - Conclut la conversation de manière appropriée

## ⚠️ Limitations actuelles

1. **Gestion du contexte** :
   - La conversation est réinitialisée lors du changement de modèle
   - Limite de longueur pour l'historique des conversations

2. **Performance** :
   - Temps de réponse variable selon le modèle et la charge des serveurs
   - Pas de gestion des timeouts

3. **Fonctionnalités** :
   - Pas de support pour les images ou les fichiers
   - Pas de persistance des conversations entre les sessions

## 🔄 Pistes d'amélioration

1. **Intelligence Conversationnelle** :
   - Étendre le système de détection d'intentions
   - Ajouter plus de patterns de reconnaissance
   - Améliorer la gestion du contexte conversationnel

2. **Fonctionnalités** :
   - Ajouter le support des images et fichiers
   - Implémenter la sauvegarde des conversations
   - Ajouter un système de favoris pour les réponses
   - Intégrer plus de modèles d'IA

3. **Interface** :
   - Ajouter des thèmes personnalisables
   - Améliorer la mise en forme des réponses
   - Ajouter des indicateurs de typing
   - Implémenter un mode sombre

4. **Performance** :
   - Optimiser la gestion de la mémoire
   - Ajouter un système de cache
   - Implémenter un fallback entre les modèles

5. **Sécurité** :
   - Ajouter un système d'authentification
   - Chiffrer les conversations
   - Implémenter des limites de rate

## 🔐 Sécurité

- Ne partagez jamais vos clés API
- Ajoutez le fichier `.env` à votre `.gitignore`
- Surveillez votre utilisation des API

## 📜 Licence

ESI SCHOOL

## 👥 Contact

Hamza EL MAATAOUI - ICSD
