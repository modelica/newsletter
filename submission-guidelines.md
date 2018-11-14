---
title: Submission guidelines
layout: default
description: How to contribute to the [Modelica Association newsletter](./)
---
## Scope
Everyone is welcome to contribute a post to the Modelica newsletter, however the editor holds the right to decline a contribution without reason. The scope of the newsletter include all topics covered by the [Modelica Association](https://www.modelica.org) (Modelica language, libraries, FMI, SSP, DCP), related tools and news in education (courses, books and related materials). If you have an item of interest that you would like to share with the Modelica community, for example:
- A brief note on a Modelica related project.
- Information about Modelica libraries, tools or services (technical details only, no marketing or advertising content).
- Upcoming Modelica related events.    
...please consider submitting a brief write-up about it to the Modelica Newsletter.

Submission guidelines are as follows (Exceptions are possible in justified cases):
- **Relevance:** Of course, the material must be of interest to the general Modelica community.  But in addition, part of being relevant is being timely.  So articles should contain information that can impact the present and future options for readers and not simply contain historical information.
- **Novelty:** This is a newsletter.  As such, what is contained in it must be new.  It is unacceptable for an article to repeat content from previous articles.  If you feel that background information is required, provide it via a hyperlink to information stored elsewhere.  For example, don't list the features of your tool and/or library with every article about it.  Instead, include a hyperlink, e.g. "In addition to existing features, version X.Y.Z includes the following new features..."
- **Tone:** Articles are expected to be of a mostly factual nature and avoid hyperbole and excessive marketing and advertising content.
One post per product: Individual new features to a product should not be divided to another article. If the features require further description, then there shall be provided links to further information.
- **Length:** approximately 3-4 paragraphs. Please try to squish only the most important information into no more than 200 words. Additional information should be linked to another page.
- **Additional materials:** Additional materials (i.e., extensive product description, leaflet, additional images etc.) could be uploaded as well to prevent dead links in the future.  It is possible (and perfectly easy) to host the linked page within the newsletter repository, however it would not be listed among the posts (only linked from the article). Any additional pages (.md files) not meant for the newsletter main page shall include the `--hidden: true` mark in the header.
- **Images:** One image no larger than 620x400 px is preferred, please upload the image alongside with your post - external images tend to break after while. It is the submitters responsibility to resize the image to meet these guidelines. 
- **Format:** clean kramdown (See below):
  - No style attributes, html tags are to be avoided, when possible
  - No spacing or layout directives


## Process
The submission is done by creating a pull request to the dedicated newsletter repository.
{% if site.contribution-open %}

The submissions are currently open! The deadline for contributions to the current issue is **{{ site.contribution-deadline }}**. The newsletter would be published on **{{ site.current-newsletter-date }}**.

0. Create a GitHub account, log in.
1. Navigate to the [newsletter repository]({{site.current-contribution-url}}) - it is important to keep your contribution within the folder with the current issue, e.g. `_2018-02`. Contributions to other folders would be discarded.
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

[Subscribe to the Newsletter Contributors mailing list](http://eepurl.com/dpvIVP), so we would let you know, when the next newsletter is being prepared.

{% endif %}

## Structure
Each post should start with a header information, starting and ending with a line with three slashes '---'. Then, three meta-information shall be inserted:
- `title` - a short title. Can be nested into quotes to prevent special characters (e.g. colons) from breaking the text.
- `author` - authors of the contribution and their affiliations, preferably including hyperlinks, e.g. `[Modelica Association](http://modelica.org)`
- `category` - a category of the post. Currently, following four categories are currently accepted. However, if you feel, that your contribution does not exactly fit one of those, we might open a new category. Just [let us know](mailto:filip.jezek@creativeconnections.cz).
  - `"association"` - news regarding Modelica association
  - `"project"` - news regarding Modelica Association related projects
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

### Text style and hyperlinks
You can use **emphasize** by double asterisks (`**emphasize**`) or *italics* using single asterisks (`*italics*`).

It is easy to create [hyperlinks](https://en.wikipedia.org/wiki/Hyperlink) (as `[hyperlinks](https://en.wikipedia.org/wiki/Hyperlink)`). Caution, not-tagged links are not generated, e.g. https://modelica.org/ will stay exactly as written (even though the GitHub's *Preview changes* shows them as links)

### Images
Each post is welcome to have one image. For a single image, please keep the image size 620x400px or below. When using multiple images, please try to occupy as low vertical space as possible. If required, you can link to the full size image. 

If you commit the image together with your post, you can link it relatively, i. e.

    ![Alt text](My-Company-logo.jpg 'Title text')

The alt and title text could be omitted. Please keep in mind, that the folder is shared for the whole issue and name the images specifically to your post to avoid collisions with contributions of others. E.g. if you post name is `new-version-of-FMI` use `new-version-of-FMI-logo.png` instead of just `logo.png` to avoid conflicts.
    
### Headings
Please use **4th level heading** for any headings within your posts, e.g.

    #### My Beautiful Subheading

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
