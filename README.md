# Raghav1807.github.io

## Content
This repository uses Github Pages. It contains my profile website background and blogs starting my term as an MDS student at UBC Vancouver

## Page Link
https://raghav1807.github.io/

## Instructions to Clone and Run on PC

### Step 1: Prerequisites (https://ubc-mds.github.io/resources_pages/install_ds_stack_windows/):

1. Git (https://git-scm.com/download/win), Git Bash (Enabled as default on Terminal)
2. Quarto CLI (1.10.3 or greater, I am using 1.10.18)
3. UV (0.12.3 or greater, I am using 0.12.7)
4. Python (inside UV) (3.14)
5. R (4.6.1), Rtools (For Windows) and RStudio
6. R Packages ('jsonlite', 'tidyverse', 'renv', 'usethis', 'devtools', 'markdown', 'rmarkdown', 'languageserver', 'janitor', 'gapminder', 'readxl', "ucbds-infra/ottr", "ttimbers/canlang", 'knitr')

#### Note: Commands Mentioned below with run on a single Git Bash session unless specified otherwise

### Step 2: Clone the Repository

1. Navigate to Folder in which you need the cloned repository folder
```{git bash}
cd <folder path>
```

2. Get the HTTPS URL from:
``` {markdown}
Gitub Repository > Code > Local > HTTPS > Copy the URL
```

3. Clone
```{git bash}
git clone <HTTPS URL>
```

4. Navigate to the folder
```{git bash}
cd Raghav1807.github.io
```

### Step 3: Sync the UV environment to create the Virtual Environment
```{git bash}
uv sync
```

### Step 4: Sync R Packages
```{markdown}
Open RStudio > File > Open Project > Navigate to Project Folder > Select .Rproj file > Go to Console
```

Run below command in **R console**

```{R console}
renv::restore()
```

### Step 5: Preview the site
```{git bash}
uv run quarto preview
```

**Ctrl + C** in the Git Bash session to exit the preview

### Step 6: Render the site (this renders the site into the docs folder where github picks it up)
```{git bash}
uv run quarto render
```

Double click the file 'index.html' inside the 'docs' folder to open the rendered version.

### (Only for Owner) Step 7: Push to Github after changes
```{git bash}
git add --all
```
```{git bash}
git commit -m "<Commit Message>"
```
```{git bash}
git push origin main
```

## Data Used
The Palmer Penguins dataset is used in 3 blog posts. It is loaded with the R and Python packages. No extra file stored locally or from the internet is required.

Data: [Palmer Penguins](https://allisonhorst.github.io/palmerpenguins/), Palmer Station Antarctica LTER.