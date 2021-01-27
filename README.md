# mask_detection

## Mask detection model

Le notebook mask_detection_model contient le code permettant de creer le modèle utiliser pour la detection du masque.
Il a été créé pour tourner sur google collab.

L'import se fait directement sur google drive. Le jue de donéne a été augmenté afin de pouvoir reconnaitre le masque lorsqu'il est sur le nez et le stipuler a l'utilisateur.

Les images sont redimensionné en 96x96 et traitées en couleur car de meilleurs resultat sont obtenus de cette facon.

### Reseau de neuronne

Un CNN a été utilisé, avec 3 couche de Conv2D, suivi d'un flatten et de 3 couches Denses. On obtient ainsi un resultat de 95% d'accuracy sur le jeu de donnée préalablement séparé pour le test.

## Video detection

La detection de la video se fait sur le notebook Video_detection. 
Elle est réalisé en deux étapes :
- Detection de visage avec cv2 classifier
- Crop de l'image et detection dans cette derniere du port du masque. Si il est bien porté, un smiley qui sourit apparait, 
sinon c'est un smiley triste accompagné d'un message vocal qui se repète toute les 15 secondes.
