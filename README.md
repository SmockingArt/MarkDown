# MarkDown
---
$$Information$$
AUTEUR : [John Gruber](https://fr.wikipedia.org/wiki/John_Gruber) | [Aaron Swartz](https://fr.wikipedia.org/wiki/Aaron_Swartz)

SOURCES: [Obsidian Help](https://help.obsidian.md/Editing+and+formatting/Basic+formatting+syntax) | [Docs.Framasoft.org](https://docs.framasoft.org/fr/grav/markdown.html) 

TAG :  #ProjetMarkDown

THÉMATIQUES : Tutoriel - Aide

Fais par : @SmockingArt
le : 2023-05-16 

---

#   La syntaxe Markdown

Markdown est un langage de balisage léger et portable qui permet d'appliquer des formats à du texte de manière simple. Il permet de se concentrer sur le contenu en utilisant une syntaxe de texte brut qui est facile à écrire et à lire. Il permet également d'insérer des éléments tels que des liens, des images, des niveaux de hiérarchies, des listes, etc.

L'avantage du Markdown est qu'il permet de conserver la simplicité et la portabilité du format texte, sans avoir à se soucier des conversions de fichiers ou de transferts entre différentes plateformes. De plus, il est facilement convertible en HTML pour être publié sur le web.

1.  se **concentrer sur l’écriture** (pas de distraction liée à la mise en forme);
2.  **garder les mains sur le clavier** pour la frappe, mais aussi pour la mise en forme. Certes il existe des raccourcis clavier pour les éléments présentés au-dessus, l’intérêt du langage réside également dans la facilité qu’il offre à _changer_ ces attributs. Par exemple _pour changer le niveau d’un titre, il suffit d’ajouter ou enlever un dièse_;
3.  **une portabilité évidente**: on est sur des fichiers texte à 100%, donc éditable sur toutes les plateformes, et tous types de logiciels, depuis le plus simple Bloc Note Windows ou TextEdit sur Mac.

## Styles de texte


Vous pouvez utiliser `_` ou `*` autour d'un mot pour le mettre en italique. Mettez-en deux pour le mettre en gras.

-   `_italique_` s'affiche ainsi : _italique_
-   `**gras**` s'affiche ainsi : **gras**
-   `**_gras-italique_**` s'affiche ainsi : **_gras-italique_**
-   `~~barré~~` s'affiche ainsi : ~~barré~~
- `==Highlighting==`  ==Highlighting==
-  `%%` %%s'affiche pas en lecture%%
 - `$this will also be grass$` $this will also be grass$
 - `$$text millieux page$$` $$texte$$

## Blocs de code

Créez un bloc de code en indentant chaque ligne avec quatre espaces, ou en mettant trois accents graves sur la ligne au dessus et en dessous de votre code. Exemple :

` ```bloc de code``` ` 

s'affiche ainsi :

```
bloc de code
```

## Liens

Créez un lien intégré en mettant le texte désiré entre crochets et le lien associé entre parenthèses.

`Aidez-vous avec [la documentation de Framasite](https://docs.framasoft.org/fr/grav/) !`

s'affichera :

Vous pouvez ajouter aux liens des attributs `id` et `class` de cette manière :

```
[la documentation de Framasite](https://docs.framasoft.org/fr/grav/){#id .class1 .class2}
```

## Images

Utilisez une image en ligne en copiant son adresse (finissant par `.jpg`, `.png`, `.gif` etc…) avec un texte alternatif entre crochets (qui sera affiché si l'image n'apparaît pas) et le lien entre parenthèses. Vous pouvez aussi ajouter un texte qui apparaîtra au survol de la souris grâce aux `"`.

```
![le logo de Framasoft](https://framasoft.org/nav/img/logo.png)
```

On peut ajouter un texte au survol :

```
![Le logo de Framasoft](https://framasoft.org/nav/img/logo.png "Un bien beau logo !")
```

Redimensionnement des images, exemple de l'image ci-dessus redimensionnée à 100 pixels de large :

```md
![Engelbart|100](https://history-computer.com/ModernComputer/Basis/images/Engelbart.jpg)
```

Ou pour une images local

```md
![[og-image.png|200]]
```

