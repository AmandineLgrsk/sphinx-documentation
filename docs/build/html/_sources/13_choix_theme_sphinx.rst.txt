13. Choix d'un thème Sphinx
===========================

Il existe **plusieurs thèmes disponibles pour personnaliser l'apparence 
de votre documentation**. Vous pouvez retrouver la liste des thèmes 
`ici <https://sphinx-themes.org/#themes>`_ .

Pour utiliser un thème spécifique, vous devez l'installer via votre terminal.

Pour chaque thème, il est précisé comment il faut procéder pour l'utiliser. 

Prenons le thème *renku*.

.. code-block:: console

    $ conda install renku-sphinx-theme

Après avoir installé le thème, vous devez le configurer dans votre fichier 
``conf.py`` pour qu'il soit appliqué à votre documentation. Pour ce faire, 
modifiez la ligne suivante dans le fichier ``conf.py`` : 

.. code-block:: python

	html_theme = 'renku'

et mettre en commentaire la ligne suivante :

.. code-block:: python
	
    # html_static_path = ['_static']

Remplacez *renku* par le nom du thème que vous souhaitez utiliser.

Une fois que vous avez configuré le thème dans votre fichier ``conf.py``, 
générez à nouveau la documentation en utilisant la commande ``make html``. 
La documentation sera générée avec le nouveau thème appliqué. 

Voici la nouvelle documentation générée avec le thème *renku* :

.. figure:: ./images/17_renku_page_accueil.PNG
    :align: center

    Page d'accueil de la documentation générée

.. figure:: ./images/18_renku_sommaire.PNG
    :align: center

    Sommaire de la documentation générée
    
.. figure:: ./images/19_renku_fonction.PNG
    :align: center

    Exemple de documentation d'une fonction

.. tip:: 
    
    Explorez différents thèmes et choisissez celui qui correspond le mieux à vos besoins 
    et à l'apparence que vous souhaitez donner à votre documentation.

Si vous rencontrez des difficultés à installer un thème via conda, vous pouvez utiliser l'alternative 
suivante pour créer un **environnement virtuel** et installer le thème souhaité.

Vérifiez que votre version de conda est à jour en exécutant la commande :

.. code-block:: console

    $ conda update conda

Créez un nouvel environnement virtuel avec le nom de votre choix. 
Par exemple, ici on utilise ``myenv`` comme nom d'environnement.

.. code-block:: console

    $ conda create -name myenv

Activez l'environnement virtuel comme suit :

.. code-block:: console

    $ conda activate myenv

Ensuite, vous pouvez installer le thème à l'aide de conda.

.. code-block:: console

    $ conda install renku

Après avoir suivi ces étapes, vous devriez être en mesure d'utiliser le thème 
installé pour personnaliser l'apparence de votre documentation. N'oubliez pas de 
configurer le thème dans votre fichier ``conf.py`` comme indiqué précédemment, puis 
générez à nouveau la documentation en faisant ``make html``.



