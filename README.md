# Page de vente – Formation montage vidéo sur téléphone

Site statique : `index.html` + dossier `media/` (vidéos). Aucun build, aucune installation.

## 1. Créer le repository sur GitHub
1. Connecte-toi sur github.com → bouton **New** (nouveau repository).
2. Nom : `page-vente-montage-video` → **Create repository**.
3. Clique sur **uploading an existing file**, puis glisse-dépose **tout le contenu de ce dossier** : `index.html`, `vercel.json`, `.gitignore` et le dossier `media`.
4. Clique sur **Commit changes**.

Avec Git en ligne de commande, à la place des étapes 3 et 4 :
```
git init
git add .
git commit -m "Page de vente"
git branch -M main
git remote add origin https://github.com/TON-COMPTE/page-vente-montage-video.git
git push -u origin main
```

## 2. Connecter le repository à Vercel
1. Sur vercel.com : **Add New… → Project**.
2. Choisis **Import Git Repository** et sélectionne `page-vente-montage-video`.
3. Réglages : **Framework Preset = Other**. Laisse **Build Command** et **Output Directory** vides.
4. Clique sur **Deploy**. Vercel te donne un lien du type `https://page-vente-montage-video.vercel.app`.

Chaque modification envoyée sur GitHub est ensuite redéployée automatiquement.

**Attention :** le plan gratuit de Vercel (Hobby) est réservé à un usage personnel non commercial. Une page de vente est un usage commercial : Vercel demande alors le plan Pro (payant). Netlify ou Cloudflare Pages se connectent à GitHub de la même façon : vérifie leurs conditions avant de choisir.

## 3. Ce que tu peux modifier dans `index.html`
- **Fin de l’offre** : cherche `var END` et change la date.
- **Prix** : cherche `5 000 F CFA` et `25 000 F CFA`.
- **Lien d’achat** : cherche `betxrepl.mychariow.shop` (il apparaît sur plusieurs boutons).
- **Pixel Facebook** : colle son code à l’endroit indiqué par le commentaire `PIXEL FACEBOOK`, en haut du fichier.
- **Numéros WhatsApp** : cherche `22606170412` et `22653911149`.
