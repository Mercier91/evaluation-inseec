# Évaluation individuelle

## Programmation - Coaching

```
Nom : Mercier
Prénom : Thomas
URL de votre compte Github : https://github.com/Mercier91
```

## Déroulé et fonctionnement. 

L'évaluation est à faire sur [Typora](https://typora.io/). Les réponses sont à écrire dans les blocks de code. 
Pour la partie Ruby, testez votre code sur [repl.it](https://repl.it/) et copiez le dans les blocks de code prévu à cet effet. 
Une fois fini, pushez votre feuille sur Github, dans un nouveau repository que vous appelerez "evaluation-inseec".
L'évaluation est individuelle et durera 1h30. Elle intègre des notions d'HTML, CSS, Ruby et computer science. 

![alt](https://media.giphy.com/media/26xBBfd0ii1khakpy/giphy.gif)

## Quelques mises en garde.

Je connais très bien ce merveilleux site qu'est Wikipédia. Je vous saurais gré de ne pas me remplir certaines questions avec les définitions de Wikipédia. Accessoirement, je sais aussi faire une recherche Google. Si j'ai un doute, je n'hésiterais pas rechercher "Qu'est-ce qu'une API" et comparer les définitions en tête de recherche avec les votre. Si je trouve une similarité trop grande et que je doute de votre bonne foi, je n'hésiterais pas à mettre 0 à la question. 
Pareil pour la copie sur les voisins. Si c'est trop gros et que j'ai un doute trop prononcé... 🔫

![alt](https://media.giphy.com/media/BtedgmzGNCiuk/giphy.gif)



------

### 1. Avec vos mots, expliquez l'interaction client-serveur

L'interaction client serveur est l'intéraction entre le client : la personne qui programme un code afin de l'afficher sur un page web ou effectuer une tache et le serveur qui lui attend les données du client pour les affichers ou executer la tache. Le client envoi les requêtes et le serveur les recoit. 



 ### 2. HTML est un langage côté... 

```
client 
```



### 3. Donnez-moi la structure de base d'une feuille HTML

```html
<!DOCTYPE html>
<!-- Completez après cette ligne -->
<!DOCTYPE html>
<html>
<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>

</body>
</html>
```



### 4. Changez la couleur du texte "J'adore la programmation" en rose en utilisant du CSS.

```html
<div>
   <p>J'adore la programmation</p>
</div>
```

```css
/* Ecrire le code CSS sous cette ligne */
<p style="color:pink;">J'adore la programmation</p>

```



### 5. Qu'est-ce que Bootstrap ?

```
C'est un framework
```



### 6. Reprenez votre code de la question 3 et ajoutez Bootstrap à votre feuille HTML, au bon endroit.

```html
<!DOCTYPE html>
<html>
<head>
    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css" integrity="sha384-MCw98/SFnGE8fJT3GXwEOngsV7Zt27NXFoaoApmYm81iuXoPkFOJwJ8ERdknLPMO" crossorigin="anonymous">
    </head>
<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>

</body>
</html>

```



### 7. Mettez ces trois divs sur le même plan horizontal avec trois colonnes de même taille.

```html
html : 
<div id="gauche">Google</div>
<div id="droite">Microsoft</div>
<div id="centre">Apple</div>
css :
#gauche {float:left; width:value;}
#droite {float:right; width:value;}
#centre {margin-right: value; /* largeur de la colonne droite */ margin-left: value; /* largeur de la colonne gauche */}
```



### 8. Avec le même code, changez le texte par le logo de la marque en question

```html
html : 
<div id="gauche">href="https://i1.wp.com/www.grapheine.com/wp-content/uploads/2015/09/nouveau-logo-google.gif?fit=1950%2C1200&quality=90&strip=all&ssl=1"</div>
<div id="droite">href="https://static.latribune.fr/full_width/106415/logo-microsoft.jpg"</div>
<div id="centre">"https://upload.wikimedia.org/wikipedia/commons/thumb/7/70/Logo_Apple.inc.gif/220px-Logo_Apple.inc.gif"</div>
css :
#gauche {float:left; width:value;}
#droite {float:right; width:value;}
#centre {margin-right: value; /* largeur de la colonne droite */ margin-left: value; /* largeur de la colonne gauche */}
```

 

### 9. Toujours sur le même bout de code, rendez les logos cliquables. Quand on clique sur le logo, on doit arriver sur le site officiel de la marque.

```html
<div>
    Google
</div>

<div>
    Microsoft
</div>

<div>
    Apple
</div>
```

![Mon gars sûr !](https://media.giphy.com/media/l0K4mbH4lKBhAPFU4/giphy.gif)

### 10. Parlons Ruby. Ruby est un langage côté...

```
serveur et client 
```



### 11. Listez-moi tous les types de données que vous connaissez.

```
Les chaines de caractères x="y", les itérateurs each, les opérateurs * == **, les valeurs numeriques, les conditions (if,else,elsif), nombres decimaux float, interpollation, concaténation, des variables
```



### 12. Assignez à des variables votre prénom, nom et le lien de votre compte Github puis affichez chacune des variables. En 6 lignes.

```ruby
first_name= "Thomas"
puts first_name

name= "Mercier"
puts name

github_account= "https://github.com/Mercier91"
puts github_account 

```



### 13. Assignez 674 et 311 à des variables `a` et `b` et stockez le résultat `a` modulo `b` dans une variable `c` et affichez la. 

```ruby

# Le résultat attendu est 52. 
a= 674
b= 311
c= a%b
print c
```



### 14. Qu'est-ce qu'une gem ? 

```texte
Une gem est un peu comme une bibliotèque. 
On installe une gem dans notre code ruby et il ira cherche les informations dont il a besoin dedans. 
```



### 15. Qu'est-ce qu'une API et qu'est-ce qui nous permet de nous y connecter ?

```
 Application Programming Interface : c'est une interface pour les applications. Nos clefs secrètes :
 - config.consumer_key
 - config.consumer_secret
 - config.access_token
 - config.access_token_secret
 
```



### 14. On va créer un script pour dire bonjour ou bonsoir, en fonction de l'heure de la journée. Votre script doit demander à l'utilisateur de rentrer son prénom. Si `hour` est inférieur à 12, lui dire `Bonjour Anthony` sinon `Bonsoir Anthony` (évidemment, le prénom doit être celui renseigné par l'utilisateur).

```Ruby
# <- Demander le prénom de l'utilisateur
first_name=""gets.chomp

hour = 15

# Si hour est inférieur à 12
	# j'écris mon code permettant de dire Bonjour prénom
elsif
    hour>12
    print "Bonjour Anthony"
if 
    hour<12 
    print "Bonsoir Anthony"
end


# sinon
	# j'écris mon code permettant de dire Bonsoir prénom

```



### 15. Itérer sur l'array contenant des noms de twitos un peu famous et follow chacun d'eux grâce à une méthode trouvée dans la [doc de la gem twitter](https://github.com/sferik/twitter). Pas besoin de lancer le code et de faire la partie authentification. Juste le bloc d'itération suffira. 

```ruby
handles = ["@richardbranson", "@jeffweiner", "@LinkedInQueen", "@ericschmidt", "@elonmusk", "@petecashmore", "@SteveForbesCEO", "@mtbarra"]
client.follow(richardbranson)
client.follow(jeffweiner)
client.follow(LinkedInQuenn)
client.follow(ericschmidt)
client.follow(elonmusk)
client.follow(petecashmore)
client.follow(SteveForbesCEO)
client.follow(mtbarra)

Il faut normalement utilisé each mais je sais plus du tout comment 


```



### 16. Félicitations, vous êtes arrivé·e à la fin, pushez cette feuille sur votre Github dans un repo appelé `evaluation-inseec`. N'oubliez pas de remplir le premier block avec votre identité tout en haut ! 

![alt](https://media.giphy.com/media/l0MYJnJQ4EiYLxvQ4/giphy.gif)

