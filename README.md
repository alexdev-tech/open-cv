# Open CV Builder

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

## Description

Open CV Builder est une plateforme open source pour créer, gérer et générer des CV professionnels directement depuis le navigateur.  
Elle est conçue pour être extensible : tout contributeur peut ajouter de nouveaux modèles de CV, fonctionnalités ou améliorations.

## 🛠 Stack technique

- **Frontend :** Next.js (App Router) + TypeScript + Tailwind CSS  
- **Backend :** Supabase (Auth, DB, Storage)  
- **CI/CD :** GitHub + Vercel (optionnel)  
- **Lint & format :** ESLint, Prettier  

## 📁 Structure du projet

app/ # Pages et routing Next.js App Router
features/ # Logique métier modulaire (auth, cv, templates)
lib/ # Clients et utilitaires (Supabase client, helpers)
types/ # Interfaces TypeScript globales
templates/ # Modèles de CV (contributions open source)


## Installation

1. Clone le repo :

```bash
git clone https://github.com/alexdev-tech/open-cv.git
cd open-cv

Installe les dépendances :

npm install

Crée un fichier .env.local :

NEXT_PUBLIC_SUPABASE_URL=ton_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=ton_supabase_anon_key

Lance l’application :

npm run dev

## 🤝 Contribuer

Voir le fichier CONTRIBUTING.md
pour les règles de contribution.

📄 License
Ce projet est sous licence MIT. Voir LICENSE
 pour plus de détails.

