## Code for my personal website

This website is built with Hugo, using blogdown. This README contains some useful things to remember, because I forget how to update this website constantly.

Opening the R project in RStudio is step 1, as usual. Once that is done, the following functions are super useful:

-   `blogdown::serve_site()` to serve the site locally and see changes as you make them.

-   `blogdown::build_site(`) when finished updating the site, which builds the site into the `public/` folder so it can be deployed to GitHub Pages. The contents of this folder need to be copied into the `docs/` folder and pushed to the remote to update the website.

To edit the content of the website,

-   `data/` folder contains the .yml files with the elements on the website.

-   `themes/hugo-story/static/images` contains the images that can be inserted into the .yml files containing the content.

-   `config.yml` contains contact info, and the information that is linked in the banner, etc.
