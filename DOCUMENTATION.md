# DOCUMENTATION — Projet 1 Web 2

Site : Ascension (gym d’escalade)

---

## 1. Comment j’ai commencé

Pour commencer, j’ai regardé la maquette Figma en détail.

J’ai essayé de comprendre :

* les espacements
* les couleurs
* comment les sections sont organisées
* comment les éléments sont placés (grâce à auto-layout → Flexbox)

Après ça, j’ai planifié mon code avant de commencer à coder.

---

## 2. Ma façon de nommer les classes (BEM)

J’ai utilisé la méthode **BEM**.

Exemples :

* `.nav` → le composant
* `.nav__menu` → un élément dedans
* `.hero__button--accent` → une variante

Pourquoi j’ai choisi ça ?

* c’est plus clair
* plus facile à lire
* plus facile à modifier plus tard

---

## 3. Mes variables CSS (design tokens)

J’ai mis toutes mes variables dans `:root`.

### Couleurs

* bleu foncé → fond du site
* orange → boutons
* blanc → texte
* gris → texte secondaire

### Espacements

* petit → `--space-sm`
* moyen → `--space-md`
* grand → `--space-lg`

### Fonts

* une pour le texte
* une pour les boutons

Pourquoi ?

* pour garder tout propre
* pour éviter de répéter les valeurs partout
* pour changer facilement le design

---

## 4. Les composants que j’ai créés

J’ai séparé mon site en plusieurs parties :

* navbar
* hero
* section titres
* cartes (services, prix, etc.)
* formulaire
* footer

Ça rend le code plus organisé et réutilisable.

---

## 5. Flexbox (le plus important)

J’ai utilisé Flexbox partout.

Exemples :

### Navbar

```css
display: flex;
justify-content: space-between;
align-items: center;
```

### Cartes

```css
display: flex;
gap: 1rem;
flex-wrap: wrap;
```

### Hero

```css
display: flex;
align-items: center;
```

Pourquoi ?

* ça permet de bien aligner les éléments
* ça rend le site flexible
* ça correspond à Figma

---

## 6. Fonctions CSS que j’ai utilisées

### clamp()

```css
font-size: clamp(2rem, 4vw, 3rem);
```

→ le texte change selon la taille de l’écran

### min()

```css
width: min(1200px, 100%);
```

→ limite la largeur du site

### calc()

→ utilisé pour certains espacements

Pourquoi ?

* pour rendre le design plus flexible
* sans utiliser de media queries

---

## 7. Mes choix techniques

* j’ai utilisé Flexbox (pas Grid, car interdit)
* j’ai fait des composants réutilisables
* j’ai utilisé des variables pour tout le design
* j’ai mis l’image du hero en background avec un overlay

---

## 8. Problèmes que j’ai eus

### 1. CSS ne marchait pas

Problème :
le style ne s’affichait pas

Solution :
le fichier CSS n’était pas bien relié (erreur de nom)

---

### 2. Menu mal aligné

Problème :
les éléments étaient un en dessous de l’autre

Solution :
j’ai ajouté `display: flex`

---

### 3. Image du hero

Problème :
l’image ne s’affichait pas

Solution :
j’ai utilisé `background-image` dans le CSS

---

## 9. Utilisation de l’IA

**Outil :** ChatGPT  
**Version :** GPT-5.3  

J’ai utilisé l’IA pour m’aider à différents moments du projet :

### Corriger des erreurs
- CSS qui ne marchait pas (problème de lien avec le HTML)
- menu mal aligné (les éléments se mettaient un en dessous de l’autre)
- problèmes avec Flexbox

### Mieux comprendre
- comment fonctionne Flexbox (alignement, espaces)
- comment utiliser BEM pour nommer les classes
- comment utiliser les variables CSS
- comment utiliser `clamp()`, `min()` et `calc()`

### Améliorer mon code
- rendre le design plus propre
- ajuster les espacements
- améliorer les boutons
- ajouter l’image du hero avec un overlay

### Je n’ai pas juste copié le code.
J’ai :
- testé moi-même
- modifié le code
- compris ce que je faisais
---

## 10. Conclusion

Ce projet m’a aidé à :

* mieux comprendre Flexbox
* organiser mon code
* transformer une maquette en site web
* utiliser des variables CSS

---
