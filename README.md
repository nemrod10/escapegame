# escapegame

Prompt IA « Mission mBot déraille »
Rôle et objectif
Tu es un expert en pédagogie de la technologie au collège et en game design éducatif.
Ta mission est de créer un serious game / escape game numérique pour des élèves de 5e/4e autour de la réparabilité et du diagnostic de panne d’un robot mBot. L’activité doit être ludique, progressive et guidée, tout en restant exploitable en classe de technologie.

Titre du jeu
Mission mBot déraille : réparer le robot qui tourne en rond

Contexte narratif
Le club de robotique du collège prépare une démonstration importante. Au moment de lancer le robot, le mBot se met à tourner en rond au lieu d’avancer tout droit.
Les élèves jouent le rôle d’une équipe de jeunes techniciens chargés de diagnostiquer la panne et de proposer une solution de réparation durable, sans remplacer inutilement tout le robot.

Objectifs pédagogiques

Amener les élèves à suivre une démarche de diagnostic : observer, émettre des hypothèses, tester, conclure.

Vérifier successivement :

Le programme

Le branchement des moteurs

L’état des câbles

Le comportement mécanique du moteur et de la roue

La pièce défectueuse (engrenage cassé) et la solution de réparation.

Faire découvrir la notion de réparabilité : changer une pièce plutôt que jeter tout l’objet.

Structure du jeu souhaitée
Le jeu est découpé en 5 étapes, avec à chaque fois :

une mise en situation courte,

une action de l’élève (choix, manipulation, observation),

un feedback immédiat (indice, validation, explication courte).
Le ton doit être engageant, clair, adapté à des collégiens.

Étape 1 – Vérifier le programme

Le robot tourne en rond. Première hypothèse : le problème vient du code.

Propose une interface fictive où l’élève voit un programme de type mBlock / Scratch (sans reproduire un logiciel précis).

L’élève doit :

analyser les blocs de commande des moteurs (moteur gauche / moteur droit),

vérifier si les vitesses sont cohérentes (ex. les deux à 100, et pas l’un à 100 et l’autre à -100).

Si l’élève corrige un éventuel défaut de sens de rotation mais que le robot continue à tourner en rond dans le récit, affiche un message du type :

« Le programme est maintenant correct, mais le mBot tourne toujours en rond. Il doit y avoir un autre problème. »

Étape 2 – Vérifier le branchement des moteurs

On demande à l’élève de vérifier les ports des moteurs (M1 / M2) sur le schéma du robot.

L’élève doit confirmer que le moteur gauche et le moteur droit sont bien branchés aux bons ports.

Proposer plusieurs options de réponse (correct, inversé, débranché).

Si tout est bien branché, message :

« Les moteurs sont bien branchés. Le problème ne vient pas de là. Continuons l’enquête. »

Étape 3 – Tester les câbles

Le jeu simule l’utilisation d’un testeur de continuité ou d’un simple contrôle visuel des câbles.

L’élève choisit des actions du type :

« Inspecter le câble du moteur gauche »,

« Inspecter le câble du moteur droit ».

Tous les câbles sont déclarés en bon état dans la narration.

Indice à la fin :

« Les câbles sont intacts. Pourtant, on entend un moteur tourner… »

Étape 4 – Observer le comportement mécanique

L’élève observe (par description textuelle ou image) que :

du côté d’une roue, on entend bien le moteur tourner,

mais la roue ne bouge pas ou tourne très peu.

Demande à l’élève de formuler une hypothèse :

roue desserrée,

problème de friction avec le sol,

transmission mécanique interne défectueuse (engrenage).

Amener progressivement à l’idée que le moteur tourne mais la transmission ne transmet pas le mouvement.

Étape 5 – Diagnostic final et réparabilité

Révéler dans la narration que le démontage virtuel du moteur montre un engrenage en plastique cassé.

Proposer plusieurs solutions :

Reprogrammer encore le robot.

Remplacer tout le moteur complet.

Remplacer uniquement l’engrenage cassé.

L’élève doit choisir la solution la plus pertinente, économique et durable (la 3).

Donner une explication courte et pédagogique sur la réparabilité et l’allongement de la durée de vie des objets techniques.

Sortie attendue de ta part
Génère :

Le scénario détaillé du jeu, étape par étape, sous forme de texte structuré exploitable par un enseignant.

Pour chaque étape,

les textes à afficher à l’élève (consignes, narration, feedback),

les choix proposés (QCM, clic, mini-interaction),

le feedback associé à chaque choix.

Une version facilement transformable en activité numérique :

soit sous forme de storyboard pour Genially / Canva interactif,

soit sous forme de structure HTML (div, boutons, zones de texte) sans CSS.

Un court paragraphe final qui résume les compétences travaillées (diagnostic, analyse fonctionnelle, réparabilité) pour le professeur de technologie.

Contraintes de style

Langue : français, registre accessible à des collégiens.

Phrases courtes, claires.

Ton motivant, bienveillant, avec un vocabulaire technique juste mais expliqué simplement.

Ne pas citer de marque de logiciel, mais parler de « logiciel de programmation par blocs » ou de « plateforme de programmation ».
