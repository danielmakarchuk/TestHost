# Hosting a Resume on GitHub Pages 

## Purpose:
---

This README Describes the practical steps of how to host a resume on GitHub Pages.  While doing so it also teaches the key principles found in Andrew Etter's book Modern Technical Writing: An Introduction to Software Documentation.

## Prerequisites:
---
*	Have a GitHub account.
*	Know the basics of how to work with GitHub (push, pull, commit).
*	Know how to write in markdown (CommonMark or GitHub flavoured).


## Instructions
---
### Setup
---

To make a static website as Etter encourages, there must have a location to host the site from.  The distributed version control site GitHub is a great location to do so at.  GitHub allows for easy modification, allows users to do offline edits, and offers version control.  All advantages Etter discusses in his book.

1.	Log into the GitHub account you want the resume hosted at.
2.	Create a new repository named: GitUsername.GitHub.io.
    * You only get one public website on GitHub.  If you are already hosting a site, use a different github account or delete the repository holding the old website.

After step 2 you should have on your Github account a repository named GitUsername.GitHub.io.

This repository will be used to create and host a static website for the resume.
### Creating the Resume
---
Etter describes various advantages of lightweight markup languages such as markdown. One advantage is that markdown can easily be turned into good XML.  This XML is necessary to generate static websites.  This is important for when you want to convert a document like your resume into a static website.

3. Create a .md file called index.md.
   *  Create index.md in GitHub, or,
   *  Clone the repository and create index.md locally with your editor of choice (Typora, Atom, Visual Studio Code, etc.).
4. Write your Resume in markdown in the index.md file.
5. Add the index.md file into the GitUsername.GitHub.io repository.
   * If written on GitHub, commit the changes into the GitUsername.GitHub.io repository.
   * If written locally:
      * Commit the changes and push to the itUsername.GitHub.io repository, or,
         * **a.** Copy the markdown into index.md in the GitUsername.GitHub.io repository.
         * **b.** Commit the changes in the GitUsername.GitHub.io repository.

After step 5 you should have in the GitUsername.GitHub.io repository a file named index.md containing your resume written in markdown.

This resume in index.md will be the contents of the static website.



### Hosting the Resume Website on GitHub Pages
---
Etter likes static websites.  They offer a robust and secure way of hosting your resume.  So long as GitHub is up the resume website will be up.  

The following steps describe how to create the resume website with GitHubs slate theme.  If another theme is wanted, follow the link to all themes supported by GitHub in more resources. 

6. Create a new file in the GitUsername.GitHub.io repository and name it _config.yml.
7. For the slate theme copy and paste the below code into _config.yml.

```
remote_theme: pages-themes/slate@v0.2.0
plugins:
- jekyll-remote-theme
```
8. Commit the changes to _config.yml. to Github.
9. Check the header directly above the repository's files.
   *  If a green checkmark appears the build  proceed to the next step.

   *  If an orange dot is present wait about five minutes and check again.
   *  If a red x appears
       * **a.**	Check the _config.yml file for typos.
         * 	If a typo is found, fix it and re-build the website.
         *  If no typo is found, try step b.
       * **b.**	Check the README.md for the chosen [GitHub](https://pages.github.com/themes/) theme in the _config.yml file.
         * 	Compare the documentation’s recommended code to the code in _config.yml.  
         *  If different, replace the _config.yml code with the code in the documentation.
       * **c.**	Go back to step 8.
10. Search for your website.
    *  type GitUsername.GitHub.io into the address bar.
    *  The below animated GIF demonstrates how to search for your website.

![a demo for finding your cite](https://github.com/danielmakarchuk/danielmakarchuk.GitHub.io/blob/main/SiteSearch.gif)

After step 10 you should be able to see your resume hosted as a static website.

* If unsatisfied by the themes GitHub automatically supports check out Jekyll. The process is more complicated than the one described above.  The Jekyll documentation will walk you through how to use it.

### Updating the Resume
Another reason Etter likes static websites is because they are easy to update.  Simply make a change in index.md and rebuild the cite.  The changes should appear after the rebuild.

11. Edit the index.md.
    *  If edited on GitHub, commit the change.
    *  If edited locally, commit then push the change.
12. Go to step 9.

After step 12 you should be able to see the changes to your resume on the static website.
## More Resources
---
1. [A markdown tutorial](https://www.markdowntutorial.com/)
2. [Etter's Book: Modern Technical Writing](https://www.amazon.ca/gp/product/B01A2QL9SS/ref=ppx_yo_dt_b_d_asin_title_o00?ie=UTF8&psc=1)
3. [Jekyll themes GitHub automatically supports](https://pages.github.com/themes/)
   * To find the code needed for _config.yml.
       1. Follow the link to the wanted theme's GitHub page.
       2. Read the GitHub pages README.md.
4. [Jekyll](https://jekyllrb.com/)


## Authors and Acknowledgments:
---
*   My groupmates: Nitya Seth, Alex Kitt, James Watts, and Jarett Koley, who helped me improve this readme.
*   [The creator of the Template I used for this README:](https://github.com/PurpleBooth/a-good-readme-template) **PurpleBooth**, Billie Thompson.

## FAQ
---
1. Why is Markdown better than a word
processor?
   * markdown and can be quickly and efficiently turned into XML which is required to generate static websites.  To host a word file, it would have to be translated it into lightweight markup (like markdown) before turning it into a website.  Writing in markdown removes a step from the process of hosting a static website.

   * In the world of computer science lightweight markup languages like markdown are used in documentation.  By using markup instead of a word processor, skills potential employers may be impressed by are displayed.

1. Why is my resume not showing up?
   * Sometimes GitHub does not automatically apply updates.  Most updates are applied within twenty minutes of completion.  Though when overloaded GitHub may take upwards of an hour to apply the changes.
