# COMPLEXITES

*Bienvenu dans notre simulateur de **rice cooker***

*Vous pouvez voir ici une seul branche qui contient le refactoring que j'ai fait pour le code de **Mayah** dans [cc-d4-rice-cooker-ci-NyAndoMayah](https://github.com/hei-school/cc-d4-rice-cooker-ci-NyAndoMayah/blob/feat/js/js/main.js)*

*Vous pouvez voir les listes de fonctionnalites dans son readme ainsi que les installation necessaire une fois vous clonner le projet mais dans ce readme , vous verrez plutot **la liste des complexites de nos codes a toutes les deux***

## Mayah

1. **Complexité temporelle :**
   - `delaySync` cause des problèmes de performance

2. **Complexité structurelle :**
   - `simulateRiceCooker` utilise une boucle while infinie parce que `condition est toujour true`. 

3. **Répétition de la logique de menu :**
   - La logique de traitement du choix utilisateur dans la boucle `while` de `simulateRiceCooker` pourrait être encapsulée de manière plus modulaire. 

4. **Structure monolithique :**
   - Les fonctions de l'objet `riceCooker` effectuent plusieurs tâches, ce qui peut rendre le code moins modulaire.

5. **Boucle bloquante :**
   - `delaySync` peut empêcher d'autres tâches de s'effectuer pendant ce temps.

6. **Utilisation de `parseInt` et `isNaN` :**
   - On peut utiliser d'autre methode plus performant

7. **Absence de gestion explicite des erreurs :**
   - Le code ne gère pas explicitement les erreurs, ce qui peut rendre le débogage plus difficile.

## Refactoring

1. **Complexité temporelle :**
   - `delaySync` cause des problèmes de performance

2. **Boucle infinie :**
   - La boucle while infinie dans la fonction `simulateRiceCooker` est toujours présente.

3. **Logique d'entrée utilisateur :**
   - La gestion de l'entrée utilisateur a été améliorée avec la vérification de l'entrée vide (`input==""`) mais le code pourrait être plus amélioré. 

4. **Retour de la fonction `addRice` :**
   - `addRice` retourne maintenant une chaîne de caractères au lieu d'afficher directement dans la console. 

5. **Répétition de la logique de menu :**
   - Le traitement du choix d'utilisateur dans `simulateRiceCooker` a été mais pourrait l'être encore plus .  

6. **Encapsulation des fonctionnalités dans `riceCooker` :**
   - Les fonctions de l'objet `riceCooker` gèrent toujours plusieurs tâches.

7. **Absence de gestion explicite des erreurs :**
   - Le code ne gère toujours pas  explicitement les erreurs.




