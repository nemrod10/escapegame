# Mission mBot déraille
## Scénario complet – Game of Tech

---

## Thème
**Réparabilité et diagnostic d'un objet programmable – le mBot**

---

## Objectif pédagogique
Amener les élèves à :
- Identifier l'origine d'un dysfonctionnement à partir d'observations.
- Vérifier successivement différents éléments d'un système technique (programme, branchements, mécanique).
- Comprendre le lien entre **fonction technique**, **chaîne d'énergie** et **chaîne d'information**.
- Proposer une **solution de réparation réaliste** (ici, remplacement d'un engrenage).

---

## Décor narratif
Le club de robotique prépare une démonstration importante devant la classe.  
Mais catastrophe — **le mBot tourne en rond sans avancer droit !**  
L'équipe des apprentis réparateurs est appelée en urgence pour **identifier la cause du problème et le résoudre avant la présentation.**

Chaque étape franchie débloque des indices (visuels, sons, schémas) jusqu'à la solution finale.  

---

## Déroulement du jeu

### **Étape 1 – Vérification du programme**
L'élève visionne le code dans l'interface (Makeblock, mBlock ou équivalent).  
Deux blocs sont visibles : avancer à vitesse 100 les deux moteurs A et B.  
Mais un joueur attentif remarque que le **moteur B est réglé à vitesse -100** !  

**Objectif** : Corriger la direction ou confirmer que le code est correct.  
**Si le joueur remet la bonne valeur** : l'erreur persiste → passage à l'étape suivante.  

💡 **Indice** : le programme semble correct, mais le robot continue à tourner.

**Choix proposés** :
1. « Le moteur gauche est à 100 et le moteur droit à 0 »
2. « Le moteur gauche est à 100 et le moteur droit à -100 »
3. ✅ « Les deux moteurs sont à 100, tout est normal »

**Feedback bon choix** :  
*« Bien vu ! le programme est correct, mais le robot continue à tourner en rond. Il doit y avoir un autre problème. »*

---

### **Étape 2 – Vérification des branchements moteurs**
Le joueur consulte le schéma de câblage.  
- Moteur gauche → Port M1  
- Moteur droit → Port M2  

**Objectif** : Vérifier virtuellement les câbles (cliquer ou tester chaque port).  
Tout est bien branché.  

💡 **Indice** : les ports sont corrects. Ce n'est donc pas un problème d'inversion.

**Choix proposés** :
1. « Les deux moteurs sont branchés sur le même port »
2. ✅ « Le moteur gauche est sur M1 et le moteur droit sur M2, tout est correct »
3. « Aucun moteur n'est branché »

**Feedback bon choix** :  
*« Les branchements des moteurs sont corrects. Le problème ne vient pas du port utilisé. Continuons l'enquête. »*

---

### **Étape 3 – Inspection des câbles**
Un testeur virtuel permet de "mesurer" la continuité du câble (outil visuel ou animation).  
Aucun défaut n'est trouvé.  

💡 **Indice sonore** : un bruit de moteur se fait entendre du côté droit, mais la roue ne bouge pas.

**Choix proposés** :
1. « Le câble du moteur gauche est coupé »
2. « Les deux câbles sont débranchés »
3. ✅ « Les câbles semblent en bon état et correctement branchés »

**Feedback bon choix** :  
*« Les câbles sont en bon état. Pourtant, le robot tourne toujours en rond. Il faut observer plus finement le comportement des roues. »*

---

### **Étape 4 – Observation fine**
Le joueur observe un schéma fonctionnel ou une vidéo du robot en action : **le moteur tourne à l'intérieur**, mais **la roue ne suit pas le mouvement.**  

💡 **Indice** : un engrenage interne semble cassé.

**Choix proposés** :
1. « La roue tourne normalement, tout va bien »
2. ✅ « On entend le moteur tourner mais la roue ne bouge presque pas »
3. « La roue est complètement bloquée et le moteur est silencieux »

**Feedback bon choix** :  
*« Exact ! Le moteur semble tourner mais la roue ne suit pas. Il y a probablement un problème dans la transmission mécanique. »*

---

### **Étape 5 – Diagnostic final et réparation**
Le joueur ouvre virtuellement le moteur : l'engrenage plastique est fendu.  

**Objectif** : Le joueur choisit la solution la plus pertinente.  
L'IA (ou le script du jeu) valide la logique du choix en expliquant les conséquences techniques.

**Choix proposés** :
1. « Reprogrammer le mBot »  
2. « Remplacer le moteur complet »
3. ✅ **« Changer seulement l'engrenage défectueux »**

**Feedback bon choix** :  
*« Très bon choix ! Remplacer uniquement l'engrenage cassé est une solution économique et durable. Tu as réparé le mBot. »*

Une fiche "Réparabilité" s'affiche alors :
> ✅ **Problème résolu : engrenage cassé remplacé.**  
> 🔧 **Compétences mobilisées** : analyser, identifier une panne, concevoir une solution durable.  
> 🌱 **Impact** : prolongation de la durée de vie du produit.

---

## Variante ludique
- Intégrer un **chrono** (5 minutes pour trouver la panne).  
- Chaque mauvaise hypothèse fait perdre du "temps atelier".  
- Ajouter des **badges virtuels** : "Diagnostic rapide", "Éco‐réparateur", "Maître des engrenages".

---

## Variante « escape game »
Chaque bonne réponse débloque un code pour ouvrir des fichiers numériques verrouillés (plan électrique, schéma 3D, firmware, etc.).  
But final : réactiver la machine avant la fin du chrono.

---

## Outils possibles

### Pour prototyper rapidement :
- **Genially** ou **Canva interactif** pour le prototype.  
- **IA générative** (ChatGPT, Claude, DALL·E) : créer les visuels du mBot, engrenage cassé, ou sons de moteur.  
- **HTML animé** : créer un mini-script HTML avec des boutons permettant de tester les hypothèses.  
- **Intégration IA** : simulent l'assistant technique du labo via un chatbot IA.

### Pour le développement final :
- Framework JS (Vue, React, Svelte)
- Plateforme LMS (Moodle, Canvas)
- Outil d'escape game dédié (Escape Classroom, etc.)

---

## Compétences travaillées (pour le professeur)

### Domaines du programme AEFE technologie :
- **Analyser** : Observer un dysfonctionnement et formuler des hypothèses logiques.
- **Concevoir** : Proposer une solution adaptée et durable aux contraintes.
- **Réaliser** : Identifier les éléments d'un système technique (programme, branchement, mécanique).
- **Valider** : Vérifier chaque piste de diagnostic successivement.

### Transversalités :
- **Chaîne d'information** : programme, branchement, signal électrique.
- **Chaîne d'énergie** : moteur, transmission mécanique, roue.
- **Développement durable** : réparabilité, allongement de la durée de vie, réduction des déchets.
- **Démarche scientifique** : observation, hypothèse, test, conclusion.

---

## Durée estimée
- **1 séance de 45-50 min** pour une classe complète.
- **Version accélérée** : 30 min (skip certains feedbacks).
- **Approfondissement** : 1h30 avec démontage/remontage réel du mBot après le jeu.

---

## Ressources à prévoir

### Pour l'enseignant :
- Un mBot (ou photo du mBot) pour montrer en vrai.
- Les engrenages de rechange du moteur (pour la démo finale).
- Un écran pour projeter le jeu.

### Pour les élèves :
- Un ordinateur (ou 2-3 par petit groupe).
- Le jeu interactif (HTML ou Genially).
- Fiche de synthèse à remplir (diagnostic trouvé, solution choisie).

---

## Notes pédagogiques

1. **Guidage progressif** : chaque étape guide doucement l'élève, sans lui donner la réponse directement.
2. **Authenticité technique** : les problèmes et solutions reflètent la vraie réalité du mBot.
3. **Ludification** : les badges, le chrono et la narration maintiennent l'engagement.
4. **Accessibilité** : adaptable à tous les niveaux (5e à 3e, voire lycée pro).
5. **Réutilisabilité** : facilement adaptable à d'autres systèmes techniques (lampe, chaîne d'énergie, capteurs, etc.).

---

## Exemple de prompt IA pour générer le contenu

Si tu veux que une IA génère automatiquement textes, images et structure interactive :

> **Tu es un expert en pédagogie de la technologie au collège et en game design éducatif.**  
> **Ta mission** : créer un serious game / escape game numérique pour des élèves de 5e/4e autour de la **réparabilité** et du **diagnostic de panne d'un robot mBot**.  
> 
> **Contexte** : Le club de robotique prépare une démo. Le mBot tourne en rond. Les élèves jouent une équipe de techniciens.  
> 
> **Étapes** :
> 1. Vérifier le programme (moteur à vitesse -100)
> 2. Vérifier les branchements (M1/M2 OK)
> 3. Tester les câbles (tous OK)
> 4. Observer le comportement (moteur tourne, roue bloquée)
> 5. Remplacer engrenage cassé
> 
> **Sortie attendue** : Scénario détaillé + code HTML interactif + suggestions d'images à générer.

---

**Document créé pour la formation AEFE – Stage de zone technologie, décembre 2025, Bogotá.**
