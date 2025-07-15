# R-container

A Singularity/Apptainer container with R 4.4.2 and essential packages for sequence analysis, association rules, and clustering.

# What's Included
This container is built on rocker/tidyverse:4.4.2 and includes:

| 📦 Core R Packages | 🔍 Data Mining & Analysis | 🗄️ Database & Utilities |
|--------------------|---------------------------|--------------------------|
| tidyverse          | arules                    | RSQLite                  |
| dplyr              | arulesSequences           | lubridate                |
| ggplot2            | TraMineR                  |                          |
| shiny              | cluster                   |                          |
| rmarkdown          | dtw                       |                          |
| knitr              | mlr3                      |                          |
| plotly             | TSP                       |                          |


# Downloading the container 
- Option 1: Build from definition file
```bash
# Clone the repository
git clone https://github.com/sukrut-shishupal/R-container.git

# Load Apptainer module
module load apptainer

# Navigate into the project directory
cd R-container
```

- Option 2: Download pre-built container 
wget <direct-download-url>/package-r.sif

# Basic Usage

<img width="2400" height="810" alt="Screenshot 2025-07-15 125307" src="https://github.com/user-attachments/assets/f10c41db-ff8c-4f10-8f1b-b6c550fc478b" />

- We have now loaded the 'R' programming language insdie the container. Now we can select the packages we want to use.

# Example use cases
- 
