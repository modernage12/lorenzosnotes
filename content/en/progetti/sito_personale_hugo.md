+++
title = "Personal Site with Hugo Framework"
date = 2025-04-27T13:55:00+02:00 # Initial or updated date
draft = false
weight = 50 # Or the weight you prefer for ordering
tags = ["Hugo", "Website", "Portfolio", "GitHub Pages", "GitHub Actions", "Paige Theme", "Static Site", "Google Analytics"] # Added GA
# Let's hide metadata/etc for consistency
[paige.pages]
  disable_keywords = true
  disable_date = true
  disable_word_count = true
  disable_reading_time = true
  disable_toc = true
+++

This is the project for the creation and continuous development of my personal website/portfolio, the digital space you are in now! It was built using the static site generator **Hugo** and the **Paige** theme.

### Objective:
To create an online space to present myself more completely than a traditional CV, showing work and educational experiences, personal projects, interests, and skills in a dynamic and authentic way.

### Technologies and Tools Used:
* **Static Site Generator:** Hugo (v0.141.0 Extended)
* **Theme:** Paige (integrated as a Git Submodule)
* **Content Language:** Markdown with TOML Front Matter
* **Hosting:** GitHub Pages (configured for free deployment)
* **Automatic Deployment:** GitHub Actions (custom workflow with `peaceiris/actions-gh-pages` for build and push to `gh-pages` branch)
* **Build Dependencies:** Dart Sass (installed in the Actions workflow to compile the theme's SCSS)
* **Version Control:** Git and GitHub
* **`Analytics: Google Analytics (GA4) for monitoring visits and user behavior.`**

### What I Learned and Challenges Overcome:
This project has been an excellent training ground for delving into various aspects of web development and modern workflow:
* **Advanced Hugo Configuration:** Managing `hugo.toml`, `baseURL`, theme parameters ([params.paige], [params.paige.site], [params.paige.subpages]), custom menus, `weight` management for sorting.
* **Content Management:** Structuring in sections (`content/`), using `_index.md`, customizing Front Matter for individual pages and sections (e.g., hiding metadata/ToC).
* **Theme Customization:** Overriding theme partials (e.g., `head.html` for GA, `site-footer-last.html` for social links) to insert custom functionalities while keeping the main theme updatable.
* **Static Asset Management:** Using the `static` folder for files like the CV PDF.
* **Automated Deployment:** In-depth configuration and debugging of GitHub Actions, experimenting with different workflows (actions/deploy-pages vs `peaceiris/actions-gh-pages`), managing permissions (`contents: write`), and resolving build dependencies in the Actions environment (Hugo versions, Dart Sass installation).
* **`Analytics Integration: Manual implementation of the Google Analytics (GA4) snippet (via override of the Hugo/Paige 'head.html' partial) with the goal of tracking site visits, analyzing user journeys, and collecting aggregated data on the usage of different sections.`**
* **Problem Solving:** Addressing and resolving 404 errors (broken links, incomplete deployment), build errors (Hugo/Theme incompatibility, Sass dependencies), permission errors on GitHub Actions.
* **Basic HTML/CSS Usage:** Inserting inline HTML (CV link, social icons) and basic styles through theme parameters.

### Current Status:
The site is **currently online** on GitHub Pages and is automatically updated with every `push` to the `master` branch of the GitHub repository. It is continuously evolving with the addition of new content and projects.

*(Link to Repository: [github.com/modernage12/lorenzosnotes](https://github.com/modernage12/lorenzosnotes) - you can add it if you want)*