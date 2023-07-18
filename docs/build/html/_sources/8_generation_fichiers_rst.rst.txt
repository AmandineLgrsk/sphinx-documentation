8. Génération des fichiers rst
==============================

Pour **générer les fichiers .rst correspondant à votre code Python**, 
vous pouvez utiliser la commande ``sphinx-apidoc`` dans votre terminal. 
Assurez-vous de vous placer à la racine de votre projet avant d'exécuter la commande.

La commande ``sphinx-apidoc`` a la syntaxe suivante : 

.. code-block:: console

	$ sphinx-apidoc -o [chemin_output] [chemin_code_source]

Voici comment vous pouvez l'utiliser pour le projet ``demo-sphinx`` :

.. code-block:: console

	$ sphinx-apidoc -o ./docs/source/ ./python/

*[chemin_output]* représente le chemin où vous souhaitez **stocker les fichiers .rst générés**. 
Dans notre exemple, on utilise *./docs/sources/* pour stocker les fichiers .rst dans le 
dossier *source* de notre dossier de documentation *docs*.

*[chemin_code_source]* indique le **chemin où se trouvent les codes Python de votre projet**. 
Dans notre exemple, le code source se trouve dans le dossier *python*.

Après avoir exécuté la commande, Sphinx générera automatiquement les fichiers .rst correspondant
à votre code Python dans le dossier spécifié.

.. figure:: ./images/10_generation_fichiers_rst.PNG
	:align: center

	Génération des fichiers rst

Vous êtes maintenant prêt à passer aux étapes suivantes pour configurer le fichier ``index.rst``
et générer la documentation finale.
