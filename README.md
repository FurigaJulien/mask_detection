# mask_detection

## Mask detection model

Le notebook mask_detection_model contient le code permettant de creer le modèle utiliser pour la detection du masque.
Il a été créé pour tourner sur google collab.

## Video detection

La detection de la video se fait sur le notebook Video_detection. 
Elle est réalisé en deux étapes :
- Detection de visage avec cv2 classifier
- Crop de l'image et detection dans cette derniere du port du masque. Si il est bien porté, un smiley qui sourit apparait, 
sinon c'est un smiley triste accompagné d'un message vocal qui se repète toute les 15 secondes.
