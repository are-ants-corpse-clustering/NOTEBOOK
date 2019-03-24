# NOTEBOOK
Contient notre compte-rendu sous forme de notebook Jupyter.

## Notre projet :

<p align="justify">
Dans le cadre de notre ARE, nous avons decidé de travailler sur l'étude comportementale des fourmis. En effet, nous allons étudier un phénomène naturel observable dans la nature: les fourmis agrègent leur morts en vastes tas de maniére regulière dans l'espace. Au fur et à mesure du temps, elles finissent par ne former qu'un seul et unique tas. Ce phénomène est observable à l'intérieur ou à l'extérieur des fourmilières (dans le cas des fourmilières, une pièce de la fourmilière est spécialement dédiée au rassemblement des cadavres de fourmis).
</p>

<br/>

![Image](https://www.researchgate.net/profile/Guy_Theraulaz/publication/6780365/figure/fig3/AS:394664680149009@1471106800860/Spatio-temporal-dynamics-Typical-spatio-temporal-dynamics-of-corpse-clustering-by-ants.png)<br/>
<p align="center"> Exemple de formation de tas de cadavres par des fourmis (vue de dessus).</p>

<p align="justify">
Notre but sera donc d'implémenter différents modèles afin d'aboutir, dans un premier tas, à la formation de tas individuels séparés, puis à la formation d'un seul et unique tas similaire à celui que l'on peut observer dans la réalité (on le considèrera comme l'état final de notre système). Nous discuterons donc la pertinence de chaque modèle en dégageant clairement leurs avantages et leurs inconvénients et en proposant des solutions afin de les améliorer lorsque cela est réalisable.</p> 
</p>

## Avancement du projet :

## 23/05/2019:
<p align="justify">
Nous avons implémenté deux modèles différents : une première approche simple et un modèle mise au point par un scientifique français nommé Deneubourg en 1991. Au cours de l'implémentation de ces deux modèles, nous avons rencontré divers problèmes liés au déplacement des fourmis et à l'affichage graphique de Tkinter.
</p>

### Modèle de Deneubourg :
<p align="justify"> Les problèmes liés au déplacement et à la disparition des fourmis sur la fenêtre graphique a été réglé à ce jour pour ce modèle. Cela était dû à une mauvaise utilisation des coordonnées dans Tkinter et à une condition manquante dans la boucle de la fonction next_generation. Le modèle semble fonctionner correctement pour former des tas de fourmis individuels mais nous avons du mal à obtenir un seul et unique tas (peut-être n'attendons nous pas assez longtemps). Nous prévoyons de remédier à remedier à ce problème rapidement.

### Première approche :
<p align="justify"> Les problèmes liés au déplacement et à la disparition des fourmis n'a pas encore été résolu pour ce modèle. En effet, l'implémentation du modèle de Deneubourg étant plus complexe, nous avons préféré concentrer nos efforts sur ce dernier afin d'en résoudre les différents problèmes. Cela étant fait, les problèmes étant similaires sur les deux modèles nous pensons être capable de les résoudre rapidement.</p>

<p align="justify"> Nous prévoyons également de comparer les différents modèles quant à leur pertinence (nottamment en comparant leur efficacité , leur rapidité, etc.) à l'aide de graphiques et d'animation. Mais aussi d'implémenter d'autres modèles ou de modifier les modèles déjà implémenté afin de les améliorer afin de pallier à certains de leur inconvénients ou d'aboutir à une approche plus efficace. </p>

### Aperçu du fonctionnement de notre implémentation du modèle de Deneubourg

![Deneubourg0](https://user-images.githubusercontent.com/47559664/54881002-9c1a6500-4e4b-11e9-9e10-fb232ff9d672.png)
<p>Etat initial (les fourmis vertes sont vivantes, les noires sont mortes).</p>

![Deneubourg15](https://user-images.githubusercontent.com/47559664/54881003-9c1a6500-4e4b-11e9-98f4-abe4d10c121c.png)
<p>Après 15 mins.</p>

![Deneubourg](https://user-images.githubusercontent.com/47559664/54881001-9c1a6500-4e4b-11e9-9692-35f94c037291.png)
<p>Après 45 mins.</p>

## Travail restant à faire :

- Résoudre les problèmes liés au déplacement des fourmis dans notre première approche.
- Réussir à aboutir à un tas final avec notre modèle de Deneubourg (peut-être est-ce seulement lié à la taille de la fenêtre?).
- Implémenter ou modifier les modèles déjà existant pour répondre plus efficacement au problème, corriger certains de leur défauts ou rajouter des facteurs (maladies,etc.).
- Comparer les différents modèles et conclure quant à leur pertinence.
