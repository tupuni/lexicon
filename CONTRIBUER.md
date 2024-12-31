# Contribuer au projet ***Lexicon***
Les données du ***Lexicon*** sont stockées à différents emplacements:
 - une table CSV [lexicon.csv](https://github.com/tupuni/lexicon/blob/main/lexicon.csv)
 - des illustrations (photographies ou représentations graphiques) pour chaque entrée dans le [dossier figures](https://github.com/tupuni/lexicon/blob/main/figures)
 - une liste de références bibliographiques dans le [fichier .bib](https://github.com/tupuni/lexicon/blob/main/lexicon.bib)

Ajouter ou mettre à jour des données dans le ***Lexicon*** se fait en suivant des normes particulières pour chacun de ces emplacements. 


## 1 La table du ***Lexicon***
La table est constituée des colonnes suivantes:  

[1-4] les premières colonnes contiennent les termes dans différentes langues, y compris anglais (*`EN`*), français (*`FR`*), allemand (*`DE`*), et espagnol (*`ES`*).  

[5] *`domain`*  
représente les trois sous-parties du ***Lexicon*** divisées par types d'industries : `bone` (pour toutes les matières dures animales), `ceramic`, ou `lithic`.  

[6] *`category`*  
correspond à une variable thématique du ***Lexicon***, dont les modalités peuvent être `concept`, `object`, ou `trace`.  

[7] *`definition:en`*   
contient la définition du terme en langue anglaise. Les citations extraites d'ouvrages doivent être non seulement être marquées par des guillemets (utiliser 3 double guillemets """text""" lorsque vous éditez le CSV) mais aussi citer la source selon le modèle suivant: `(author year: page)`.  

[8] *`definition:native`*  
contient la définition du terme dans d'autres langues que l'anglais. Les citations extraites d'ouvrages doivent être non seulement être marquées par des guillemets (utiliser 3 double guillemets """text""" lorsque vous éditez le CSV) mais aussi citer la source selon le modèle suivant: (author year: page).  

[9] *`figures`*  
répertorie les illustrations stockées dans le [dossier figures](https://github.com/tupuni/lexicon/blob/main/figures) grâce à des identifiants uniques. Cette colonne peut également lister des resources externes grâce à des URL/URI ou DOI.  

[10] *`references`*  
répertorie les références bibliographiques avec des idenfitiants uniques placés dans le [fichier .bib](https://github.com/tupuni/lexicon/blob/main/lexicon.bib).  

[11] *`related`* 
répertorie les entrées logiquement reliées dans le ***Lexicon*** (synonymes, ou  hierarchically related in an ontology).  

[12] *`URI`*  
Un Uniform Resource Identifiers fait le lien avec l'entrée correspondante dans le  [Thesaurus Pactols](https://pactols.frantiq.fr/).  

[13] *`note`* 
non mandatory free comments section.  


### 1-1 Procédure pour ajouter de nouvelles données
In [lexicon.csv](https://github.com/tupuni/lexicon/blob/main/lexicon.csv) columns are separated by commas (`,`) and items within the same column (such as Figure codes and Reference codes) must be separated by semicolons (`;`). The use of commas within a text must be handled as a special case, with the text wrapped within double quotation marks (`"text,text"`).

There are two ways to add new data in the repository :  
(1) **Using the web-based editor** (which should be preferred if you discover Git). 
<details>
  <summary> Procedure </summary>
 
1) Open [lexicon.csv](https://github.com/tupuni/lexicon/blob/main/lexicon.csv) and click the **Edit** button.  

2) Press `Enter` to add a new line following alphabetical order.  

3) Then add the following line
   `,,,,,," "," ",,,,,`

4) Start editing this new row following the pattern described above in [1 The ***Lexicon*** table](CONTRIBUTING.md#1-The-Lexicon-table)  
   
5) Save your changes using the `commit` button, if possible after every addition or modification of a each lexical entry.  
If you would like to modify more than one row in the table entry, please do so for every single row: indicate your action in a short descriptive message in the **Commit message** (example: `Add item x`, or `Add DE version for item x`, or `Modify description y`) before pressing **Commit changes** (on the main branch).

![edit](archives/edit.png) 
</details>
or   

(2) **Working locally** and using the Desktop app or Git commands to synchronize your version of the files with the main branch of the online repository.
<details>
  <summary> Procedure </summary>

1) Download and install the [GitHub Desktop App](https://github.com/apps/desktop)

2) Clone the repository using the HTTPS path `https://github.com/tupuni/lexicon.git` visible in the **code** panel

3) Paste the HTTPS path in the URL section of the cloning function. Check the local path to find out/choose where your Github files will be stored locally, i.e. on your computer.

![clone](archives/clone.png) 

4) Find the repository on your computer, start using them or add new files.

