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
- Since the container file is pretty big (~900 MB), I've uploaded it in the box folder (https://uofu.box.com/s/yszplfezqb0num2l30g3qiif7rb9esxc).
- You can download the `.sif` file from this link and place it in your working directory in any CHPC platform.

# Basic Usage

<img width="2400" height="810" alt="Screenshot 2025-07-15 125307" src="https://github.com/user-attachments/assets/f10c41db-ff8c-4f10-8f1b-b6c550fc478b" />

- We have now loaded the 'R' programming language insdie the container. Now we can select the packages we want to use.

# Example Use Cases
- Arules library

<img width="1744" height="1320" alt="Screenshot 2025-07-15 134803" src="https://github.com/user-attachments/assets/bd31b2e6-32a9-433b-8580-8a2908c956f9" />

- You can then use:
``` bash
# Mine association rules with minimum support and confidence
rules <- apriori(Groceries, parameter = list(supp = 0.01, conf = 0.2))

# Inspect top 5 rules sorted by lift
inspect(sort(rules, by = "lift")[1:5])
```
<img width="2124" height="1264" alt="Screenshot 2025-07-15 135700" src="https://github.com/user-attachments/assets/c3699514-a8f0-46ab-8449-33589e1e1374" />

# Future Work
- If you'd like to modify this container—such as adding packages or updating versions—you can use the attached `.def` file. Simply make your changes there and build a new `.sif` file with the updated packages.
---

## Contact

If you have any questions, feel free to reach out:

**Sukrut Shishupal**  
PhD Student  
Department of Biomedical Informatics  
University of Utah  
Salt Lake City, UT 84112-5880   
📧 [sukrut.shishupal@utah.edu](mailto:sukrut.shishupal@utah.edu)  
🌐 [sukrut-shishupal.github.io](https://sukrut-shishupal.github.io)
