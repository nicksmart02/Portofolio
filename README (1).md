# 🔐 Nicolas AHADJITSE — Cybersecurity Portfolio

> Portfolio professionnel single-page pour étudiant en cybersécurité.  
> Dark mode glassmorphism · Palette bleu/violet · Orange/rouge en mode clair · 100% standalone

---

## ⚡ Lancement rapide

```bash
# Ouvrir directement — aucune installation requise
double-clic sur index.html
```

Ou avec un serveur local (meilleur rendu des polices Google) :

```bash
# Python 3
python3 -m http.server 8080
# → http://localhost:8080

# Node.js
npx serve .
# → http://localhost:3000
```

---

## 📁 Structure

```
portfolio/
└── index.html      ← Fichier unique autonome (HTML + CSS + JS inlinés)
└── README.md       ← Ce fichier
```

> Tout le code est dans **un seul fichier** `index.html`.  
> Pas de dépendances. Pas de build. Pas de framework.

---

## 🎨 Design

| Élément | Dark mode | Light mode |
|---|---|---|
| Background | Bleu nuit `#050c18` | Crème chaud `#fffaf4` |
| Accent 1 | Bleu `#3b82f6` | Orange `#ea580c` |
| Accent 2 | Violet `#8b5cf6` | Rouge `#b91c1c` |
| Accent 3 | Cyan `#06b6d4` | Vert `#15803d` |
| Texte | `#e2eaff` | `#1c0a00` |

- Glassmorphism avec `backdrop-filter: blur`
- Polices : **Orbitron** (titres) · **Share Tech Mono** (code) · **Rajdhani** (corps)
- Curseur personnalisé + ring animé
- Fond de particules interactif (canvas)

---

## 📑 Sections

| # | Section | Contenu |
|---|---|---|
| 01 | **Hero** | Nom, typing effect (7 phrases), avatar animé, boutons CV + Contact |
| 02 | **About** | Présentation, intérêts, compteurs (projets / labs / techs / certs) |
| 03 | **Skills** | 10 barres de progression animées + cloud de 12 badges technos |
| 04 | **Projects** | 6 cartes filtrables + modals détaillées (GitHub + Demo) |
| 05 | **Timeline** | Parcours académique et professionnel animé |
| 06 | **Certifications** | 4 cards (ISC², TryHackMe, HackTheBox, LPI) avec preview |
| 07 | **Stats** | 4 compteurs animés au scroll |
| 08 | **Terminal** | Terminal interactif avec 15 commandes |
| 09 | **Contact** | Formulaire validé JS + liens GitHub / LinkedIn / Email |
| 10 | **Footer** | Navigation, réseaux sociaux, copyright |

---

## 🖥️ Terminal — Commandes disponibles

```bash
whoami       # Présentation de Nicolas
skills       # Compétences détaillées
projects     # Liste des 6 projets
certs        # Certifications
contact      # Coordonnées
education    # Parcours académique
hack         # Easter egg 😄
help         # Toutes les commandes
clear        # Vider le terminal
ls           # Fichiers du portfolio
pwd          # Répertoire courant
date         # Date et heure
uname        # Info système
uptime       # Uptime
```

**Raccourci clavier :** `Ctrl + /` → focus direct sur le terminal  
**Historique :** flèches `↑` `↓`  
**Autocomplétion :** touche `Tab`

---

## 🔧 Fonctionnalités JS

- **Particles** — fond de particules connectées, interactives avec la souris
- **Typing effect** — rotation de 7 titres avec effet machine à écrire
- **Scroll reveal** — apparition progressive des éléments au scroll
- **Skill bars** — animation déclenchée à l'entrée dans le viewport
- **Counters** — compteurs ease-out cubic au scroll
- **Project filters** — filtrage par catégorie (All / Detection / Web / Hardening / CTF)
- **Project modals** — popup détaillée pour chaque projet
- **Cert preview** — modal de prévisualisation des certificats
- **Contact form** — validation en temps réel (blur) + simulation d'envoi
- **Dark/Light toggle** — préférence sauvegardée en `localStorage`
- **Smooth scroll** — navigation fluide entre sections
- **Active nav** — highlight automatique de la section visible
- **Mobile menu** — burger menu animé pour mobile

---

## 📱 Responsive

| Breakpoint | Layout |
|---|---|
| `> 1024px` | Grille 3 colonnes projets, 4 stats |
| `768px – 1024px` | Grille 2 colonnes projets |
| `< 768px` | Colonne unique, menu burger, timeline verticale gauche |
| `< 480px` | Padding réduit, textes adaptés |

---

## ✏️ Personnalisation

Tout est dans `index.html`. Les zones clés :

```
Nom / Titre         → Section <section id="hero"> — .hero-name
Typing phrases      → JS : const phrases = [...]
Photo / Avatar      → .avatar-initials (remplacer "NA" par une <img>)
Projets             → JS : const projectData = [...]
Liens sociaux       → href="#" → remplacer par vos URLs
CV download         → <a href="#" ... download> → mettre le chemin du PDF
Certifications      → Section #certs — remplacer les PDF dans btn-cert
Couleurs dark       → CSS :root { ... }
Couleurs light      → CSS [data-theme="light"] { ... }
```

---

## 🌐 Compatibilité

| Navigateur | Support |
|---|---|
| Chrome / Edge | ✅ Complet |
| Firefox | ✅ Complet |
| Safari | ✅ Complet (webkit prefixes inclus) |
| Mobile Chrome | ✅ Responsive |
| Mobile Safari | ✅ Responsive |

> ⚠️ `backdrop-filter` non supporté sur Firefox < 103 sans flag.  
> Le glassmorphism se dégrade gracieusement (fond opaque).

---

## 📄 Licence

Usage personnel libre. Crédits appréciés 🙏

---

*Built with passion & code — Nicolas AHADJITSE · 2025*
