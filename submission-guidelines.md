---
title: Submission guidelines
layout: default
description: How to contribute to the newsletter
---
## Scope
The scope of the newsletter include all topics covered by the [Modelica Association](https://www.modelica.org) (Modelica language, libraries, FMI, SSP), related tools and news in education (courses, books and related materials).

## Process
Everyone is welcome to contribute a post to the Modelica newsletter, however the editor holds the right to decline a contribution without reason. The submission is done by creating a pull request to the dedicated newsletter repository.
{% if site.contribution-open %}

The submissions are currently open! The deadline for contributions to the current issue is **{{ site.contribution-deadline }}**. The newsletter would be published on **{{ site.current-newsletter-date }}**.

0. Create a GitHub account, log in.
1. Navigate to the [newsletter repository]({{site.current-contribution-url}}) - it is important to keep your contribution within the folder with the current issue, e.g. `_2018-01`. Contributions to other folders would be discarded.
2. Click Create new markdown file, e.g. *my-new-post.md* (the file extension is important)
3. Insert your post. You can reuse the example below or inspire yourself from other posts in the [folder]({{site.current-contribution-url}}). 
4. Commit changes. 
   * Note, that no changes has been made to the [newsletter repository]({{site.current-contribution-url}}) itself. Instead, GitHub created your own copy (*a fork*) of the repository with your changes. 
   * If you already have this repository forked, you may create a new branch from the original repository.
   * If you want to modify your contribution or add a local image, you have to navigate to this branch of your fork (e.g. patch-1) and make the desired changes or upload an image. You can then create a pull-request. This would issue a request to merge your whole branch - that is all changes you have made - to the original repository.
5. Create a pull-request
   * Please let the *Allow the maintainers edit...* checked, so we can fix any potential issues for you.
6. Submit the pull request -- all done.

Please note, that all your contributions are public from the beginning for anyone who knows the (public) repository. If you insist on having the contribution private prior to the release, please [let me know](mailto:filip.jezek@creativeconnections.cz).

  {% else %}

*The contributions are closed right now*

{% endif %}

## Structure
Each post should start with a header information, starting and ending with a line with three slashes '---'. Then, three meta-information shall be inserted:
- `title` - a short title. Can be nested into quotes to prevent special characters (e.g. colons) from breaking the text.
- `author` - authors of the contribution and their affiliations, preferably including hyperlinks, e.g. `[Modelica Association](http://modelica.org)`
- `category` - a category of the post. Currently, following four categories are currently accepted. However, if you feel, that your contribution does not exactly fit one of those, we might open a new category. Just [let us know](mailto:filip.jezek@creativeconnections.cz).
  - `"association"` - news regarding Modelica association
  - `"education"` - news regarding educational resources, or training  
  - `"library"` - news regarding new or improved libraries
  - `"vendor"` - news regarding new Modelica tools versions
  
## Markdown syntax   
For the text body, use the [kramdown](https://kramdown.gettalong.org/) flavor of the Markdown syntax. See the [quick reference](https://kramdown.gettalong.org/quickref.html). It is *mostly* compatible with the GitHub flavored markdown. 

### Paragraphs
Simple line break 
in the source would not create separate paragraphs. Please use empty line between intended paragraphs instead. When a hard line-break is required, you may use four spaces `    ` at the end of the line.

    First paragraph

    Second paragraph    
    with hard break - note the four spaces at the end of the upper line

### Text style
You can use **emphasize** by double asterisks (`**emphasize**`) or *italics* using single asterisks (`*italics*`).

It is easy to create [hyperlinks](https://en.wikipedia.org/wiki/Hyperlink) (as `[hyperlinks](https://en.wikipedia.org/wiki/Hyperlink)`)

### Images
Each post is welcome to have at least one image. If you commit the image together with your post, you can link it relatively, i. e.

    ![](logo.jpg)

or if the image resides online, you can also provide an absolute address, e.g.

    ![](https://modelica.org/logo.jpg)
    
Please keep in mind, that the folder is shared for the whole issue and name the images specifically to your post to avoid collisions with contrbutions of others. E.g. if you post name is `new-version-of-FMI` use `new-version-of-FMI-logo.png` instead of just `logo.png` to avoid conflicts.
    
### Headings
Please use 4th level heading for headings within your posts, e.g.

    #### My Beatiful Subheading

### Preview
If writing directly in GitHub, make use of the *Preview changes* - which offers a live formatted preview of your text, including the images. GitHub-flavored Markdown is supported by kramdown by default, so you can use Markdown with GitHub Pages the same way you use Markdown on GitHub.

## Example
You can use the following code as a basis for your article or explore the [newsletter repository]({{site.current-contribution-url}}) to inspire from the previous contributions.

    ---
    title: FMI User Meeting at the Modelica Conference 2015
    author: "Christian Bertsch ([Robert Bosch GmbH](https://www.bosch.com/))"
    category: "association"
    ---

    ![FMI logo](http://fmi-standard.org/assets/img/fmi-logo.svg "FMI image"){:width="250px"}

    The FMI Project will organize an "**FMI User Meeting**" within the tutorial/workshop session on the first day of the Modelica Conference 2015 as a complement to the scientific track(s) on FMI.    
    The intention is 
    to increase the interaction between FMI users in different companies / institutions and the Modelica Association Project FMI.

    #### Agenda
    - FMI overview
    - FMI current status
    - future developments   
      (a longer discussion is anticipated here)
    - conclusion

## Example output
This code would yield the result in GitHub preview similar to this: 
(The table with the meta information would be stripped out in the final output)

| title  | author | category |
| :----: | :----: | :----: | 
| FMI User Meeting at the Modelica Conference 2015 | Christian Bertsch ([Robert Bosch GmbH](https://www.bosch.com/)) | association |


![FMI logo](http://fmi-standard.org/assets/img/fmi-logo.svg "FMI image"){:width="250px"}

The FMI Project will organize an "**FMI User Meeting**" within the tutorial/workshop session on the first day of the Modelica Conference 2015 as a complement to the scientific track(s) on FMI.    
The intention is 
to increase the interaction between FMI users in different companies / institutions and the Modelica Association Project FMI.

#### Agenda
- FMI overview
- FMI current status
- future developments   
  (a longer discussion is anticipated here)
- conclusion
