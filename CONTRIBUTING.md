# Contributing to Open CV Builder

Merci de votre intérêt pour contribuer à Open CV Builder !  
Ce guide explique comment configurer le projet et contribuer correctement.

---

## 🏗 Structure du projet

- `app/` : pages et routing Next.js (App Router)  
- `features/` : logique métier modulaire (auth, CV, templates)  
- `lib/` : clients et helpers (Supabase, utils)  
- `types/` : types TypeScript globaux  
- `templates/` : modèles de CV (contributions open source)  

---

## 🔹 Règles générales

1. Respectez la structure du projet.  
2. Commits clairs et concis en suivant le format **Conventional Commits** :
   - `feat:` nouvelle fonctionnalité  
   - `fix:` correction de bug  
   - `chore:` modifications non fonctionnelles (docs, setup)  
3. Utilisez TypeScript strict et assurez-vous que le lint/format passe avant de commit.  
4. N’exposez jamais vos clés privées Supabase dans le code ou dans Git.  

---

## 🔹 Configuration pour les contributeurs

1. Copiez le fichier d’exemple `.env.local.example` :

```bash
cp .env.local.example .env.local

Remplissez vos propres variables si vous utilisez votre projet Supabase de test :

NEXT_PUBLIC_SUPABASE_URL=VOTRE_PROJECT_URL
NEXT_PUBLIC_SUPABASE_ANON_KEY=VOTRE_ANON_KEY


⚠️ Ne committez jamais vos clés privées.
Le fichier .env.local est ignoré par Git.

🔹 Ajouter un template de CV

1. Créez un dossier dans /templates :

templates/mon-template


2. Ajoutez un composant React exporté par défaut, par exemple Template.tsx :

export default function Template() {
  return <div>Mon modèle de CV</div>
}

3. Ajoutez un petit README pour décrire le template.

4. Créez une Pull Request avec vos changements.

## 🔹 Bugs et suggestions

- Ouvrez un issue sur GitHub pour tout bug ou amélioration.

- Les idées pour de nouveaux templates, fonctionnalités ou corrections sont les bienvenues.

## 🔹 Bonnes pratiques

Utilisez des branches descriptives :

feat/auth-login
fix/cv-download

Faites des commits atomiques et lisibles.

Respectez la structure et la typographie du code existant.

Merci encore pour votre contribution !
