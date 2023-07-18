10. Génération de la documentation
==================================

En supposant que vous vous trouvez à la racine de votre, vous devez 
vous placer dans le dossier *docs* pour exécuter les commandes suivantes :

Dans votre terminal, tapez

.. code-block:: console

    $ cd docs

Pour accéder au dossier *docs* puis 

.. code-block:: console

	$ make html

Pour générer la documentation au format ``html``. 

Cette commande va générer les fichiers ``html`` de votre documentation 
à l'aide de Sphinx. Les fichiers générés se trouveront dans le dossier 
*docs/build/html*.

.. important:: 
    
    Une fois la documentation générée, vous pouvez accéder au **menu principal** en ouvrant le fichier ``index.html``
    dans le dossier *docs/build/html*.

.. tip:: 
    
    Si vous apportez des modifications à votre code et que vous souhaitez regénérer la documentation en conséquence, 
    vous pouvez exécuter les commandes suivantes :

    .. code-block:: console

        $ make clean
        $ make html

    La commande ``make clean`` supprime les fichiers générés précédemment, 
    puis la commande ``make html`` génère à nouveau la documentation mise à jour.


