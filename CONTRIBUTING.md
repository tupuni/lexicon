# Contributing to the Lexicon
The Lexicon data is stored in multiple locations:
 - a CSV table [lexicon.csv](https://github.com/tupuni/lexicon/blob/main/lexicon.csv)
 - photographs or graphic representations of each entry in the [figures folder](https://github.com/tupuni/lexicon/blob/main/figures)
 - a bibliographical reference list in the dedicated [.bib file](https://github.com/tupuni/lexicon/blob/main/lexicon.bib)

Adding or updating data in the Lexicon requires following specific guidelines for each of these locations. 

[1 The Lexicon table](CONTRIBUTING.md#1-The-Lexicon-table)  
[1-1 Procedure to add new data](CONTRIBUTING.md#1-1-procedure-to-add-new-data)  
[1-2 Procedure to suggest modifications](CONTRIBUTING.md#1-2-procedure-to-suggest-modifications)  
[2 The Lexicon figures](CONTRIBUTING.md#2-The-Lexicon-figures)  
[3 The Lexicon references](CONTRIBUTING.md#3-The-Lexicon-references)  

## 1 The Lexicon table
The table is made of the following columns:  
[1-4] the first columns store lexical items in different languages, including English (`EN`), French (`FR`), German (`DE`), and Spanish (`ES`).  
[5] `domain` represents a subsection of the Lexicon and can either relate to `bone`, `ceramic` or `lithic` industries.  
[6] `category` corresponds to a thematic variable which modalities are `concept`, `object` and `trace`.  
[7] `definition:en` stores unified semantic values in english. Exact citations need to use quotes (use 3 quotes `"""text"""` while editing the CSV to render actual quotes) and cite the source using the following pattern: `(author year: page)`.  
[8] `definition:native` stores unified semantic values in other languages.  
[9] `figures` lists related figures through image codes (unique identifiers) located in the [figures folder](https://github.com/tupuni/lexicon/blob/main/figures). Alternatively it can also refer to external resources through URL/URI or DOI.  
[10] `references` lists related bibliographical references through reference codes (unique identifiers) located in the [.bib file](https://github.com/tupuni/lexicon/blob/main/lexicon.bib).  
[11] `related` connects the entry with other related entries in the Lexicon (synonyms, or hierarchically related in an ontology).  
[12] `URI` (Uniform Resource Identifiers) identifies the corresponding entry in the [Pactols Thesaurus](https://pactols.frantiq.fr/).  
[13] `note` is a non mandatory free comments section.  


### 1-1 Procedure to add new data
In [lexicon.csv](https://github.com/tupuni/lexicon/blob/main/lexicon.csv) columns are separated by commas (`,`) and items within the same column (such as Figure codes and Reference codes) must be separated by semicolons (`;`). The use of commas within a text must be handled as a special case, with the text wrapped within double quotation marks (`"text,text"`).

There are two ways to add new data in the repository: 
- using the web-based editor
or
- working locally on your machine and using [GitHub Desktop App](https://github.com/apps/desktop) to synchronize your version of the files with the main branch of the online repository.

#### 1-1-1 Adding new data using web-based editor 

1) Open [lexicon.csv](https://github.com/tupuni/lexicon/blob/main/lexicon.csv) and click the **Edit** button.  
![edit-table](archives/edit-table.png) 

2) Press `Enter` to add a new line following alphabetical order.  

3) Then add the following line
   `,,,,,," "," ",,,,,`
![edit-row](archives/edit-row.png) 

5) Start editing this new row following the pattern described above in [1 The Lexicon table](CONTRIBUTING.md#1-The-Lexicon-table)  
   
6) Save your changes using the `commit` button, if possible after every addition or modification of a each lexical entry.  
If you would like to modify more than one row in the table entry, please do so for every single row: indicate your action in a short descriptive message in the **Commit message** (example: `Add item x`, or `Add DE version for item x`, or `Modify description y`) before pressing **Commit changes** (on the main branch).

#### 1-1-2 Working locally and using the GitHub Desktop App

1) Download and install the [GitHub Desktop App](https://github.com/apps/desktop)

2) Clone the repository using the HTTPS path `https://github.com/tupuni/lexicon.git`
![clone1](archives/clone1.png) 

3) Paste the HTTPS path in the URL section of the cloning function. Check the local path to find out/choose where your Github files will be stored locally, i.e. on your computer.
![clone2](archives/clone2.png)
![clone3](archives/clone3.png)

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

4) In the issue **Description**, paste the path to the Lexicon entry by referring to the line in the CSV table, which you get by:
- clicking on the line,
- then on the `...` button
- and then on `copy permalink`
(example for the first row):
```
https://github.com/tupuni/lexicon/blob/.../lexicon.csv#L1
```

5) If necessary, assign one or several collaborator-s to that issue in order to explicitaly encourage them to participate in the discussion (see the **Assignee** button).

7) Click on **Submit new issue**.

8) Follow and comment in the discussion below.

## 2 The Lexicon figures
Each Lexicon entry should be illustrated with an associated figure in the [dedicated folder](https://github.com/tupuni/lexicon/blob/main/figures).  

1) Name your picture according to the unique identifier(s) in the related Lexicon entry - see the `Figures` column of the **Lexicon table**.  
*NB 1 : The figure file name and unique identifier should be created according to the following pattern : entryname_referencecode.extension  
Example : splitfracture_faivre2010_1.png*.  
*NB 2 : Make sure the picture quality is sufficient (min 300 dpi).*  
*NB 3 : Accepted extensions are jpg, png, tiff ou pdf. Please don't use proprietary formats such as **.ai** or **.ps**.*

2) Add your picture in the [**Figures** folder](https://github.com/tupuni/lexicon/blob/main/figures) using the **Upload** function.
![upload](archives/upload.png) 

3) Insert the unique identifier in the related Lexicon entry in [lexicon.csv](https://github.com/tupuni/lexicon/blob/main/lexicon.csv).

## 3 The Lexicon references
1) Open the [Zotero Group Library](https://www.zotero.org/groups/5548572/lexicon), using either the [Web Application](https://www.zotero.org) or the [Desktop Application](https://www.zotero.org/support/installation).  

2) Add the new reference details and the Reference unique identifier **as a note**.  
*NB : Reference code = first author name + year of publication (ex: faivre2010)*.  
![zotero](archives/zotero.png) 

3) Insert the unique identifier in the related Lexicon entry in [lexicon.csv](https://github.com/tupuni/lexicon/blob/main/lexicon.csv).

4) **Do not modify the .bib file in the repository**. The Lexicon maintainers will update the .bib file based on newly added references in the Zotero Group Library.  

[1 The Lexicon table](CONTRIBUTING.md#1-The-Lexicon-table)  
[2 The Lexicon figures](CONTRIBUTING.md#2-The-Lexicon-figures)  
[3 The Lexicon references](CONTRIBUTING.md#3-The-Lexicon-references)  
