15. Sur Windows
===============

Si vous travaillez sur **Windows**, vous pouvez suivre les mêmes étapes que celles 
décrites précédemment pour la génération de la documentation. 

Cependant, il peut y avoir quelques différences lors de l'exécution de certaines commandes.

De plus, vous devrez utiliser **Git Bash** comme terminal sur Windows pour exécuter les commandes.

Lors de l'exécution de la commande ``make html``, vous devrez effectuer une modification 
pour Windows. Au lieu d'utiliser ``make html``, vous devrez utiliser la commande suivante :
 
.. code-block:: console

    $ .\make.bat hmtl

Si vous rencontrez des problèmes lors de l'exécution de cette commande, vous pouvez 
essayer la commande suivante :

.. code-block:: console
    
    $ cmd.exe /c make.bat html
    $ .\make.bat hmtl

Assurez-vous de suivre les autres étapes de la notice telles quelles en adaptant 
uniquement la commande pour la génération de la documentation sur Windows.

