## Code for my personal website

This website is built with Hugo, using blogdown. This README contains some useful things to remember, because I forget how to update this website constantly.

Opening the R project in RStudio is step 1, as usual. Once that is done, the following functions are super useful:

-   `blogdown::serve_site()` to serve the site locally and see changes as you make them.

-   `blogdown::build_site(`) when finished updating the site, which builds the site into the `public/` folder so it can be deployed to GitHub Pages. The contents of this folder need to be copied into the `docs/` folder and pushed to the remote to update the website.

To edit the content of the website,

-   `data/` folder contains the .yml files with the elements on the website.

-   `themes/hugo-story/static/images` contains the images that can be inserted into the .yml files containing the content.

-   `config.yml` contains contact info, and the information that is linked in the banner, etc.

-   `themes/hugo-story/layouts/partials/publications.html` to add publications.

-   `themes/hugo-story/assets/sass/libs/_vars.scss` to change the colour of text, buttons, hover links, backgrounds, etc.

#### A note about deployment:

- The deployment to GitHub Pages is set up in the Settings of this repo. You go in Settings > Pages, and set the website to deploy from a folder on the main branch (in this case, docs/). I build the website locally using blogdown::build_site(), which puts all the files in a "public/" folder. Then, I copy the contents of that folder into "docs/" manually (not the coolest workflow, but hey - it works), push to GitHub, and the deployment workflow is triggered.

Does it all need to be this complicated? Probably not. The convoluted structure of these website files is a direct result of me working on this in a very patchy way, and an unwillingness to deviate from the template in case it all breaks down. But as they say, if it isn't broken, don't fix it (until I break this website when I update it again someday soon. And that's the fun of it!!)
