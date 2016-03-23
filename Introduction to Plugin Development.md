# Introduction au développement de plugin

Bienvenue dans le manuel du développeur de plugin. Que ce soit votre prermier ou
votre cinquantième plugins, nous espérons que ces ressources vous aideront à
écrire le meilleur plugin possible.

Le guide du développeur de plugin couvre un grand nombre de sujets - depuis les
en-têtes de plugin, aux meilleurs pratiques de sécurité, les outils que vous
pouvez utiliser pour construire votre plugin. Il s'agit également d'un guide
en constante évolution - si trouvez une erreur ou des informations manquantes,
n'hésitez pas à éditer et le rendre meilleur.

Il a 3 composants principaux dans WordPress:
- Le Coeur (Core)
- Les Themes
- Les Extensions (plugins)

Ce manuel concerne les plugins et décrit l'interaction de ceux-ci avec WordPress.
Cela vous aidera de comprendre comment ils fonctoinent et comment créer votre
propre plugin.

## Pourquoi nous créons des plugins

Il y a une règle majeure dans le développement WordPress qui est: **Ne touchez
pas au coeur de WordPress (WordPress Core)**. Ce qui veut dire qu'il ne faut pas
modifier le coeur de WordPress pour ajouter des fonctionnalités à votre site.
C'est ainsi, car lors d'une mise à jour de WordPress vers une nouvelle version,
les fichiers sont écrasés. Toutes fonctionnalités que vous voulez ajouter doit
passer par un ou des plugins qui utilisent l'API WordPress officiel.

Les plugins WordPress peuvent être simple ou aussi complexe que vous le souhaitez,
en fonction de vos besoins. Le plugin le plus simple est un fichier PHP.
Le plugin [Hello Dolly][0] est un exemple d'un tel plugin.
Le fichier Php du plugin nécessite une en-tête de plugin, quelques fonctions PHP
et quelques crochets (hooks) auquel attacher vos fonctions.

[0]: https://wordpress.org/plugins/hello-dolly/

Les plugins vous permettrons d'étendre les fonctionnalités WordPress sans avoir
à toucher au coeur de WordPress lui-même.
