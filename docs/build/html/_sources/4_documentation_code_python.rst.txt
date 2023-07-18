4. Documentation du code python
===============================

Pour documenter votre code Python, vous pouvez suivre les étapes suivantes :

* Ajouter une **documentation en tête à chaque fichier Python** pour qu'il soit reconnu par Sphinx. Vous pouvez utiliser un commentaire multi-lignes pour décrire le contenu du fichier tel que :

    .. code-block:: python

        """
        Description du fichier
        ======================

        Il est possible de renseigner diverses informations telles que :
        -	Quelles sont les fonctions présentes dans le script ?
        -	Quels sont les packages que je dois importer ? 
        -	Quelles sont les dépendances entre les fichiers ?
        -	…
        """
        
    Cette description permet d'expliquer brièvement le contenu et le contexte du fichier, 
    ce qui facilite la compréhension pour les autres utilisateurs.

* Utilisez les **Docstrings** pour générer automatiquement la documentation. Les Docstrings sont des chaînes de caractères placées au début d'une fonction, d'une classe ou d'un module pour documenter son fonctionnement.

    Considérons la fonction ``perimetre_carre(c)``. Voici un exemple de génération automatique de Docstring par Python :

    .. figure:: ./images/3_code_python_sans_docstring.PNG
        :align: center
        
        Code python de la fonction ``perimetre_carre``


    .. figure:: ./images/4_proposition_generation_docstring.PNG
        :align: center

        Proposition de la génération de Docstring


    .. figure:: ./images/5_squelette_docstring.PNG
        :align: center

        Squelette pour la documentation de la fonction


* Complétez la documentation générée automatiquement en **ajoutant des informations spécifiques à votre code**. Cela inclut la **description des paramètres, de leur type, des valeurs de retour et toute autre information pertinente**.

    .. figure:: ./images/6_docstring_complet.PNG
        :align: center
        
        Informations de la fonction

    .. note:: 
        
        Vous pouvez aussi utiliser une **combinaison de markdown et de reStructuredText** 
        dans vos Docstring pour formater le texte de manière plus lisible et attrayante.

    .. figure:: ./images/7_docstring_md_rst.PNG
        :align: center

        Docstring constituée de markdown et de reStructuredText  

.. attention:: 
    
    Les commentaires, c'est-à-dire les textes précédés d'un dièse # ne seront 
    pas affichés dans la documentation générée par Sphinx.

