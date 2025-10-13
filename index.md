---
title: "[Workshop] Introduction to R"
description: "Harvard FAS Informatics' multi-day introduction to R, covering R and Rstudio basics, tidyverse, and ggplot."
authors:
    - Adam Freedman
    - Danielle Khost
    - Lei Ma
    - Tim Sackton    
    - Gregg Thomas
author_header: Workshop Developers
---

# Introduction to R

{{ author_row(page) }}

This workshop aims to introduce first-time users to the [R programming language :octicons-link-external-24:](https://www.r-project.org/){:target="_blank"} and the [RStudio :octicons-link-external-24:](https://posit.co/download/rstudio-desktop/){:target="_blank"} development environment. We will provide a basic introduction to coding in R and then shift to data manipulation using the [tidyverse :octicons-link-external-24:](https://www.tidyverse.org/){:target="_blank"}, a set of R libraries designed to handle data tables in a consistent and easy way. Then, we'll learn how to generate some basic plots to explore our data using [ggplot :octicons-link-external-24:](https://ggplot2.tidyverse.org/){:target="_blank"}. You do not need any prior programming experience to take this workshop. But also note that this workshop is not a comprehensive programming class nor a comprehensive statistics class. The main goal of this workshop is to get you familiar with reading your data into R and performing basic operations and generating figures.

## Before Class

First of all, before class, it is important that you have R and RStudio installed and are able to open RStudio. These are two programs necessary for our workshop. We'll get into their details later, but for now know that R is the programming language and RStudio is the development environment from which we will run R commands.

!!! warning "R and RStudio are installed separately"

    Note that R and RStudio are different programs and need to be installed separately, with R being installed first.

### Installing R

Click on the button below to go the R project website to download and install R:

[Download R :octicons-link-external-24:](https://cloud.r-project.org/){:target="_blank" .md-button .md-button--primary .centered }

Briefly, once on the R site, click the link for your operating system to bring up a list of files to download.

For **Windows** you will want to download the **base** install files (**R-4.5.1-win.exe**).

For **Macs**, the file you download will depend on the processor in your computer.

* If you have an **M1 Mac** or higher, you will want the file **R-4.5.1-arm64.pkg**.
* If you have an older **Intel Mac**, you will want the file **R-4.5.1-x86_64.pkg**.

For **Linux**, please download the package appropriate for your distro.

After you have downloaded the file appropriate for your operating system, navigate to them and install the program as you would any other program on your computer. 

### Installing RStudio

Click on the button below to go to the RStudio website to download and install RStudio:

[Download RStudio :octicons-link-external-24:](https://posit.co/download/rstudio-desktop/){:target="_blank" .md-button .md-button--primary .centered }

Once there, scroll down and select the file appropriate for your operating system and click to download.

After you have downloaded the file appropriate for your operating system, navigate to them and install the program as you would any other program on your computer.

If you have any trouble installing these programs, or experience any errors that prevent you from completing the installation, please let us know before class by replying to the email that you got with information about this workshop.

---

### Opening RStudio

Once you have **both R and RStudio** installed, navigate to the RStudio program on your computer and open the program. This should open an interface that looks something like this: 

![RStudio interface](img/RStudio.png)

!!! important "Be sure you can successfully open RStudio before class"

    If you have any trouble opening RStudio, or experience any errors that prevent you from opening the program, please **let us know before class** by replying to the email that you got with information about this workshop.

### Installing Packages

 For Days 2-4, we will use several **packages** that may not already be installed in your RStudio environment. You can try to install them before class to troubleshoot any issues or get help beforehand. Otherwise, we will walk you through installing them in class. If you already have these packages installed, it may be beneficial to make sure they are updated to the latest version.

In general, packages can be installed from the **Packages tab**in the RStudio panel in the lower right hand corner (default location). Once you click on this tab, you will see a list of packages already installed in your RStudio environment. To INSTALL a new package, click the "Install" button on the top left corner of the panel and search for the package name. To UPDATE an already installed package, click the "Update" button, also on the top of the panel, and again search for the package name. 

#### Package requirements by workshop day

Part 1 (day 1):

* No packages required

Part 2 (days 2 & 3):

* [`tidyverse` :octicons-link-external-24:](https://www.tidyverse.org/){:target="_blank"}

Part 3 (days 3 & 4):

* [`tidyverse` :octicons-link-external-24:](https://www.tidyverse.org/){:target="_blank"}
* [`ggsignif` :octicons-link-external-24:](https://cran.r-project.org/web/packages/ggsignif/index.html){:target="_blank"}

#### Package installation - Common problems

 Installing packages can be fraught with problems because everyone has different versions of things on their own computer. We are happy to help troubleshoot with you on the day of the workshop. If you experience problems installing packages before class, try to come a few minutes early for help. Otherwise, we will help you as best we can during the workshop.

Some common problems you may encounter: 

1. The `rlang` package is a dependency for many other packages and cannot be updated from within RStudio since it is always in use. To update this package, open the R interface (NOT RStudio) and use the `update.packages()` command. Again we will be happy to help with this if it is an issue. 

2. On Windows machines, you may be prompted to install the **RTools** dependency. Note that in most cases this can be ignored since we are using common packages that don't need to be built from source. But on the off-chance this needs to be installed it is done OUTSIDE of RStudio. We will be happy to help with this if it is an issue. 

---

## Workshop content

Workshop content is available below. Download the R Markdown (.Rmd) files for each day to do the excercises. After each day, we will make available the instructor version of the R Markdown file with the solutions to the exercises.

### Day 1: Introduction to R (Part 1)

Tuesday October 14th, 9:30 am - 12:30 pm, Location: [Northwest Labs :octicons-link-external-24:](https://chsi.harvard.edu/nw_labs){:target="_blank"} room NWB 453 

* Opening RStudio and learning about its interface
* Executing R commands in the console
* Writing and running R scripts
* R objects and data types

### Day 2: Introduction to data manipulation with the tidyverse (Part 2)

Thursday October 16th, 9:30 am - 12:30 pm, Location: [Northwest Labs :octicons-link-external-24:](https://chsi.harvard.edu/nw_labs){:target="_blank"} room NWB 453 

* Installing and loading the tidyverse package
* Tibbles
* Filtering and manipulating data tables (tibbles)
* Piping

### Day 3: More tidyverse and introduction to data visualization with ggplot (Part 2 and Part 3)

Tuesday October 21st, 9:30 am - 12:30 pm, Location: [Northwest Labs :octicons-link-external-24:](https://chsi.harvard.edu/nw_labs){:target="_blank"} room NWB 453 

* Grouping and summarizing data
* Generating basic plots with ggplot
* Aesthetics and layers in ggplot
* Various plot types

### Day 4: More on ggplot (Part 3)

Thursday October 23rd, 9:30 am - 12:30 pm, Location: [Northwest Labs :octicons-link-external-24:](https://chsi.harvard.edu/nw_labs){:target="_blank"}, room NWB 453 

* More plot types
* Colors and grouping data
* Multi-panel figures

### Student notebooks

|     |     |     |
| --- | --- | --- |
| [Part 1 - Intro to R :octicons-download-24:](R-workshop-Part1-student.Rmd){ .md-button } 
<!-- | [Part 2 - tidyverse :octicons-download-24:](R-workshop-Part2-student.Rmd){ .md-button } | [Part 3 - ggplot :octicons-download-24:](R-workshop-Part3-student.Rmd){ .md-button } |-->

### Completed notebooks

|     |     |     |
| --- | --- | --- |
| [Part 1 - Intro to R :material-arrow-right:](R-workshop-Part1.md){ .md-button } 

<!--| [Part 2 - tidyverse :material-arrow-right:](R-workshop-Part2.md){ .md-button } | [Part 3 - ggplot :material-arrow-right:](R-workshop-Part3.md){ .md-button } |-->

---

<!-- --------------------------------- -->
<!-- Page speciifc CSS -->

<style>
    table thead { display: none; }
    .md-typeset table, 
    .md-typeset th, 
    .md-typeset td {
        border: none !important;
    }
    /* Remove borders from table, th, and td */

    .md-typeset__table tr:nth-child(even):hover,
    .md-typeset__table tbody tr:nth-child(even):hover {
        background-color: #f6f8fa !important;
    }
    .md-typeset__table tr:nth-child(odd):hover,
    .md-typeset__table tbody tr:nth-child(odd):hover {
        background-color: #ffffff !important;
    }
    /* Disable hover effect on table rows */

    .md-button {
        text-align: center !important;
        justify-content: center !important;
        align-items: center !important;
        display: inline-flex !important;
    }
    /* Center the text in the button */
</style>
