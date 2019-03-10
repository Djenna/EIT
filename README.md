# PROJET EIT

***********************************

PTBtoUniv.py : Change les tags PTB d'un fichier en suivant une table de correspondance

Syntaxe: python PTBtoUniv.py Path_To_POSTags_PTB_Universal_Linux.txt Path_To_Input.txt Path_to_output.txt
Exemple: python PTBtoUniv.py POSTags_PTB_Universal_Linux.txt wsj_0010_sample.txt.pos.stanford wsj_0010_sample.txt.pos.univ.stanford

***********************************

FormatNER.py : Represente un resultat de l'outil de reconnaissance des entites nommees de Stanford sous une nouvelle forme

Syntaxe: python FormatNER.py Path_To_Input.txt Path_to_output.txt
Exemple: python FormatNER.py formal-tst.NE.key.04oct95_small.txt.output new-format.NE.key.04oct95_small.txt

***********************************

FormatRefToLima.py : Transforme les balises ENAMEX d'un fichier en "\_TAG"

Syntaxe: python FormatRefToLima.py Path_To_Input.txt Path_to_output.txt
Exemple: python FormatRefToLima.py formal-tst.NE.key.04oct95_small.ne output.04oct95.ne.lima

***********************************

FormatEspace.py : Transforme les "Espaces" compris dans les mots composes comme "BocaEspaceRaton_TAG" en "Boca_TAG Raton_TAG"

Syntaxe: python FormatEspace.py Path_To_Input.txt Path_to_output.txt
Exemple: python FormatEspace.py output.04oct95.ne.lima output.04oct95.ne.stanford

***********************************

LimaToStanford.py : Permet de changer les tags LIMA d'un fichier en suivant une table de correspondance (identique a PTBtoUniv.py)

Syntaxe: python LimaToStanford.py Path_To_POSTags_LIMA_Stanford.txt Path_To_Input.txt Path_to_output.txt

***********************************

toEvaluateFormat.py : Modifie les etiquettes des entites nommes "/TAG" en "\_TAG" pour pouvoir utiliser le script evaluate.py

Syntaxe: python toEvaluateFormat.py Path_To_Input.txt Path_to_output.txt
Exemple: python toEvaluateFormat.py formal-tst.NE.key.04oct95_small.txt.output stanford.eval.txt.output
