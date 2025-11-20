# Female Abolitionist Poets

## Corpus
This dataset contains a brief selection of female authored poets, manually collected from [Brycchan Carey's website](https://brycchancarey.com/slavery/poetry.htm)
This list contains several poems authored by both men and women, but for the scope of this project (max 10.000 tokens) a selection of female poetry has been made. 

The target audience is anyone who is interested in abolitionist or female literature, or anybode else who might find this data useful in any way.

As mentioned before, the poems that were selected had the criterium of female authorship and token length. 

The data has manually been collected from [Brycchan Carey's website](https://brycchancarey.com/slavery/poetry.htm), who provides a preselection of antislavery poems in digital format. The metadata has also been manually created.

## Cleaning and Preproccesing
In general the textual data was of very good quality. One data cleaning measure i took was removing whitespaces between word characters in titles for the purpose of better tokenization. (P O E M --> POEM)

/t and /n have been removed from the text before tokenizing. The tokenization and lemmatization were performed using the spaCy library for python. The code can be reviewed in the Jupyter Notebook in this repo.

## Annotated Dataset Columns

| Column | Description |
|--------|-------------|
| Filename | Name of the text file containing the work |
| Title | The full title of the literary work or poem |
| Year | Year of publication |
| Author | Name of the author |
| AuthorGender | Gender of the author |
| Link | URL to the online version of the text on Brycchan Carey's website |
| Text | Raw text content of the work |
| Doc | spaCy Doc object containing the processed text |
| Tokens | List of tokenized words from the text |
| POS | Part-of-speech tags for each token |
| Lemmas | Lemmatized forms of the tokens |



## Data Formats
The data is provided in .txt format. The metadata and the annotation data are provided as .csv files.

## Metadata Columns

| Column | Description |
|--------|-------------|
| Title | The full title of the literary work or poem |
| Year | Year of publication |
| Author | Name of the author |
| AuthorGender | Gender of the author|
| Filename | Name of the text file containing the work |
| Link | URL to the online version of the text on Brycchan Carey's website|