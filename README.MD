Generalitat de Catalunya
CFGS Desenvolupament d'Aplicacions
Departament d'Educació
Web
Institut Almatà
Utilització de Git i Github
M6 – Pràctica EAF
L’objectiu d’aquesta activitat és conèixer i practicar les diferents ordres i instruccions de Git i
Github vistes a classe, aplicant-los a un exemple de construcció pàgina Web.
Notes prèvies:
-
TOTES LES INSTRUCCIONS S'HAN DE REALITZAR DES DE TERMINAL,
EXCEPTE LES RELATIVES A MARKDOWN I LES FETES EN GITHUB.COM EN EL
REPOSITORI REMOT.
-
Seria recomanable que feu una carpeta imagesDocument amb totes les captures de
pantalla que considereu adients per documentar la pràctica. Així us serà més fàcil
treballar amb MarkDown.
-
Es recomana instal.lar ( si no els teniu ja) en Atom els plugins: linter-markdown,
Language-markdown i markdown-preview per treballar amb Mardown.
1 – Creació d’una pàgina Web utilitzant eines Git i Github
1. Creo un directori de treball anomenat /DiariVostreNom/ en el directori de l'usuari.
2. Inicialitzar el repositori buit.
3. Crear l'arxiu index.html
4. Afegir l'estructura bàsica
<!DOCTYPE HTML>
<html>
<head>
</head>
<body>
</body>
</html>
5. Crear un commit indicant que es crea l'esquelet bàsic del index.html
6. Afegir el contingut al head, entre <head> i </head>.
<meta charset="UTF-8" />
<title></title>
<link rel="stylesheet" type="text/css" href="style.css" />
<!--[if IE]>
<script src="http://html5shiv.googlecode.com/svn/trunk/html5.js"></script>
<![endif]-->
7. Crear un commit indicant que s'afegeix la capçalera del index.html
8. Afegir el contingut al body, entre <body> i </body>
<header>
<h1>Diari de Vostre Nom</h1>
</header>
<aside>
<p></p>
</aside>
<section>
</section>
<footer>
<p>&copy; 2012 - dissenyat per <a href="http://www.ciclesbalaguer.com" title="DiariVostre-
Nom">VostreNom</a></p>
</footer>
9. Crear un commit indicant que s'afegeix l'estructura bàsica del body.
10. Crear un repositori en GitHub que s’anomeni RemoteDiariVostreNom (exemple RemoteDia-
riEduardo)
11. Assignar al vostre repostiorio global el remot
Executar:
1. git remote
2. git remote add origin https://VOSTRE-REPOSITORI.git
3. git remote -v
4. Pujar amb un push tota el que heu fet a la branca master del remot.
Executar:
12.
1. git push -o origin --all
2. Veure Github
3. git push -o origin --tags
4. Veure Github
Afegir el contingut de section, entre <section> i </section> ( la idea és afegir al menys tres
posts en la zona d’articles del vostre document). Podeu afegir notícies, articles etc...
<article>
<header>
<h2>Post 3</h2>
</header>
<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sigueu do eiusmod tempor inc
didunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco
laboris nisi ut aliquip exea commodo consequat. Duis aute irure dolor in reprehenderit in vo-luptate
velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat senar proident, sunt
in culpa qui officia deserunt mollit anim aneu est laborum.</p>
</article>
<article>
<header>
<h2>Post 2</h2>
</header>
<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sigueu do eiusmod tempor inci-
didunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco
laboris nisi ut aliquip exea commodo consequat. Duis aute irure dolor in reprehenderit in vo-luptate
velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat senar proident, sunt
in culpa qui officia deserunt mollit anim aneu est laborum.</p>
</article>
<article>
<header>
<h2>Post 1</h2>
</header>
<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sigueu do eiusmod tempor inci-
didunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco
laboris nisi ut aliquip exea commodo consequat. Duis aute irure dolor in reprehenderit in vo-luptate
velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat senar proident, sunt
in culpa qui officia deserunt mollit anim aneu est laborum.</p>
</article>
13. Crear un commit indicant que s'afegeix tota l'estructura de la zona de posts.
14. Crear un arxiu style.css.
15. Afegir la següent informació.
html {
margin: 0;
padding: 0;
}
body {
width: 940px;
margin: 0 acte;
font: 10pt/1.5em Helvetica,"Helvetica neue", Arial, sans-serif;
}
16. Crear un commit indicant que s'afegeixen les CSS d'html i de body.
17. Afegir la següent informació.
header,section,article,aside,footer{
display: block;
}
aside {
float: left; width: 470px;
min-height: 480px;
background: url(logo.png) center top no-repeat;
margin: 0 0 20px 0;
}
18.
Crear un commit indicant que s'afegeixen les CSS de diversos elements HTML5: header,
section, article, aside i footer.
19.
Afegir en el directori arrel de projecte el logotip que apareixerà en la barra lateral esquerra:
logo.png ( podeu ficar la imatge que vulgueu)
20. Crear un commit indicant que s'afegeix el logotip del Vostre Diari.
21. Afegir la següent informació.
section {
float: right; width: 428px;
padding-left: 20px; margin: 0 0 20px 0px;
//border-left: 1px dotted #000;
}
section h2 {
font: 14pt Helvetica,"Helvetica neue", Arial, sans-serif;
font-weight: lighter;
text-transform: uppercase;
color: #493831;
padding-bottom: 10px;
margin: 0;
}
22. Crear un commit indicant que s'afegeixen les CSS de section.
23. Afegir la següent informació.
footer{
clear:both !important;
width:940px;
height: 100px;
padding: 10px;
color:#200f08 ;
//border-top: 1px dotted #000;
background:#fff;
}
24. Crear un commit indicant que s'afegeixen les CSS del footer.
25. Afegir la següent informació.
h1 {
font: 32pt Helvetica,"Helvetica neue", Arial, sans-serif;
text-align: center;
text-transform: uppercase;
color: #000;
padding-top: 30px ;
text-shadow: 1px 1px 2px #fff;
}
a:hover {
border-bottom:1px dotted #d2543c;
}
a img {
border:none;
}
26. Crear un commit indicant que s'afegeixen les CSS de l'H1 i dels enllaços.
27. Actualitzar la pàgina remota de forma regular fent amb l'ordre push.
git push [nom-remot][nomeni-branca] ( és possible que tingueu que pujar mes d'una
branca en algun moment de la practica)
28. Crear una etiqueta de v1.0
29. Crear una branca “develop”.
30. En aquesta branca de desenvolupament anem a realitzar diverses tasques:
31. Crear un directori de images i moure allí el logotip logo.png.
32. Crear un commit indicant que es mou el logotip a la carpeta images.
33. Crear un directori de CSS i moure allí les CSS style.css.
34. Crear un commit indicant que es mou la CSS a la carpeta CSS.
35. Canviar les referències a la CSS en el index.htm i al logotip logo.png en la CSS.
36. Crear un commit indicant que es canvien les referències a les CSS i a les imatges al reorga-
nitzar-les en directoris.
37. Actualitzar la pàgina remota de forma regular fent amb l'ordre push.
38. Anar al vostre repositori en Github.com i comprovar que ho teniu idèntic al vostre repositori
local.
A GITHUB.COM:
39. Crear una branca “bugfix” a partir de la “master” per resoldre una sèrie de modificacions.
40. Treure els comentaris en les CSS de les dues vores (comencen per //border ).
41. Crear un commit indicant que introdueixen les vores en la barra dreta i en el footer.
42. Introduir com a títol “Diari de Vostre Nom”.
43. Crear un commit indicant que s'introdueix el títol a la pàgina.
44. Canviar 2012 per 2018 en el footer. Treure (c).
45. Crear un commit indicant que es realitzen petits ajustos en el footer.
46. Crear una etiqueta de v1.1
47. Portar aquests canvis a la branca “master” ( realitzar un merge).
48. Esborrar la branca “bugfix”.
49. Portar els canvis de la branca “develop” a la branca “master”. Resoldre els conflictes, si hi
hagués.
50. Crear una etiqueta de v1.2
51. Afegir fitxer DOCUMENT.MD amb tota la pràctica, captura de pantalla, explicacions
etc...També en Markdown. ( en github). Podeu triar entre elaborar-lo en local i pujar-
ho a github ( ex: drag and drop) o treballar directament en l'editor de Github.
52.
Activar la utilització de gh-pages i l'adreça de la pàgina web que es mostrés: recordar que
serà del tipus https://username.github.io/Diariremotoeduardo.
53.
Afegir un document Readme.md escrit en Markdown, amb el vostre nom, curs i nom- prac-
tica “Practica Diari Vostre Nom” i enllaç a la vostra pàgina generada anteriorment.
54.
Lliurar l'adreça web del vostre master ( repositori). Heu de tenir tots els elements i la pagina
s'ha de visualitzar de forma correcta, en particular la carpeta CSS amb el css creat i la carpeta
imatges.
AL REPOSITORI LOCAL :
55.
Actualitzar-ho amb els commits i canvis fets en el repositori remot ( fent possiblement git
fetch i git pull
EN AQUEST PUNT HAURIES DE TENIR EL MATEIX
EN LOCAL QUE EN REMOT :
56.
Actualitzar DOCUMENT.MD amb els últims canvis, fer commit corresponent i actualitzar
repositori remot.
EN AQUEST PUNT HAURIES DE TENIR EL MATEIX
EN LOCAL QUE EN REMOT :
2 – Fork d’una pàgina Web utilitzant eines Git i Github
Vegeu el següent vídeo com explica com es pot col·laborar en diferents projectes de software
lliure o fer canvis en repositori de forma general.
https://www.youtube.com/watch?v=_NrSWLQsDL4&list=PLRqwX-
V7Uu6ZF9C0YMKuns9sLDzK6zoiV&index=3
Feu el mateix però agafeu com referència: https://github.com/ejgutierrez74/Billiards, feu un
fork ( això crearà una còpia del repositori en el vostre compte: tipus github.com/username/Billiards)
hi aneu al fitxer Billiards/src/Billiards.cpp i feu alguna modificació ( ex: canviar el text que fica a
cout). Feu un pull request a l’original. Us aprovaré el canvi o el denegaré.
3 – Clonar un repositori
Cloenu el projecte: https://github.com/ejgutierrez74/individual i ho descarregeu a una carpeta
local. Vegeu els remotes que té. Feu una inspecció amb git log dels commits i historial del projecte.
Feu alguna modificació al poema i un commit. NO el torneu a pujar ni res. Els canvis han de restar
al vostre repositori local.
Consells i ajudes:
•
Es valorarà si s'afegeixen elements, com a més articles, es millora la web etc....L'element tag
no és obligatori perquè no hem donat en classe, però puja nota.
•
Es recomana afegir més commits i push de forma regular, per mantenir tant el repositori local
com global.
•
Vigileu i utilitzeu:
• git branch i checkout per saber on sou en cada moment ( en quina branca)
• git log i git status ( veure que heu modificat i historial de commits fets)
• Instruccions útils: git remote show i git remote show [ nom branca]
• If you want to push all branches at once:
git push <URL> --all
To push all the tags:
git push <URL> --tags

