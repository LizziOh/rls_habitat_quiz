RLS Habitat Quiz

A flashcard and quiz app to learn Reef Life Survey habitat labels in R

This reads your photos from simple folders (per labelling scheme → per label), launches a Shiny app, and (optionally) records quiz scores.

Forked from: coralquiz by Matthew Doherty:  https://github.com/dohertyml/coralquiz
This version has been adapted to include RLS images, new folder structure, and renamed functions.


Users can adapt this without code changes by adding a new top-level folder containing other labels to learn and their images.

Supports jpg, jpeg, JPEG, png, webp. Requires ≥ 4 species per location.

Installation
------------------
Install remotes if not already installed:
install.packages("remotes")

Install the RLS Habitat Quiz package from GitHub:
remotes::install_github("LizziOh/rls_habitat_quiz")

Usage
------------------
Load the package:
library(rls_habitat_quiz)

Launch practice mode (default folder: "rls_catalogue"):
rls_practice()

Launch quiz mode with 20 questions:
rls_quiz("rls_catalogue", n = 20)


Adding new image folders
------------------
Add folders under inst/app/www/photos/<source>/<species>/images
Each <source> folder will be recognized automatically


Acknowledgements
------------------
Original coralquiz package by Matthew Doherty
Thanks for sharing the coralquiz framework that we adapted for Reef Life Survey habitats.
