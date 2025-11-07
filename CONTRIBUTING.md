# 🚀 New Developer Setup Guide

This guide is for developers who want to contribute to any VitekLab project. It will walk you through setting up a local development environment to run the app from its source code.

## 1. Prerequisites 💻

Make sure you have the following software installed:

* **[R](https://cran.r-project.org/)**
* **[RStudio](https://posit.co/download/rstudio-desktop/)**
* **[Git](https://git-scm.com/downloads)**

## 2. Step-by-Step Setup

### Step 1: Clone the Repository (MSstatsShiny Example)

1.  Open your computer's **Terminal** (Mac/Linux) or **Git Bash** (Windows).
2.  Navigate to the folder where you want to store the project.
3.  Run the `git clone` command

    ```bash
    git clone [https://github.com/Vitek-Lab/MSstatsShiny.git](https://github.com/Vitek-Lab/MSstatsShiny.git)
    ```

### Step 2: Set Up the RStudio Project

1.  Open the **RStudio** application.
2.  Go to the top menu: **File > New Project...**
3.  Select **Existing Directory**.
4.  Click **Browse...** and navigate to the `MSstatsShiny` folder you just cloned.
5.  Click **Create Project**.

### Step 3: Install All Dependencies

1.  In RStudio, go to the **Console** pane.
2.  Install the `devtools` package:

    ```r
    install.packages("devtools")
    ```

3.  Run the following command to install all project dependencies:

    ```r
    devtools::install_deps(dependencies = TRUE)
    ```

> **Note:** This step can take a long time. You only need to do this once.

## 3. The Developer Workflow 🧑‍💻

This is the cycle you will follow to make and test changes.

### Step 1: Load Your Local Code

In the RStudio **Console**, run:

```r
library(MSstatsShiny)
```

### Step 2: Edit, Load, and Test!

This is your core workflow:

1.  **Edit:** Open any project file and make your code changes.
2.  **Save:** Save the file.
3.  **Install:** Go to the top right corner and click "Install" to reinstall the package.
4.  **Build:** Go to the top right corner and click "Build" to run all tests and build the package.

Repeat this **Edit > Save > Install > Build** cycle as you develop.
