7. Modification du fichier de configuration
===========================================

Le fichier ``conf.py`` est l'endroit principal où vous apporterez des **modifications 
pour configurez Sphinx selon vos besoins**.

Voici les étapes pour modifier le fichier de configuration ``conf.py`` qui se trouve 
dans le dossier *docs/source/*.

Ajoutez ou décommentez les lignes suivantes pour indiquer à Sphinx où se trouve 
le code source de votre projet.

.. code-block:: python

    import os
    import sys

    sys.path.insert(0, os.path.abspath('../../python/')

Assurez-vous de remplacer *'../../python/'* par le chemin réel vers le dossier qui contient votre code source.

Ajoutez les **extensions** en modifiant la liste *extensions*. Je vous recommande d'ajouter les extensions suivantes : 

.. code-block:: python

	extensions = [
		'sphinx.ext.autodoc',
		'sphinx.ext.napoleon',
		'sphinx.ext.viewcode'
	]

``'sphinx.ext.autodoc'`` => permet la génération automatique de la documentation à partir des Docstrings de votre code.

``'sphinx.ext.napoleon'`` => permet d'inclure du markdown dans vos Docstrings.

``'sphinx.ext.viewcode'`` =>  permet aux utilisateurs de visualiser le code source directement depuis la documentation générée.

Vous pouvez ajouter d'autres `extensions <https://www.sphinx-doc.org/en/master/usage/extensions/index.html>`_ en 
fonction de vos besoins spécifiques.

Une fois les modifications apportées au fichier ``conf.py``, sauvegardez le et passez 
à l'étape suivante pour générer les fichiers reStructuredText (.rst) à partir de votre code source.

