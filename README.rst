OntoContext
======
To annotate biomedical texts using three ontologies and gene names recovering using the geniatagger: 
+-----------------------------+--------------------------+
Cell Ontology (CL)						|	Cell populations         |
Human Disease Ontology (DOID)	|	Pathologies              |
Anatomical Ontology (UBERON)	|	Anatomical localisation  |
+-----------------------------+--------------------------+


Prerequisites
-------------
This package is coded using python 2.7
It need: 
|the NLTK package
|the geniatagger package
|| the geniatagger folder can be downloaded from here (http://www.nactem.ac.uk/tsujii/GENIA/tagger/geniatagger-3.0.2.tar.gz) 
|the sqlite3 package 
|the Tkinter package 
|the operator package
|the Concept databases can be downloaded from here (https://github.com/walidbedhiafi/OntoContext1/blob/master/OntoContext/Concepts.sqlite)


Installation
------------
This package is tested under Linux Python 2.7 and is available from the PyPI.  
To install via pip :

     pip install ontocontext

Usage
-----

import OntoContext
from OntoContext.annot import annotation 
from OntoContext.crisscross import crisscross
annotation('path_to_texts_folder', 'table_name_to_store_annotations', 'path_to_the_genia_tagger') 
print crisscross('table_name_to_store_annotations')


License
-------
OntoContext is distributed under a `MIT License`.

