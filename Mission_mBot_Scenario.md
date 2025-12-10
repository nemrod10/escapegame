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

# Prompt IA « Mission mBot déraille »

## Rôle et objectif

Tu es un expert en pédagogie de la technologie au collège et en game design éducatif.  
Ta mission est de créer un **serious game** / **escape game** numérique pour des élèves de 5e/4e autour de la **réparabilité** et du **diagnostic de panne d’un robot mBot**. L’activité doit être ludique, progressive et guidée, tout en restant exploitable en classe de technologie.

---

## Titre du jeu

**Mission mBot déraille : réparer le robot qui tourne en rond**

---

## Contexte narratif

Le club de robotique du collège prépare une démonstration importante. Au moment de lancer le robot, le mBot se met à **tourner en rond** au lieu d’avancer tout droit.  

Les élèves jouent le rôle d’une équipe de jeunes techniciens chargés de **diagnostiquer la panne** et de **proposer une solution de réparation durable**, sans remplacer inutilement tout le robot.

---

## Objectifs pédagogiques

Amener les élèves à suivre une **démarche de diagnostic** : observer, émettre des hypothèses, tester, conclure.

Vérifier successivement :

- Le **programme**
- Le **branchement des moteurs**
- L’**état des câbles**
- Le **comportement mécanique du moteur et de la roue**
- La **pièce défectueuse** (engrenage cassé) et la solution de réparation

Faire découvrir la notion de **réparabilité** : changer une pièce plutôt que jeter tout l’objet.

---

## Structure du jeu souhaitée

Le jeu est découpé en **5 étapes**, avec à chaque fois :

- une **mise en situation courte**,
- une **action de l’élève** (choix, manipulation, observation),
- un **feedback immédiat** (indice, validation, explication courte).

Le ton doit être engageant, clair, adapté à des collégiens.

---

## Étape 1 – Vérifier le programme

Le robot tourne en rond. Première hypothèse : le problème vient du code.

- Propose une interface fictive où l’élève voit un programme de type mBlock / Scratch (sans reproduire un logiciel précis).  
- L’élève doit :
  - analyser les blocs de commande des moteurs (moteur gauche / moteur droit),
  - vérifier si les vitesses sont cohérentes (ex. les deux à 100, et pas l’un à 100 et l’autre à -100).

L’élève corrige un défaut de sens de rotation mais que le robot **continue à tourner en rond** dans le récit, affiche un message du type :

> « Le programme est maintenant correct, mais le mBot tourne toujours en rond. Il doit y avoir un autre problème. »

---

## Étape 2 – Vérifier le branchement des moteurs

On demande à l’élève de vérifier les ports des moteurs (M1 / M2) sur le schéma du robot.

- L’élève doit confirmer que le moteur gauche et le moteur droit sont bien branchés aux bons ports.  
- Proposer plusieurs options de réponse (correct, inversé, débranché).

Si tout est bien branché, message :

> « Les moteurs sont bien branchés. Le problème ne vient pas de là. Continuons l’enquête. »

---

## Étape 3 – Tester les câbles

Le jeu simule l’utilisation d’un testeur de continuité ou d’un simple contrôle visuel des câbles.

L’élève choisit des actions du type :

- « Inspecter le câble du moteur gauche »
- « Inspecter le câble du moteur droit »

Tous les câbles sont déclarés en bon état dans la narration.

Indice à la fin :

> « Les câbles sont intacts. Pourtant, on entend un moteur tourner… »

---

## Étape 4 – Observer le comportement mécanique

L’élève observe (par description textuelle ou image) que :

- du côté d’une roue, on entend bien le moteur tourner,
- mais la roue ne bouge pas ou tourne très peu.

Demande à l’élève de formuler une hypothèse :

- roue desserrée,
- problème de friction avec le sol,
- transmission mécanique interne défectueuse (engrenage).

Amener progressivement à l’idée que le **moteur tourne mais la transmission ne transmet pas le mouvement**.

---

## Étape 5 – Diagnostic final et réparabilité

Révéler dans la narration que le démontage virtuel du moteur montre un **engrenage en plastique cassé**.

Proposer plusieurs solutions :

- Reprogrammer encore le robot.
- Remplacer tout le moteur complet.
- **Remplacer uniquement l’engrenage cassé.**

L’élève doit choisir la solution la plus **pertinente, économique et durable** (la 3).

Donner une explication courte et pédagogique sur la **réparabilité et l’allongement de la durée de vie des objets techniques**.

---

## Sortie attendue de ta part

Génère :

- Le **scénario détaillé** du jeu, étape par étape, sous forme de texte structuré exploitable par un enseignant.
- Pour chaque étape :
  - les textes à afficher à l’élève (consignes, narration, feedback),
  - les choix proposés (QCM, clic, mini-interaction),
  - le feedback associé à chaque choix.
- Une version **facilement transformable en activité numérique** :
  - soit sous forme de storyboard pour Genially / Canva interactif,
  - soit sous forme de structure HTML (div, boutons, zones de texte) sans CSS.
- Un court paragraphe final qui résume les **compétences travaillées** (diagnostic, analyse fonctionnelle, réparabilité) pour le professeur de technologie.

---

## Contraintes de style

- Langue : **français**, registre accessible à des collégiens.
- Phrases courtes, claires.
- Ton motivant, bienveillant, avec un vocabulaire technique juste mais expliqué simplement.
- Ne pas citer de marque de logiciel, mais parler de « logiciel de programmation par blocs » ou de « plateforme de programmation ».
