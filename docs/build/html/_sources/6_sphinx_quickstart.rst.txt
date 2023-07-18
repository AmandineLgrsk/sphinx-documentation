6. Sphinx-quickstart
====================

Cette étape consiste à **créer la structure de base du dossier de documentation** qui sera le dossier  *docs*.

A la racine de votre projet, ouvrez un terminal et tapez la commande suivante pour créer le dossier docs : 

.. code-block:: console

	$ mkdir docs

Puis accédez au dossier :

.. code-block:: console

	$ cd docs

Ensuite, exécutez la commande suivante pour initialiser le projet Sphinx :

.. code-block:: console

	$ sphinx-quickstart

Après avoir exécuté ``sphinx-quickstart``, vous serez invité à répondre à plusieurs 
questions pour configurer votre projet Sphinx. Voici les questions et les réponses 
recommandées pour certaines questions :

.. code-block:: console

    Separate source and build directories (y/n) [n]: y
    Project name: [Nom de votre projet]
    Author name(s): [Votre nom]
    Project release []: [Date de votre projet]


.. figure:: ./images/8_sphinx_quickstart.PNG
    :align: center

    Questions et réponses possibles lors de l'exécution de ``sphinx-quickstart``

Vous pouvez laisser les autres questions avec les valeurs par défaut ou y répondre en fonction de vos préférences.

.. tip:: 
    
    Je vous recommande de répondre **y** à la première question. Cela permet de séparer les dossiers *source* et *build*. 
    Cela aide à maintenir une structure de projet plus organisée.

Une fois que vous avez répondu à toutes les questions, le projet Sphinx sera initialisé avec 
les fichiers et les dossiers nécessaires à la génération de la documentation.

.. figure:: ./images/9_squelette_dossier_docs.PNG
    :align: center

    Squelette du dossier *docs* ainsi généré

.. note::
    
    Il sera possible de modifier les informations fournies lors de cette étape telles que le nom 
    du projet, votre nom et la date réalisation en éditant le fichier ``conf.py``.
