1. Langage reStructuredText
===========================

Dans cette section, on va découvrir les **éléments de balisages** les plus utiles de **reStructuredText**, 
qui vous aideront à formater et organiser votre documentation de manière claire et cohérente.

Mises en forme 
--------------

Vous pouvez appliquer des mises en forme spécifiques au texte en utilisant les balises appropriées:

- Le texte peut être mis en gras en l'entourant de **doubles astérisques**.

.. code-block:: rst

	**texte en gras**

**texte en gras**

-	Le texte peut être mis en italique en l'entourant d'**astérisques simples**.

.. code-block:: rst

	*texte en italique*

*texte en italique*

Les titres
----------

Les **titres** aident à structurer le contenu et à faciliter la navigation pour les lecteurs. 
Vous pouvez utiliser différentes balises pour créer des titres de différents niveaux :

.. code-block:: rst
	
	*************
	Titre de page
	*************

.. code-block:: rst

	Titre de niveau 1
	=================

.. code-block:: rst

	Titre de niveau 2
	-----------------
.. code-block:: rst

	Titre de niveau 3
	*****************

.. code-block:: rst

	Titre de niveau 4
	~~~~~~~~~~~~~~~~~

.. code-block:: rst

	Titre de niveau 5
	+++++++++++++++++

.. code-block:: rst

	``exemple``
	===========
	
Les paragraphes
---------------

Les paragraphes sont simplement des **blocs de texte séparés par des lignes vides**.

Les directives
--------------

Les **directives** permettent de mettre en évidence des informations importantes ou 
des remarques spécifiques dans votre documentation.

Voici quelques directives couramment utilisées :

- ``note`` permet de mettre en évidence des remarques.

.. code-block:: rst
	
	.. note:: Ceci est une note.

.. note:: Ceci est une note.

- ``warning`` est utilisé pour indiquer des avertissements importants.

.. code-block:: rst

	.. warning :: Ceci est un avertissement.

.. warning :: Ceci est un avertissement.

- ``important`` est utilisé pour mettre en évidence des informations essentielles.

.. code-block:: rst

	.. important:: Ceci est important.

.. important:: Ceci est important.

- ``tip`` est utilisé pour donner des conseils.

.. code-block:: rst

	.. tip:: Ceci est un conseil.

.. tip:: Ceci est un conseil.

- ``attention`` est utilisé pour attirer l'attention du lecteur.

.. code-block:: rst

	.. attention:: Ceci est pour attirer l'attention.

.. attention:: Ceci est pour attirer l'attention.

- ``caution`` est utilisé pour prévenir le lecteur d'être prudent sur un certain point.

.. code-block:: rst

	.. caution:: Ceci est pour prévenir d'être prudent sur un point.

.. caution:: Ceci est pour prévenir d'être prudent sur un point.

- ``danger`` est utilisé pour avertir sur un danger potentiel.

.. code-block:: rst

    .. danger:: Ceci est un danger.

.. danger:: Ceci est un danger.

- ``error`` est utilisé pour avertir une erreur potentielle.

.. code-block:: rst

	.. error:: Ceci est une erreur.

.. error:: Ceci est une erreur.

Les listes
----------

Les **listes non ordonnées** sont créées en utilisant des **astérisques (*)**, 
des **tirets  (–)** ou des **signes plus (+)**.

Les **listes ordonnées** sont créées en utilisant des **chiffres suivis d'un point**.

Les blocs de code
-----------------

Les blocs de code sont créés en utilisant la directive ``code-block``.

.. code-block:: rst

	.. code-block:: langage de programmation

Où *'langage de programmation'* peut être ``python``, ``console``, ``java``, ``rst``, …

Les liens
---------

Vous pouvez créer des **liens hypertextes** en utilisant la syntaxe suivante :

.. code-block:: rst

	Lien vers le site officiel de `Sphinx <https://www.sphinx-doc.org/en/master/>`_

Lien vers le site officiel de `Sphinx <https://www.sphinx-doc.org/en/master/>`_

Les images
----------

Vous pouvez insérer des **images** dans votre documentation en utilisant la 
directive ``figure`` et en **spécifiant le chemin vers l'image**.

.. code-block:: rst

	.. figure:: chemin/vers/l/image


Ce ne sont là que quelques-unes des balises de base utilisées dans reStructuredText. 
Il existe d'autres balises pour formater des tables, des citations, etc. Pour une référence 
complète de la syntaxe reStructuredText, vous pouvez consulter la documentation officielle 
`ici <https://www.sphinx-doc.org/en/master/usage/restructuredtext/index.html>`_
