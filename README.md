# Exercice d'accessibilité des contenus

## Équipe 
Travailler à 2 ou maximum 3. Chacun versionne individuellement mais les réponses et le code peuvent être identiques.
- Cassiopée Gariépy
- Coralie Beauvais

## Objectifs
- Expérimenter le versionnage de fichiers avec GIT
- Acquérir des compétences en accessibilité des contenus

## Prérequis
- Avoir lu et pris connaissance des notes du cours 
- Avoir installé l'outil CCA (colour-contrast-analyzer)
- Avoir un compte GitHub
- Avoir installé et configurer GIT sur votre ordinateur

## Instructions

### 0. 
- Initialiser un dépôt GIT dans le dossier du projet
- Créer un fichier `index.html` et un fichier `style.css`

### 1.	Donner une alternative textuelle aux images

#### 1.1 Baliser dans le fichier `index.html` les images du dossier `1-textes-alternatifs` 

Pour vous guider dans le choix des balises, des attributs et des valeurs d'attributs, utiliser l'arbre de décision et référez-vous aux notes de cours.

#### 1.2 Évaluer la pertinence des contenus textuels alternatifs

Pour chacune des pages ci-dessous:
* __Utiliser la barre d'outil de développement pour inspecter les images__ et juger de la qualité des attributs *alt*. __Prendre une capture-écran et la joindre ci-dessous.__
*  __Les textes alternatifs sont-ils adéquats ?__ Commenter votre observation. Pourrait-on faire mieux ? Donnez un exemple de ce que vous proposeriez.

##### Le soleil
- https://www.lesoleil.com/  
![Image du Soleil montrant le alt des images](/images/CapturesImages/img1.png)
Je crois qu'il y a deux problèmes sur la page d'accueil. Premièrement, le logo principal en haut de la page n'a aucun alt, alors qu'il sagit du bouton pour aller à la page principale.
Deuxièment, le bouton pour accéder à son profil n'a aucun alt, alors que aucun texte n'est présent pour l'indiquer. 

- https://www.lesoleil.com/  
![Image du Soleil montrant le alt des images](/images/CapturesImages/img2.png)
Ici, le texte alternatif est déja présent en dessous, il y a donc une rédondance de l'information. Je crois qu'il aurais été mieux de ne rien mettre dans le alt.  

### 2. Structurer avec les h1-h6 une table des matières

#### 2.1 Vérifier la structure

D’après les captures-écrans que vous trouverez dans le dossier __images/2-table-des-matieres_h1-h6/2-1/__, est-ce que la table des matières du document est correcte?  

Sinon, expliquez le problème en vous basant sur les règles de base énoncées dans les notes de cours. 

__Tutoriel sur les formulaires du w3c__  
[Article](images/2-table-des-matieres_h1-h6/2-1/tuto-form-w3c.pdf)  
[Table des matières (outline)](images/2-table-des-matieres_h1-h6/2-1/tuto-form-w3c-outline.png) 

Réponse : 

Ici, la table des matières était très bien, avec un h1 présent, puis 3 h2 bien structurés. 

__L’affaire Savtchenko__ 
[Article](images/2-table-des-matieres_h1-h6/2-1/article-savtchenko.pdf)  
[Table des matières (outline)](images/2-table-des-matieres_h1-h6/2-1/article-savtchenko-outline.png) 
  
Réponse : 

Dans cette exemple, je crois qu'il y a quelques erreurs. Premièrement, il manque un premier H1, mais ce problème est surtout causé par l'assignation de H2 au élément de Navigation, ce qui ne semble pas optimal. 

Ensuite, le h2 pour l'élément sous l'image me semble une mauvaise idée, car c'est plus un paragraphe/caption qu'un titre. 


#### 2.2 S'exercer à bien structurer

- Ouvrir la capture-écran [concevoir-un-design-sans-la-couleur](images/2-table-des-matieres_h1-h6/2-2/concevoir-un-design-sans-la-couleur.pdf) dans le logiciel PhotoShop.  
- Ajouter un calque de blanc à 50% de transparence
- Dans un 3e calque, par-dessus, identifiez les titres et leurs niveaux (h1-h6) de manière voyante (couleur rouge et font-size suffisant)
- Sauvegarder au format .png dans le même dossier.
![Image du Soleil montrant le alt des images](/images/CapturesImages/resultat.png)

### 3. Baliser un tableau de données pour qu’il soit accessible

D’après la capture-écran et le texte fourni dans le dossier [3-tableau-de-donnees](images/3-tableau-de-donnees), balisez de manière accessible ce tableau de données.  
  
Votre tableau de données doit comporter un titre (caption) : 

> "Recommandations de consommation de poissons selon l’âge, le sexe et la condition physique".  


Les __entêtes de rangées et de colonnes__ doivent être balisées comme des `<th>` plutôt que des `<td>` et puisque le tableau est *complexe*, vous devez utiliser des attributs `id` dans les `<th>`. 

Chaque cellule `<td>` du tableau doit avoir un attribut headers avec comme valeur(s), le ou les identifiants de ses entêtes de colonnes et de rangées.

Styler le tableau conformément au fichier [consommation-poissons.pdf](images/3-tableau-de-donnees/consommation-poissons.pdf).

#### Ressources
•	balisage accessible d’un tableau (voir les notes du cours)
•	balisage html : https://www.w3schools.com/TAGs/tag_table.asp
•	balisage css de tableau: https://www.w3schools.com/css/css_table.asp

VOIR HTML POUR LE TABLEAU



