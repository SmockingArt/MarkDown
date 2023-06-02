# MarkDown
---
$$Information$$
AUTEUR : [John Gruber](https://fr.wikipedia.org/wiki/John_Gruber) | [Aaron Swartz](https://fr.wikipedia.org/wiki/Aaron_Swartz)

SOURCES: [Obsidian Help](https://help.obsidian.md/Editing+and+formatting/Basic+formatting+syntax) | [Docs.Framasoft.org](https://docs.framasoft.org/fr/grav/markdown.html) 

TAG :  #ProjetMarkDown

THÉMATIQUES : Tutoriel - Aide

✍ Fais par : @SmockingArt 

🧭 le : 2023-05-16 

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

## Citation

Les citations se font avec le signe `>` :

```
> Oh la belle prise !
```

> Oh la belle prise !

### Callouts

Utilisez la syntaxe suivante pour désigner un bloc d'appel: `> [!INFO]`.

Pour en savoir plus sur les callouts [here](https://help.obsidian.md/How+to/Use+callouts).

```markdown
> [!INFO]
> Here's a callout block.
> It supports **markdown** and [[Internal links|wikilinks]].
```

> [!INFO]
> Here's a callout block.
> It supports **markdown** and [[Internal links|wikilinks]].

#### Foldable callouts

Vous pouvez rendre un appel pliable en ajoutant un plus (+) ou un moins (-) directement après l'identifiant du type.

```
> [!faq]- Are callouts foldable?
> Yes! In a foldable callout, the contents are hidden when the callout is collapsed.
```


> [!faq]- Are callouts foldable?
> Yes! In a foldable callout, the contents are hidden when the callout is collapsed.

#### Nested callouts

```
> [!question] Can callouts be nested?
> > [!todo] Yes!, they can.
> > > [!example]  You can even use multiple layers of nesting.
```


> [!question] Can callouts be nested? 
> > > [!todo] Yes!, they can.
> > >  > > > [!example] You can even use multiple layers of nesting.


> [!question] Can callouts be nested?

> [!todo] Yes!, they can.

> [!example] You can even use multiple layers of nesting.

## Listes

Vous pouvez créer des listes avec les caractères `*` et `-` pour des listes non ordonnées ou avec des nombres pour des listes ordonnées.

Une liste non ordonnée :

```
* une élément
* un autre
 * un sous élément
 * un autre sous élément
* un dernier élément
```

-   une élément
-   un autre
    -   un sous élément
    -   un autre sous élément
-   un dernier élément

Une liste ordonnée :

```
1. élément un
2. élément deux
	1. un sous élément
	2. un autre sous élément 
```

1.  élément un
2.  élément deux
	1. un sous élément
	2. un autre sous élément 

```md
- Item 1

- Item 2
- Item 3
```

-   Item 1
    
-   Item 2
    
-   Item 3

### Task list

```md
- [x] #tags, [links](), **formatting** supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [?] this is also a complete item (works with every character)
- [ ] this is an incomplete item
- [ ] tasks can be clicked in Preview to be checked off
```

-   [#tags](https://publish.obsidian.md/#tags), [links](https://publish.obsidian.md/), **formatting** supported
-   list syntax required (any unordered or ordered list supported)
-   this is a complete item
- [?]  this is also a complete item (works with every character)
- [ ] this is an incomplete item
- [ ] tasks can be clicked in Preview to be checked off
- [ ] 

```
bloc de code
```

## Titres

Pour faire un titre, vous devez mettre un `#` devant la ligne. Pour faire un titre plus petit, ajoutez un `#`  :

```
# Un grand titre
## Un titre un peu moins grand
### Un titre encore moins grand
...
...
###### Le plus petit titre
```

Vous pouvez également souligner le texte en utilisant `===` ou `---` pour créer des titres.

```
Un grand titre
=============
```
Graph View

Filtrer avec un mot clé ou avec un hastag.

Colorer des recherches pré-enregistrées

Jouer avec les forces de liens :

-   Central force : 0
-   Repulsion : 70%
-   Links : 100%
-   Distance : 0

> MÉTHODE IMPORTANTE : utiliser le Graph View surtout pour repérer les notes solitaires dans les limbes et non-raccrochées à quoi que ce soit.

