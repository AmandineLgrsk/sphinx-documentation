9. Modification du fichier index.rst
====================================

Dans le fichier ``index.rst``, vous devez modifiez la directive ``toctree``
pour **spécifier les modules** que vous souhaitez inclure dans votre documentation.

Voici comment vous pouvez le faire :

.. code-block:: rst

	.. toctree::
		:maxdepth: 2
		:caption: Contents :

		modules

La directive ``toctree`` permet de **créer une table des matières pour votre documentation**. 
On spécifie le titre de la table des matières en utilisant le paramètre ``:caption:``. 
Par défaut, c'est *Contents*.

Le fichier *modules* est référencé dans notre exemple. C'est le seul élément qu'on a dû 
ajouter ici, mais vous pouvez inclure d'autres fichiers ou modules selon votre structure 
de projet. Assurez-vous que les fichiers .rst correspondant aux modules que vous souhaitez 
inclure se trouvent dans le même dossier que le fichier ``index.rst``.

.. warning::  
    
    Assurez-vous de laisser une **ligne vide** entre les paramètres de la directive et le contenu. 
    Cette ligne vide est essentielle pour séparer les paramètres de la directive du reste du contenu.

Si vous disposez d'une **documentation existante** au format .md ou .rst que vous souhaitez 
intégrer, vous pouvez utiliser la directive ``include`` pour l'inclure dans votre fichier ``index.rst``. 

.. code-block:: rst
	
	.. include:: nom_doc_externe.md

Assurez-vous que le fichier de documentation externe se trouve dans le même dossier que 
les fichiers .rst. Cela vous permettra d'intégrer facilement du contenu existant à votre 
documentation générée par Sphinx.
