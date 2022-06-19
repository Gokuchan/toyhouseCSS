Tuto pour utiliser le template! 
----------

1. Récupérer le code ici (copier / coller à l’étape 3): https://github.com/Gokuchan/toyhouseCSS/blob/main/tpl.html

2. **⚠️IMPORTANT⚠️** sur Toyhouse dans "Edit Character" il faut **DESABLE WYSIWYG**.. et ne jamais le reactiver !

demo:

https://user-images.githubusercontent.com/3582779/174462336-5d61a2c6-12af-4ba0-bc10-a8df372828ec.mov

*❔Pourquoi? Malheureusement, malgré l'aspect pratique du mode WYSIWYG (what you see is what you get), le nom est en fait un mensonge partiel car ce que vous voyiez n'est pas exactement ce que vous aurez :( le code est altéré et certains éléments se "cassent" mais pas de panique... au contraire ça sera plus simple ainsi d’éditer le code! je vous montre juste après ;)*

3. Supprimer le contenu dans la zone de texte et coller le code que vous avez copié:

https://user-images.githubusercontent.com/3582779/174462681-ce482d34-e594-45c7-9741-6b89d49d29d8.mov

Le code est maintenant formaté, coloré et les lignes numéroté, ce qui va rendre l’édition du template plus simple que le bloc informe qui était là auparavant (c'est le WYSIWYG qui etait enable qui causait ça et c'est pourquoi on l'a disable

4. Editer le template en remplaçant le texte [EN MAJUSCULE ENTRE CROCHET UN PEU PARTOUT]

------------------------------------------

Tips
----

Je sais qu'en ne faisant pas de code (ici du HTML) ça peut paraitre intimidant de ne pas avoir accès à l'éditeur de texte normal (malheureusement celui-ci pourrit le code comme je disais)
Du coup voilà des petites astuces / pointeurs que je vais vous donner (vous en connaissez peut eêtre certains mais on va quand même tout lister ici :)

1. **Comment visualier / tester au fur et à mesure?**

Pour voir votre progrès sur le template sans avoir à attendre de tout finir pour le "voir", il suffit de sauvegarder vos changements puis de cliquer sur le nom du personnage pour ouvrir un nouvel onglet à garder à côté de votre onglet "EDIT".
Quand vous voulez voir vos changements, sauvegardez votre avancement et rafraîchissez l'onglet de la fiche perso.

demo:



https://user-images.githubusercontent.com/3582779/174463609-8d571e24-696c-4677-af21-afa54a0ff1ed.mov

------------------------------------------

2. **Les paragraphes**

Les sauts à la ligne ne sont pas automatiques en appuyant sur "Entrée" en HTML du coup on rédige un paragraphe ainsi:
```
<p> Mon paragraphe 1</p>
<p> Mon paragraphe 2</p>
```
qui donne:

Mon paragraphe 1

Mon paragraphe 2

Pour sauter une ligne dans un paragraphe on utilise le tag `<br>` seul. Par exemple:

```
<p>Mon paragraphe <br> saute une ligne</p>
```

------------------------------------------

3. **Les liens**

J'ai déjà créer les tags de liens dans le template et il suffira d'y ajouter les URLs que vous désirez mais pour vous aider à les identifier:

```
<a href="https://google.com">Texte à cliquer aui dirige vers le lien</a>
```
Intégrer une image:

```
<img src="https://une-image.com/image-jolie.jpg" />
```

------------------------------------------

3. **Les Pokémon**

Les icones de Pokémon sont dispo ici -> https://msikma.github.io/pokesprite/overview/dex-gen8.html

Si vous connaissez le nom anglais du Pokémon vous pouvez simplement remplacer le text dans l'URL

demo:

```
<!-- Pokemon image -->
   <img src="https://raw.githubusercontent.com/msikma/pokesprite/master/pokemon-gen8/regular/bulbasaur.png" border="0">
   <!-- Pokemon gender -->
   <p class="gender">[♀ / ♂ + ✧]</p> 
   <!-- Pokemon name -->
   <div class="tooltip-content">
        <p>[PKMN NAME]</p>
   </div> 
```  
devient pour Germignon femelle non shiny:
```
<!-- Pokemon image -->
   <img src="https://raw.githubusercontent.com/msikma/pokesprite/master/pokemon-gen8/regular/chikorita.png" border="0">
   <!-- Pokemon gender -->
   <p class="gender">♀</p> 
   <!-- Pokemon name -->
   <div class="tooltip-content">
        <p>Germignonne</p>
   </div> 
```  
si le Pokémon est shiny la fin de l'URL passe de `/regular/nom-du-pkmn` à `/shiny/nom-du-pkmn`:

```
<img src="https://raw.githubusercontent.com/msikma/pokesprite/master/pokemon-gen8/regular/espeon.png" border="0">
```  

![](https://raw.githubusercontent.com/msikma/pokesprite/master/pokemon-gen8/regular/espeon.png)

```
<img src="https://raw.githubusercontent.com/msikma/pokesprite/master/pokemon-gen8/shiny/espeon.png" border="0">
```  
![](https://raw.githubusercontent.com/msikma/pokesprite/master/pokemon-gen8/shiny/espeon.png)

Pour les Pokémon régionaux `/regular/pkmn-region`, si shiny `/shiny/pkmn-region`:


```
<img src="https://raw.githubusercontent.com/msikma/pokesprite/master/pokemon-gen8/regular/zorua.png" border="0">
```  

![](https://raw.githubusercontent.com/msikma/pokesprite/master/pokemon-gen8/regular/zorua.png)

```
<img src="https://raw.githubusercontent.com/msikma/pokesprite/master/pokemon-gen8/regular/zorua-hisui.png" border="0">
```  
![](https://raw.githubusercontent.com/msikma/pokesprite/master/pokemon-gen8/regular/zorua-hisui.png)
```
<img src="https://raw.githubusercontent.com/msikma/pokesprite/master/pokemon-gen8/shiny/zorua-hisui.png" border="0">
```  
![](https://raw.githubusercontent.com/msikma/pokesprite/master/pokemon-gen8/shiny/zorua-hisui.png)


Cette base de données de malade a aussi tous les sprites de tous les objets de tous les jeux existants: https://msikma.github.io/pokesprite/overview/inventory.html (si jamais vous voulez utiliser dans l'espace "Gardiens" (Goku a la plume de Lugia, mais Hika tu peux utiliser la Gracidée ![](https://raw.githubusercontent.com/msikma/pokesprite/master/items/key-item/gracidea.png), Bibi, ce charm ressemble a un bijou d'aura: ![](https://raw.githubusercontent.com/msikma/pokesprite/master/items/key-item/shiny-charm.png) ou l'orbe adamant ![](https://raw.githubusercontent.com/msikma/pokesprite/master/items/hold-item/adamant-orb.png)
