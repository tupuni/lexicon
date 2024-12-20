# Contribuer au projet Lexicon
Les données du Lexicon sont stockées à différents emplacements:
 - une table CSV [lexicon.csv](https://github.com/tupuni/lexicon/blob/main/lexicon.csv)
 - des photographies ou représentations graphiques pour chaque entrée dans le [dossier figures](https://github.com/tupuni/lexicon/blob/main/figures)
 - une liste de références bibliographiques dans le [fichier .bib](https://github.com/tupuni/lexicon/blob/main/lexicon.bib)

Ajouter ou mettre à jour des données dans le Lexicon se fait en suivant des normes particulières pour chacun de ces emplacements. 

[1 La table du Lexicon](CONTRIBUTING.md#1-La-table-du-Lexicon)  
[1-1 Procédure pour ajouter de nouvelles données](CONTRIBUER.md#1-1-procédure-pour-ajouter-de-nouvelles-données)  
[1-2 Procédure pour suggérer des modifications](CONTRIBUER.md#1-2-procedure-pour-suggérer-des-modifications)  
[2 Les figures du Lexicon figures](CONTRIBUER.md#2-Les-figures-du-Lexicon-figures)  
[3 Les références du Lexicon references](CONTRIBUTING.md#3-Les-références-du-Lexicon)  

## 1 La table du Lexicon
La table est constituée des colonnes suivantes:  
[1-4] les premières colonnes contiennent les termes dans différentes langues, y compris anglais (`EN`), français (`FR`), allemand (`DE`), et espagnol (`ES`).  
[5] `domain` représente les trois sous-parties du Lexicon divisées par types d'industries : `bone` (pour toutes les matières dures animales), `ceramic`, ou `lithic`.
[6] `category` correspond à une variable thématique du Lexicon, dont les modalités peuvent être `concept`, `object`, ou `trace`.
[7] `definition:en` contient la définition du terme en langue anglaise. Les citations extraites d'ouvrages doivent être non seulement être marquées par des guillemets (utiliser 3 double guillemets """text""" lorsque vous éditez le CSV) mais aussi citer la source selon le modèle suivant: (author year: page).
[8] `definition:native` contient la définition du terme dans d'autres langues que l'anglais. Les citations extraites d'ouvrages doivent être non seulement être marquées par des guillemets (utiliser 3 double guillemets """text""" lorsque vous éditez le CSV) mais aussi citer la source selon le modèle suivant: (author year: page).
[9] `figures` lists related figures through image codes (unique identifiers) located in the [figures folder](https://github.com/tupuni/lexicon/blob/main/figures). Alternatively it can also refer to external resources through URL/URI or DOI.  
[10] `references`lists related bibliographical references through reference codes (unique identifiers) located in the [.bib file](https://github.com/tupuni/lexicon/blob/main/lexicon.bib).  
[11] `related` connects the entry with other related entries in the Lexicon (synonyms, or hierarchically related in an ontology).  
[12] `URI` (Uniform Resource Identifiers) identifies the corresponding entry in the [Pactols Thesaurus](https://pactols.frantiq.fr/).  
[13] `note` is a non mandatory free comments section.  


### 1-1 Procedure to add new data


