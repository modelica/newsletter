---
title: Submission guidelines
layout: default
---
## Process
Everyone is welcome to contribute a post to the Modelica newsletter, however the editor holds the right to decline without reason. The submission is done by creating a pull request to the dedicated newsletter repository.
{% if site.contribution-open %}

The submissions are currently open! The deadline for contributions to the current issue is **{{ site.contribution-deadline }}**. The newsletter would be published on {{ site.current-newsletter-date }}.

0. Create a GitHub account, log in.
1. Navigate to the [newsletter repository]({{site.current-contribution-url}}).
2. Click Create new markdown file, e.g. *my-new-post.md* (the file extension is important)
3. Insert your post. You can reuse the example below or inspire yourself from other posts in the folder. 
4. Commit changes. 
   * Note, that no changes has been made to the [newsletter repository]({{site.current-contribution-url}}). Instead, GitHub created your own copy (*a fork*) of the repository with your changes. 
   * If you already have this repository forked, you may create a new branch from the original repository.
   * If you want to modify your contribution or add a local image, you have to navigate to this branch of your fork (e.g. patch-1) and click on Create Pull-request.
5. Create pull-request   
6. Submit the pull request.

Please note, that all your contributions are public from the beginning for anyone who knows the (public) repository. If you insist on having the contribution private prior to the release, please [let me know](mailto:filip.jezek@creativeconnections.cz).

  {% else %}

*The contributions are closed right now*

{% endif %}

## Structure
Each post should start with a header information, starting and ending with a line with three slashes '---'. Then, three meta-information shall be inserted:
- `title` - a short title. Can be nested into quotes to prevent special characters (e.g. colons) from breaking the text.
- `author` - authors of the contribution and their affiliations, preferably including hyperlinks `[Modelica Association](http://modelica.org)`
- `category` - a category of the post. Currently, following four categories are currently accepted. However, if you feel, that your contribution does not exactly fit one of those, we might open a new category. Just [let us know](mailto:filip.jezek@creativeconnections.cz).
  - `"association"` - news regarding Modelica association
  - `"education"` - news regarding educational resources, or training  
  - `"library"` - news regarding new or improved libraries
  - `"vendor"` - news regarding new Modelica tools versions
  
## Markdown syntax   
For the text body, use the [kramdown](https://kramdown.gettalong.org/) flavor of the Markdown syntax. See the [quick reference](https://kramdown.gettalong.org/quickref.html).

### Text style
You can use **emphasize** by double asterisks (`**emphasize**`) or *italics* using single asterisks (`*italics*`).

It is easy to create [hyperlinks](https://en.wikipedia.org/wiki/Hyperlink) (as `[hyperlinks](https://en.wikipedia.org/wiki/Hyperlink)`)

### Images
Each post is welcome to have at least one image. If you commit the image together with your post, you can link it relatively, i. e.

    ![](logo.jpg)

or if the image resides online, you can also provide an absolute address, e.g.

    ![](https://modelica.org/logo.jpg)
    
### Preview
If writing directly in GitHub, make use of the *Preview changes* - which offers a live formatted preview of your text, including the images.

## Example
You can use the following code as a basis for your article:

    ---
    title: FMI User Meeting at the Modelica Conference 2015
    author: "Christian Bertsch ([Robert Bosch GmbH](https://www.bosch.com/))"
    category: "association"
    ---

    ![FMI logo](http://fmi-standard.org/assets/img/fmi-logo.svg "FMI image"){:width="250px"}

    The FMI Project will organize an "**FMI User Meeting**" within the tutorial/workshop session on the first day of the Modelica Conference 2015 as a complement to the scientific track(s) on FMI.   
    The intention is to increase the interaction between FMI users in different companies / institutions and the Modelica Association Project FMI.

    ### Agenda
    - FMI overview
    - FMI current status
    - future developments   
      (a longer discussion is anticipated here)
    - conclusion

## Example output
This code would yield the result in GitHub preview similar to this: 
(The table with the meta information would be stripped in the final output)

| title  | author | category |
| :----: | :----: | :----: | 
| FMI User Meeting at the Modelica Conference 2015 | Christian Bertsch ([Robert Bosch GmbH](https://www.bosch.com/)) | association |


![FMI logo](http://fmi-standard.org/assets/img/fmi-logo.svg "FMI image"){:width="250px"}

The FMI Project will organize an "**FMI User Meeting**" within the tutorial/workshop session on the first day of the Modelica Conference 2015 as a complement to the scientific track(s) on FMI.   
The intention is to increase the interaction between FMI users in different companies / institutions and the Modelica Association Project FMI.

### Agenda
- FMI overview
- FMI current status
- future developments   
  (a longer discussion is anticipated here)
- conclusion
