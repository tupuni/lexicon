# Contributing to the ***Lexicon***
The ***Lexicon*** data is stored in multiple locations:
 - a CSV table [lexicon.csv](https://github.com/tupuni/lexicon/blob/main/lexicon.csv)
 - photographs or graphic representations of each entry in the [figures folder](https://github.com/tupuni/lexicon/blob/main/figures)
 - a bibliographical reference list in the dedicated [.bib file](https://github.com/tupuni/lexicon/blob/main/lexicon.bib)

Adding or updating data in the ***Lexicon*** requires following specific guidelines for each of these locations.  
[1 The ***Lexicon*** table](CONTRIBUTING.md#1-The-Lexicon-table)  
[1-1 Procedure to add new data](CONTRIBUTING.md#1-1-procedure-to-add-new-data)  
[1-2 Procedure to suggest modifications](CONTRIBUTING.md#1-2-procedure-to-suggest-modifications)  
[2 The ***Lexicon*** figures](CONTRIBUTING.md#2-The-Lexicon-figures)  
[3 The ***Lexicon*** references](CONTRIBUTING.md#3-The-Lexicon-references)  

## 1 The ***Lexicon*** table
The table is made of the following columns:  

[1-4] the first columns store lexical items in different languages, including English (*`EN`*), French (*`FR`*), German (*`DE`*), and Spanish (*`ES`*).  

[5] *`domain`*  
represents the three subsections of the ***Lexicon*** which are kinds of industries: modalities can either be `bone`, `ceramic` or `lithic`.  

[6] *`category`*   
corresponds to a thematic variable which modalities are `concept`, `object` or `trace`.  

[7] *`definition:en`*   
stores unified semantic values in english. Exact citations need to use quotes (use 3 quotes `"""text"""` while editing the CSV to render actual quotes) and cite the source using the following pattern: `(author year: page)`.  

[8] *`definition:native`*  
stores unified semantic values in other languages. Exact citations need to use quotes (use 3 quotes `"""text"""` while editing the CSV to render actual quotes) and cite the source using the following pattern: `(author year: page)`.  

[9] *`figures`*  
lists related figures through unique identifiers using the following pattern: `entryname_referencecode.extension`. Figures are located in the [figures folder](https://github.com/tupuni/lexicon/blob/main/figures). Alternatively, this column can also store external resources through URL/URI or DOI.  

[10] *`references`*  
lists related bibliographical references through unique identifiers located in the [.bib file](https://github.com/tupuni/lexicon/blob/main/lexicon.bib).  

[11] *`related`*  
lists logically related entries in the ***Lexicon*** (synonyms, or hierarchically related in an ontology).  

[12] *`URI`*  
Uniform Resource Identifiers are links to the corresponding entry in the [Pactols Thesaurus](https://pactols.frantiq.fr/).  

[13] *`note`*  
non mandatory free comments section.  


### 1-1 Procedure to add new data
In [lexicon.csv](https://github.com/tupuni/lexicon/blob/main/lexicon.csv) columns are separated by commas (`,`) and items within the same column (such as Figure codes and Reference codes) must be separated by semicolons (`;`). The use of commas within a text must be handled as a special case, with the text wrapped within double quotation marks (`"text,text"`).

There are two ways to add new data in the repository : [using the web-based editor](CONTRIBUTING.md#1-1-1-adding-new-data-using-web-based-editor) or [working locally on your machine and using the desktop app](CONTRIBUTING.md#1-1-2-working-locally-and-using-the-github-desktop-app) to synchronize your version of the files with the main branch of the online repository.

#### 1-1-1 Adding new data using web-based editor 

1) Open [lexicon.csv](https://github.com/tupuni/lexicon/blob/main/lexicon.csv) and click the **Edit** button.  

![edit](archives/edit-row.png|width=10) 

2) Press `Enter` to add a new line following alphabetical order.  

3) Then add the following line
   `,,,,,," "," ",,,,,`

4) Start editing this new row following the pattern described above in [1 The ***Lexicon*** table](CONTRIBUTING.md#1-The-Lexicon-table)  
   
5) Save your changes using the `commit` button, if possible after every addition or modification of a each lexical entry.  
If you would like to modify more than one row in the table entry, please do so for every single row: indicate your action in a short descriptive message in the **Commit message** (example: `Add item x`, or `Add DE version for item x`, or `Modify description y`) before pressing **Commit changes** (on the main branch).

![edit](archives/edit.png) 

#### 1-1-2 Working locally and using the GitHub Desktop App

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

### 1-2 Procedure to suggest modifications
1) Open an issue with the top **Issues** tab, 
![issue1](archives/issue1.png) 

2) Click on the green **New Issue** button at the top right.
![issue2](archives/issue2.png) 

3) Use the `Lexical item` as the **Title** for your issue.  

4) In the issue **Description**, paste the permalink to the related entry in [lexicon.csv](https://github.com/tupuni/lexicon/blob/main/lexicon.csv) 
> [!TIP]  
> To get the permalink :
> 1) click on the line
> 2) then click on the `...` button
> 3) and then `copy permalink`
> 4) Example for the first row : `https://github.com/tupuni/lexicon/blob/.../lexicon.csv#L1`

5) If necessary, assign one or several collaborator-s to that issue in order to explicitaly encourage them to participate in the discussion (see the **Assignee** button).

7) Click on **Submit new issue**.

8) Follow and comment in the discussion below.

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

3) Insert the unique identifier in the related Lexicon entry in [lexicon.csv](https://github.com/tupuni/lexicon/blob/main/lexicon.csv).

## 3 The ***Lexicon*** references
1) Open the [Zotero Group Library](https://www.zotero.org/groups/5548572/lexicon), using either the [Web Application](https://www.zotero.org) or the [Desktop Application](https://www.zotero.org/support/installation).  

2) Add the new reference details and the Reference unique identifier **as a note**.  
NB : Reference code = first author name + year of publication (ex: faivre2010).  
![zotero](archives/zotero.png) 

3) Insert the unique identifier in the related ***Lexicon*** entry in [lexicon.csv](https://github.com/tupuni/lexicon/blob/main/lexicon.csv).

> [!CAUTION]  
> Do not modify the .bib file in the repository. The ***Lexicon*** maintainers will update the .bib file based on newly added references in the Zotero Group Library.  


Get back to :  
[1 The Lexicon table](CONTRIBUTING.md#1-The-Lexicon-table)  
[2 The Lexicon figures](CONTRIBUTING.md#2-The-Lexicon-figures)  
[3 The Lexicon references](CONTRIBUTING.md#3-The-Lexicon-references)  
