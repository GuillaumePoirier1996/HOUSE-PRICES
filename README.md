<div>
    <img src="src/img/maison.png" alt="House Logo" title="House pricing work" align="right" width="40" />
</div>

# House Pricing Work

<div align="center">
    <img src="src/img/banner.png" alt="Banner Project" title="Banner Project" width="65%" />
</div>

⭐ Star me on GitHub — it motivates me a lot!

[![html renderer](https://img.shields.io/badge/html%20renderer-myst-pink)](https://mystmd.org/guide)
[![language](https://img.shields.io/badge/language-python-yellow)](https://wiki.python.org/moin/BeginnersGuide/Programmers)
![OS](https://img.shields.io/badge/OS-linux%2C%20windows%2C%20macOS-0078D4)
[![GitHub release](https://img.shields.io/github/v/release/GuillaumePoirier1996/HOUSE-PRICES)](#)
[![GitHub release date](https://img.shields.io/github/release-date/GuillaumePoirier1996/HOUSE-PRICES)](#)
[![GitHub last commit](https://img.shields.io/github/last-commit/GuillaumePoirier1996/HOUSE-PRICES)](#)
[![Total Downloads](https://img.shields.io/github/downloads/GuillaumePoirier1996/HOUSE-PRICES/total.svg)](#)

[![Share](https://img.shields.io/badge/share-000000?logo=x&logoColor=white)](https://x.com/intent/tweet?text=Discover%20my%20GitHub%20project:%20https://github.com/GuillaumePoirier1996/HOUSE-PRICES%20%23DataScience%20%23MachineLearning%20%23Python)
[![Share](https://img.shields.io/badge/share-1877F2?logo=facebook&logoColor=white)](https://www.facebook.com/sharer/sharer.php?u=https://github.com/GuillaumePoirier1996/HOUSE-PRICES)
[![Share](https://img.shields.io/badge/share-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/sharing/share-offsite/?url=https://github.com/GuillaumePoirier1996/HOUSE-PRICES)
[![Share](https://img.shields.io/badge/share-FF4500?logo=reddit&logoColor=white)](https://www.reddit.com/submit?title=Check%20out%20this%20project%20on%20GitHub:%20https://github.com/GuillaumePoirier1996/HOUSE-PRICES)
[![Share](https://img.shields.io/badge/share-0088CC?logo=telegram&logoColor=white)](https://t.me/share/url?url=https://github.com/GuillaumePoirier1996/HOUSE-PRICES&text=Check%20out%20this%20project%20on%20GitHub)

🔥 In this little repo, you're gonna find some fantasies about a big topic : 🏠 the property business 🏠

## Table of Contents

- [Summary](#-summary)
- [Getting Started](#-getting-started)
- [License](#-license)
- [Contacts](#%EF%B8%8F-contacts)

## 📝 Summary

Welcome to this repository❗Here, you'll find code and resources focused on real estate. During a period of professional downtime, I decided to channel my thoughts into a subject that interests me deeply and affects us all. For more context, feel free to check out [this document](src/utilities/00-presentation.md) (written in French for now 👎), which provides an insightful and humorous overview of the project's background and initial ideas👌. Below is a quick summary of the repository's structure:

- **Kaggle Project**: A few years ago, I embarked on my first Kaggle project: the House Pricing Model, a competition dating back to the 2010s. After spending a year collaborating with data scientists at MAIF, I decided to revisit this project. The goal was to code and implement my ideas while reflecting on and sharing the progress I've made since my early days. Learn more about the competition on its [Kaggle page](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/overview).

- **Web Scraping and Data Collection on French Real Estate**: This section focuses on developing several programs to scrape data from various websites featuring real estate listings in France, particularly in the Charente-Maritime region.

- **Fair Pricing**: The final section addresses a key question: how can we regulate real estate prices to ensure fair pricing per square meter while managing market price increases effectively?

## 🚀 Getting Started

All the notebooks works with python (3.12). I hesitated a bit to use poetry for all dependencies but i opted for a simple solution : use an environment.yml file and code with a conda environment for more simplicity. To visualize the repo, i suggest you to use myst and build a html page to navigate easely. all you have to do is :

### 1. Clone the repo

To work locally on your computer, navigate to the directory you want. Open a terminal and run the following command:

```shell
# Open a terminal (Command Prompt or PowerShell for Windows, Terminal for macOS or Linux)

# Ensure Git is installed
# Visit https://git-scm.com to download and install console Git if not already installed

# Clone the repository
git clone https://github.com/GuillaumePoirier1996/HOUSE-PRICES.git
```

### 2. Recreate the right environment

If you want to run all with no trouble, I suggest you to run the following command:

```shell
# Navigate to the project directory
cd house-prices

# Ensure conda is installed
# Visit https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html to download and install conda if not already installed

# Create the environment
conda env create -f environment.yml

# Activate it, to deal with all dependencies and libs
conda activate house-prices-env
```

### 3. Explore, as you want

If you like the tree structure and organization of the project you can run and explore it as you wish. But if like me, you want a structure and a visualization like a web article, I can advise you to build an html page with myst and appreciate the organization in this way :

```shell
# if it's not already done navigate to the project directory
# you have to be in the root path (the base of the project)
cd house-prices

# Ensure node.js is installed
# Visit https://docs.npmjs.com/downloading-and-installing-node-js-and-npm to download and install node.js if not already installed

# Initialize myst, at the root path (where the myst.yml file is)
myst init
```

Normally, you're gonna see this :

![myst-question](/src/img/would-you-like-to-start-myst.png)

You just have to answer 'Y'. then you will have this in your command prompt :

![myst-generated-html](/src/img/myst-generated-html.png)

🛠 Open your web browser by clicking on the link (your can be an other one, so don't panic) and enjoy. If you want you can save the website, by doing this :

```shell
myst build --html
```

I let you focus on the documentation of Myst for more detail. Everything is explained [here](https://mystmd.org/guide).

### 4. Pre-commit, just in case

One day, if you want to help me improve things, I just want to warn you. If you want to commit changes, you'll need to write this command in a prompt, with the environment activated :

```shell
# house-prices-env already activated
Pre-commit install
```

Change the pre-commit-config.yaml file. If you're using macOS or Linux, just uncomment like this:

```yaml
repos:
  - repo: local
    hooks:
      - id: update-environment
        name: Mise à jour de environment.yml
        # Pour Windows
        # entry: powershell -Command "
        #   conda activate house-prices-env;
        #   conda env export --no-builds --file environment.yml"
        # Pour Linux/macOS
        entry: bash -c "source $(conda info --base)/etc/profile.d/conda.sh;
        conda activate house-prices-env;
        conda env export --no-builds --file environment.yml"
        language: system
```

## 📃 License

This project is licensed under the MIT License.

Copyright (c) 2024 Guillaume Poirier

You are free to use, copy, modify, merge, publish, distribute, sublicense, or sell copies of this software under the terms of the MIT License.

A full copy of the license is included in the repository's [LICENSE](/LICENSE.md) file.

## 🗨️ Contacts

For more details about my work or any general information, feel free to reach out to me. I'm here to provide support and answer any questions you may have. Below are the best ways to contact me:

<div style="display: flex; justify-content: center; align-items: center; gap: 30px;">
    <a href="tel:0785548643">
      <img src="src/img/tel.png" alt="Téléphone">
    </a>
    <p>+33 7 85 54 86 43</p>
    <a href="mailto:guillaume.poirier1996@gmail.com">
      <img src="src/img/mail.png" alt="Email">
    </a>
    <a href="https://www.linkedin.com/in/guillaume-poirier-41231713a/">
      <img src="src/img/linkedin.png" alt="Linkedin">
    </a>
</div>

Don't hesitate if you want to work with me, I'm steel looking for a job 😂😂.

[Back to top](#top)
