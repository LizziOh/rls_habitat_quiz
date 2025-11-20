RLS_habitat_quiz

Flashcard-style identification practice and quiz app in R.
Reads your photos from simple folders (per location → per species), launches a Shiny app, and (optionally) records quiz scores.

✨ What it does

Practice mode: big photo, four chunky options, instant feedback.

Quiz mode: fixed number of questions (default 20) with a score screen.

Zero data wrangling: just put photos in folders; names become labels.

Multiple locations/projects: add a new top-level folder, no code changes.

Supports jpg, jpeg, JPEG, png, webp. Requires ≥ 4 species per location.

# Install remotes if not already installed
install.packages("remotes")

# Install the RLS Habitat Quiz package from GitHub
remotes::install_github("LizziOh/rls_habitat_quiz")

# Load the package
library(rls_habitat_quiz)

# Launch practice mode (default folder: "rls_catalogue")
rls_practice()

# Launch quiz mode with 20 questions
rls_quiz("rls_catalogue", n = 20)

# Optional: save a CSV summary of results
quiz("rls_catalogue", n = 20, save_csv = TRUE, csv_path = getwd(), user = "YOURNAMEHERE")



