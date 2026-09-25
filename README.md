# eshadhi.github.io

## Eshadhi's Quarto Website
This repository contains my personal Quarto website, with pages about myself and my recent blog posts. In my blog posts you will find two computational posts that use R and Python to analyze the Palmer Penguins dataset.

## Installations

To build this website, you will need to install the following software first:
    Quarto — version 1.10.18
    R — version 4.6.1
    uv — version 0.12.7

The R project uses renv to manage its packages. The required R packages can be restored from renv.lock.

The Python project uses uv to manage its packages. The required Python packages are listed in pyproject.toml and locked in uv.lock.

## Clone the repo

In your terminal got to a folder of your choosing, clone the repo:

git clone https://github.com/Eshadhi/eshadhi.github.io.git

Go into your folder:

cd eshadhi.github.io

## Setting up R and Python

From inside your the top-level repository folder, run:

uv sync

renv::restore()

## Render Website

To open the website locally, run the following commands from your top-level repository folder:

uv run quarto render

uv run quarto preview

## Data

The data used in my blog posts can be found here: 

Data: [Palmer Penguins](https://allisonhorst.github.io/palmerpenguins/),
Palmer Station Antarctica LTER.

The dataset does not need to be downloaded from a URL each time the website is rendered, as it is download through the R and Python index.qmd.
Website contents

## Website Content

    A home page with information about me.

    An About page with more information about my background and interests.

    A Blog page containing my posts.

    An R computational post analyzing penguin flipper length by species and sex.

    A Python computational post analyzing the same data.
