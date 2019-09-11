# Study Case Development of Life Expectancy

## Presentation

This assignment for the DH Benelux 2019 Workshop "Documenting Research Practice in DH".
It is about largely structured data, as these make it easier to illustrate and discuss the necessity to prepare them for analysis and the consequences of the various steps needed for data preparation. Data originate from the Dutch Biography Portal ([http://biografischportaal.nl]), that combines data from many sources. The data were partially cleaned.

## The challenge - a newspaper article

In 2011 an article appeared in the Dutch NRC newspaper that state that demographers discovered that painters and sculptors in the seventeenth century (the Dutch Golden Age) were part of the middle classes but that they lived longer than members of the aristocracy. Their conclusion was based on the comparison of the data from the RKD Artists database with some prosopographies of 'aristocrats' (Dutch: regenten) from Zealand and Leiden. This surprised the demographers as in modern times a lower socio-economic status often means a lower life expectancy [Joke Mat, "Er was iets met die schilders in de Gouden Eeuw", NRC 24 November, 2011](https://www.nrc.nl/nieuws/2011/11/24/er-was-iets-met-die-schilders-in-de-gouden-eeuw-12113509-a1183926)

In general, there are not many data available about life expectancy before the statistical period in the 19th century started. Often heard generalizations that people before modern times did not live beyond 35 years are rough estimates mostly based on archaeology and include child mortality. However, there were always people who lived much longer than 35, even in the most primitive societies. We have only scattered data about life expectancy and especially no data about specific groups. However, the available biographies have been collected in the Dutch Biography Portal that contains especially data about different professional groups. These mostly contains people from middle-class and elite groups, but they are more varied than just artists or aristocrats but includes all people past compilers of biographical dictionaries deemed worth writing a biography about. These often included elites, but also a varied mix of heroes, administrators, ministers and artists such writers. In more modern times biographical lexicons tend to specialize on specific groups based on professions or regions (such as the RKD artists database mentioned above). Because the Biography Portal is a compilation of many different biographical lexicons, old and new, this make it possible to check the findings of the demographers in more detail and over a longer period of time. They hardly contain data about the lowest strata of society, but a mix of middle and higher strata. The basic question is whether there is a marked difference in survival rates between different groups in various periods of time.

This leads to the **assignment**

**Make a overview in tables of the life expectancy of different groups**

## The dataset

The zipped dataset is available on
https://surfdrive.surf.nl/files/index.php/s/KJx9RfbPwSOeaj6 (the file is called _datasets_dag4.zip_)

It is a selection from the data from the Biography Portal, that needs some cleanup before they can be processed into the overviews with which we will tackle the assignment. The RKD artists data have been excluded from the database in order to prevent pollution of the data with the findings from the newspaper article.

The explanation of the data elaboration is [here](./toelichting.pdf)

For your convenience we have already put up a [Google Spreadsheet](https://docs.google.com/spreadsheets/d/1LVnzU5trcKIv43FGfFMuJtAWqwCapbfanWpnmoUCEFU/edit?usp=sharing) at  with the rough data. Please note that it is read only and you have to make a copy to start editing.

## Proposed steps

For this workshop we propose the following steps for cleaning and processing the data. To work with these data, you will need tools, for our purposes any spreadsheet like program will do.

_Tools_:

    - Open Refine (http://openrefine.org/),
    - Spreadsheet (Excel, Libre Office, Google Spreadsheets),
    - programmatic (e.g. Python Pandas (https://pandas.pydata.org/)).

Use the tool you are most comfortable with, it should be able to import csv data and to make pivot tables.

### Step 1 - Conversion and cleaning

The data are in csv format, and not completely usable as is

_Cleaning_:

    - convert (cast) numbers in text format to real numbers;
    - convert datetime numbers to dates;
    - remove nulls (this is optical, but distracting in visual inspection);
    - import and check for import mistakes



**N.B.** _The dataset is an export from an SQL database with has some 'locale' problems that OpenRefine handles well but a spreadsheet program like Excel does not. For our purposes this does not matter all that much. We propose not to tackle this problem_

### Step 2 - Selection

Select the data for further processing. The dataset does not contain complete data (for instance birth and death dates) for all individuals and data are not normalized.

_decisions to make_

    - which data do we need to make the assignment
    - which alternative in dates do we choose
    - how do we choose between a maximum number of persons or more precise data


### Step 3 - Overview

Make an overview of the data:

    - make an extra column with ages
    - use your (spreadsheet-like) tool to make pivot tables of your data on ages. This will take some data mangling as grouping the pivot tables will take some manual intervention. Also take into account that a resulting table should fit on a page or a screen and that you want to communicate with it!
    - the data contain categories per person. Use these to make a more fine-grained overview.

_Issues_

  - The dataset contains evident mistakes and errors. How to deal with those?
  - There are probably also many non-evident other mistakes and errors. How to deal with these?
  - are the selections sufficient for conclusions? If not - what to do?

### Step 4 - Analysis

Analyse the data. What conclusions can we draw with regards to the assignment?

_Issues_

    - what qualifications can we make regarding our conclusions - and can they still be considered valid
    - are there any other conclusions to draw than the original research questions
    - how representative are these data

[link to spreadsheet](https://docs.google.com/spreadsheets/d/1WR5QVI96FJoZ5cWyMU1KYTbuEONrULl83V6CILCFzCY/edit?usp=sharing)
