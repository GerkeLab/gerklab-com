---
title: "So You'd Like to Make an R Package?"
author: Garrick Aden-Buie
date: 2018-07-03
categories: ["R", "R Package", "R Development"]
description: A guide and workflow for planning your next R package.
toc: no
hero_bg: "/img/hero/leone-venter-469710-unsplash.jpg"
---


[cran]: https://www.r-project.org/
[bioc]: https://bioconductor.org/
[github]: https://github.com/

## Introduction

The goal of this document is guide planning and collaboration when initiating the development of a new R package.

High-quality and user-friendly R software is an important and complementary aspect of producing and disseminating impactful research.
The R programming language provides a standardized structure for bundling software, data, and documentation that allows for the software to be distributed as a cohesive package through online repositories such as [CRAN][cran], [BioConductor][bioc], [GitHub][github], and others.


## What problem does your package solve?

This is the "problem statement" for your package.
A good package solves a problem faced by its users.
The problem solved by the package can range from accomplishing a task that is otherwise difficult or time-consuming, or providing access to new statistical methods, or making available the code and data used in a research article.

Think about the following questions and answer any that apply to your package:

1. Does this package make an otherwise tedious task easier? Describe the task and its challenges.

1. Will this package provide custom algorithms, methods or data?

1. Do other packages exist to help with the problem described above?

    - List any relevant packages in this problem area.

    - In what ways are they similar or different to this package?

    - Are any of the related packages open to collaboration? Is this package significantly different from the others, or would it make sense to build on a related package?

    - If the functionality of a related package overlaps with this package, how will your package differentiate itself from the others? Will the interface be easier to use or more comprehensive, etc.?
    
At this point, take a good, critical look at the ecosystem for your potential package.
Will your package occupy a clearly defined area of this space?
Will it link functionality among other packages?
Is there room for improvement in the existing packages?

It's okay at this step to decide not to make a package.
Your code and ideas can still be useful to others as a blog post or white paper that you can share on Twitter, GitHub or your personal website.

## What functionality will your package contain?

After defining the problem solved by your package and establishing an understanding of where your package fits into the R software ecosystem, the next step is to decide exactly what functionality your package will provide to its users.

There are two key ingredients to consider at this stage:

1. Your package should be compatible with the established workflows of your users.

1. Simple interfaces are best.

### User Workflow

If your package solves a problem for its users, then you also have a particular user group in mind (the kind of users that have the problems you want to solve).

1. What typical workflows lead to the problem at hand? Outline the steps that lead up to the point that a user would use your package and then the steps that occur afterwards.

1. In particular, what format will be expected or required of inputs -- data files, images, etc. -- and outputs -- R objects, data files, reports, etc.

### User Interface

When thinking about the functionality of your package, it's important to avoid being overly ambitious.
A simple and consistent user interface will allow your users to rely on and trust your package and when combined with thoughtful integration with the user's workflow you allow users to build on the best solutions available for each step in their workflow.

This concept is reminiscent of the [Unix philosophy](https://en.wikipedia.org/wiki/Unix_philosophy): short, modular code is easier to maintain and pair with other software.

1. What are the core features (functions) of your package? 

    Each feature should follow this template: *A function that ...*

1. Which of these features are **essential** to your package, and which are extra or "nice to have"?

1. Which of these features **need to be present** for your package to work (e.g. for the initial release) and which features can be developed later in the process?

## What will your package be called?

Choosing a name for your package is an important part of development cycle because the name will embody all of the aspects outlined above while serving to advise the first impressions your users will have of the package. A good name sets expectations and serves as a valuable marketing tool.

Package names

- can only consist of letters, numbers and periods
- must start with a letter
- cannot end with a period
- cannot include `-`, `_`, or spaces.

Lowercase, single word package names are recommended.
For two word package names, you can use camelCase.
Hadley Wickham's [R Packages](https://r-pkgs.had.co.nz/) book contains a useful section on [Naming your package](https://r-pkgs.had.co.nz/package.html) for more information.

Finally, use the R package [available](https://github.com/ropenscilabs/available) to search for existing packages and to ensure that the name you choose is... _available_.

## The future of your package

If all goes according to plan, your package will someday become a reality.
At that point, you need to decide how and where your package will be released. Once it has been released, you'll also need to decide how much support for maintenance you'll be willing to provide. Note that actively developed packages have a greater impact on the community at large.

As a package owner, you may choose from the following options:

- Release the package to [GitHub][github] or another online repository. Users will be able to view the source code, report issues, and contribute code. Installation is possible, but less straightforward than the following options. A package released only to GitHub (or other repo) will have somewhat lower visibility and discoverability.

- Release the package to [CRAN][cran] (as well as an online repository like GitHub). Installation and discoverability is much easier for users, but more work is required by the developers to prepare for releasing the package on CRAN.

- Release the package to [BioConductor][bioc] (as well as an online repository). Again, installation and discoverability are significantly easier for users, in particular for R users in the areas of bioinformatics and genomics. Developer investment in preparation of release is similar in difficulty to a release on CRAN, although the process is [slightly different for BioConductor](https://bioconductor.org/developers/package-submission/) where higher requirements are established for the documentation that accompanies the package among other areas.

- Release on CRAN, BioConductor and GitHub.

Additionally, you may wish to accompany the release of your package with a paper.
Venues for this paper may include [bioRxiv](https://www.biorxiv.org/), [The R Journal](https://journal.r-project.org/), the [Journal of Statistical Software](https://www.jstatsoft.org/index), the [Journal of Open Source Software](https://joss.theoj.org/), and other academic journals such as [Bioinformatics](https://academic.oup.com/bioinformatics/).

Finally, who will maintain the software once it is released?


## Checklist

Answer all of these questions to complete the **Package Planning Checklist**.

### Problem Statement

1. Describe the central task of this package and its challenges.

1. Will this package provide custom algorithms, methods or data?

1. Do other packages exist to help with these problems?

    - List any relevant packages in this problem area.

    - In what ways are related packages different from your package?
    
    - In what ways do related pacakges overlap?

    - How will your package differentiate itself from the others?
    
### User Workflow

1. What typical workflows lead to the problem at hand? Outline the steps that lead up to the point that a user would use your package and then the steps that occur afterwards.

1. In particular, what format will be expected or required of inputs -- data files, images, etc. -- and outputs -- R objects, data files, reports, etc.

### User Interface

1. What are the core features (functions) of your package? 

    Each feature should follow this template: *A function that ...*

1. Which of these features are **essential** to your package, and which are extra or "nice to have"?

1. Which of these features **need to be present** for your package to work (e.g. for the initial release) and which features can be developed later in the process?

### Packaging Your Package

1. What will your package be called?

1. Where will it be released? (CRAN, BioConductor, GitHub, etc.)

1. Will the release include a paper, and if so where will the paper be published?

1. Who will maintain the package and for how long?
