# Veille-technologique-p8

Le projet de formation se divise en deux parties principales :

### Première partie : Dashboard de Scoring Client
L'objectif est de développer un dashboard interactif pour les chargés de relation client de "Prêt à dépenser". Ce dashboard expliquera de manière transparente les décisions d'octroi de crédit en utilisant les données et API de scoring existantes. Il affichera : le score de crédit, la probabilité de remboursement, des comparaisons descriptives entre un client et l'ensemble des clients, le dashboard doit respecter les critères d'accessibilité WCAG.

### Deuxième partie : État de l'Art et Proof of Concept
Cette partie vise à comparer une technique récente de modélisation de données texte ou images avec une approche classique déjà implémentée. Un proof of concept sera développé pour illustrer l'application pratique de la nouvelle technique.

### Étapes clés :

- Sélection du Dataset : utilisation de 1050 images de biens de consommation
- Sélection de l'algorithme CLIP d'Open AI pour évaluer la similarité entre images et textes.
- Mise en œuvre d'un modèle basé sur l'encodeur d'image de CLIP avec des couches de réseau de neurones linéaires et activation ReLU.
- Comparaison avec VGG16 : CLIP atteint une précision supérieure (~90%) avec moins d'itérations d'entraînement comparé à VGG16 (~80%).
- Utilisation de LIME pour analyser les segments d'image importants pour les prédictions du modèle.
- Interprétabilité des Résultats : interprétabilité avec LIME et proposition d'utiliser SHAP pour une visualisation alternative.
- Limitations Identifiées : Limites dues au nombre limité d'images d'entraînement et à la spécificité des données initiales de CLIP.
- Conclusion sur les Performances : CLIP offre des performances supérieures à VGG16 avec moins d'itérations, démontrant son efficacité pour la classification des produits de consommation.

### Livrables :
**Gamba_Lucas_2_notebook_veille_062024** :
Contient le code pour la réalisation de la veille technologique qui se décompose en quatres grande partie :
 * Approche en "zero shot" sans entraînement préalable de l'algorithme CLIP, en utilisant à les descriptions textuelles et les images des différents produits,
 * Approche "Fine-Tuning" en entraînant des couches linéaires en sortie de l'encodeur image de CLIP,
 * Comparaison des performances du modèle avec celles de VGG16,
 * Analyse des segements d'images les plus important dans les prédictions de chaque catégories par le modèle.

**Gamba_Lucas_3_note_méthodologique_062024** :
"Proof Of Concept" décrivant la méthodologie appliquée lors de la veille technologique, justifiant les choix technique et énonçant leurs limites.

**Gamba_Lucas_4_presentation_062024** :
Présentation Power Point des graphiques du dashbord et de la veille technologique.
