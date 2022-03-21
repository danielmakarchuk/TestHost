# Hello World

# Hosting a Resume on GitHub Pages 

## Purpose:
---
This readme teaches the key principles found in Etter’s book Modern Technical Writing: An Introduction to Software Documentation by Andrew Etter.  These principles are demonstrated through the hosting of a Resume on GitHub Pages.

## Prerequisites:
---
*	Have a GitHub account.
*	know the basics of how to work with GitHub.
*	know how to write in markdown (CommonMark or GitHub flavoured)


## Instructions
---
### Setup
---

To make a static website as Etter encourages you must have a location to host the site.  The Distributed Version Controle site GitHub provides a great location to host such sites.  It allows for easy modification, version controle and allows users to do offline edits.

1.	Log into the GitHub account you want the resume hosted at.
2.	Create a new repository named: GitUsername.GitHub.io.

This repository will be used to create and host a static website.
### Creating the Resume
---
Etter describes various advantages of lightweight markup languages such as markdown.  Markdown can easily be turned into good XML.  This XML is necissary to generate static websites.  

3. Create a .md file called index.md.
   *  Create index.md in GitHub, or,
   *  Clone the repository and create index.md locally.
4. Write your Resume in markdown in the index.md file.
5. Add index.md into the GitUsername.GitHub.io repository.
   * If written on GitHub commit the changes.
   * If written locally commit the changes and push the repository.

The resume in index.md will be the contents of the static website.

### Hosting the Resume Website on GitHub Pages
---
Etter likes static websites.  They offer a robust and secure way of hosting your resume.  So long as GitHub is up the resume will be up.  

6. Create a new file in the GitUsername.GitHub.io repository and name it _config.yml.
7. For the slate theme copy and paste the below code into _config.yml.

```
remote_theme: pages-themes/slate@v0.2.0
plugins:
- jekyll-remote-theme
```
8. Commit the changes to _config.yml. to Github.
9. Check the header directly above the repositories files.
   *  If a green checkmark appears the build  proceed to the next step.

   *  If an orange dot is present wait about five minutes and check again.
   *  If a red x apears
       * **a.**	Check the _config.yml file for typos.
         * 	If a typo is found, fix it and re-build the website.
         *  If no typo is found, try step b.
       * **b.**	Check the README.md for the chosen [GitHub](https://pages.github.com/themes/) theme in the _config.yml file.
         * 	Compare the documentation’s recommended code to the code in _config.yml.  
         *  If different, replace the _config.yml code with the code in the documentation.
       * **c.**	Go back to step 8.
10. Search for your website.
    *  type GitUsername.GitHub.io into the address bar.
    *  as seen in the below animated GIF.

![a demo for finding your cite](https://github.com/danielmakarchuk/danielmakarchuk.GitHub.io/blob/main/SiteSearch.gif)

Static websites are also easy to update.  Simply make a change in index.md and rebuild the cite.  The changes should appear after the rebuild.

If unsatisfied by the themes GitHub automatically supports check out Jekyll. The process is more complecated then the one described above.  The Jekyll documentation will walk you through how to use it.
## More Resources
---
1. [A markdown tutorial](https://www.markdowntutorial.com/)
2. [Etter's Book: Modern Technical Writing](https://www.amazon.ca/gp/product/B01A2QL9SS/ref=ppx_yo_dt_b_d_asin_title_o00?ie=UTF8&psc=1)
3. [Jekyll themes GitHub automatically supports](https://pages.github.com/themes/)
4. [Jekyll](https://jekyllrb.com/)


## Authors and Acknowledgments:
---
*   My groupmates: Nitya Seth, Alex Kitt, James Watts, and Jarett Koley, who helped me improve this readme.
*   [The creator of the Template I used for this README:](https://github.com/PurpleBooth/a-good-readme-template) **PurpleBooth**, Billie Thompson.

## FAQ
---
1. Why is Markdown better than a word
processor?
   * markdown and can be quickly and efficiently turned into XML which is required to generate static websites.  To host a Word file you would have to translate it into lightweight markup (like markdown) before turning it into a website.  Writing in markdown you remove a step from the process.

2. Why is my resume not showing up?
   * Sometimes GitHub does not automatically apply updates.  Most updates are applied within twenty minutes of completion.  Though when overloaded GitHub may take upwards of an hour to apply the changes.