5) Save your changes on the main branch using the `Commit to main` button, if possible after every addition or modification of a each lexical entry.  
If you would like to modify more than one row in the table entry, please do so for every single row: indicate your action in a short descriptive message in the **Commit message** (example: `Add item x`, or `Add DE version for item x`, or `Modify description y`) before pressing **Commit changes** (on the main branch).
![commit](archives/commit.png)
![push](archives/push.png)

6) Check GitHub Desktop for possible changes on the main branch: `fetch` and `pull` to get the last changes from other users
![fetch](archives/fetch.png)
![pull](archives/pull.png)
</details>

### 1-2 Procedure to suggest modifications
1) Open an issue with the top **Issues** tab, 
![issue1](archives/issue1.png) 

2) Click on the green **New Issue** button at the top right.
![issue2](archives/issue2.png) 

3) Use the `Lexical item` as the **Title** for your issue.  

4) In the **Description** section, paste the permalink to the related entry in [lexicon.csv](https://github.com/tupuni/lexicon/blob/main/lexicon.csv). 
> [!TIP]  
> How to get a permalink :
> 1) Click on the line
> 2) Click on the `...` button
> 3) Choose `copy permalink`
> 4) Example for the first row : `https://github.com/tupuni/lexicon/blob/.../lexicon.csv#L1`

5) If necessary, assign one or several collaborator-s to that issue in order to explicitaly encourage them to participate in the discussion (see the **Assignee** button).

7) Click on **Submit new issue**.

8) Follow and comment in the discussion below.
</details>

## 2 The ***Lexicon*** figures
Each ***Lexicon*** entry should be illustrated with an associated figure in the [dedicated folder](https://github.com/tupuni/lexicon/blob/main/figures).  

1) Name your picture according to the unique identifier(s) in the related ***Lexicon*** entry - see the `Figures` column of [lexicon.csv](https://github.com/tupuni/lexicon/blob/main/lexicon.csv).  
> [!CAUTION]  
> - The figure file name and unique identifier should be created according to the following pattern : `entryname_referencecode.extension`  
Example : `splitfracture_faivre2010_1.png`.  
> - Make sure the picture quality is sufficient (min 300 dpi).  
> - Accepted extensions are jpg, png, tiff ou pdf. Please don't use proprietary formats such as .ai or .ps.

2) Add your picture in the [**Figures** folder](https://github.com/tupuni/lexicon/blob/main/figures) using the **Upload** function.
![upload](archives/upload.png) 

3) Insert the unique identifier in the related ***Lexicon*** entry in [lexicon.csv](https://github.com/tupuni/lexicon/blob/main/lexicon.csv).

## 3 The ***Lexicon*** references
1) Open the [Zotero Group Library](https://www.zotero.org/groups/5548572/lexicon), using either the [Web Application](https://www.zotero.org) or the [Desktop Application](https://www.zotero.org/support/installation).  

2) Add the new reference details and the Reference unique identifier **as a note**.  
NB : Reference code = first author name + year of publication (ex: faivre2010).  
![zotero](archives/zotero.png) 

3) Insert the unique identifier in the related ***Lexicon*** entry in [lexicon.csv](https://github.com/tupuni/lexicon/blob/main/lexicon.csv).

> [!CAUTION]  
> Do not modify the .bib file in the repository. The ***Lexicon*** maintainers will update the .bib file based on newly added references in the Zotero Group Library.  



[Back to top](CONTRIBUTING.md##contribuer-au-projet-lexicon)  
