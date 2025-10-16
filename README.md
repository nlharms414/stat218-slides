# Accessibility Materials Project, Summer 2025

As of April 2024, a rule under Title II of the Americans with Disabilities Act (ADA) requires that all web content and mobile applications become compliant with the Web Content Accessibility Guidelines (WCAG) 2.1 Level AA. More simply put, this requires public institutions (like UNL) to ensure all web content and mobile applications can be accessed by anybody- though the main focus is ensuring that individuals with disabilities can freely access any of the previously mentioned materials. Materials meeting these guidelines are often referred to as "accessible materials".

A big part of making materials accessible lies in the underlying code. Good coding allows devices like screen readers and other assistive technologies to be effective. Thus, creating accessible web-based materials for the Statistics Department was the main focus of this project.

Ultimately, this project resulted in HTML-based slides for the Stat 218 class at UNL. A website containing all slide decks was generated that students can easily access.

## Create your own slides website!

If you'd like to customize slide decks by creating your own website, follow the steps to use this repository as a template.

\*\*Note that instructions are for use in R Studio

1.  Make sure R Studio is connected to GitHub! If this is already done, you can skip this step. If you need to connect the two, check out these more detailed [instructions.](https://happygitwithr.com/connect-intro)

2.  Clone this repository to create a local copy of its files on your computer.

3.  Go to your GitHub account and create a new repository.

4.  Create a new R Project using Git version control in R Studio and clone your newly created repository. This gives you a local copy you can edit in R Studio. The only file in this repository should be `your-repo-name.Rproj` file.

5.  Move or copy all the files from the clone of **this repository** on your computer **except for `stat218-slides.Rpoj`** to your newly created repository.

6.  Go to the 'Build' panel in R Studio and click "Render Website".

7.  Go to the 'Git' panel and commit **ALL** files. If some don't commit, you may need to do this step again with the remaining files.

8.  Now go to your repository on the web. Go to Settings \> Pages. Under the 'Branch' subheading, you'll see a couple dropdown menus. One should display "main", and the other should display "/(root)". Change the one displaying "/(root)" to "/docs". Hit "Save". It may take few minutes, but now your website should be deployed! If you refresh the page, you should now find a box at the top saying, "Your site is live at \<website url\>."

Congrats! Your website is now deployed. New changes will automatically be deployed.

### Some housekeeping items

-   Any changes to `.qmd` files will need to be rendered before the changes are committed and pushed. Otherwise, the changes will not be displayed on the website.

-   If you create a new `.qmd` file, you'll need to click "Render Website" in the 'Build' pane before rendering your changes, or the new slide deck won't show up on the website.

-   If a `.qmd` file is created within a subfolder (or new subfolder) of the `slides` folder, it will automatically display on the website. If you wish to create a new `.qmd` file in a different sublevel (or entirely new folder outside the slides folder), the `index.qmd` will need to be updated to include files from that new folder.

-   Website layout and themes can be changed from the `index.qmd` and `_quarto.yml` files, respectively.
