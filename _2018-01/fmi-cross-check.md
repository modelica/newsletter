---
title: Updated FMI Cross Check Process 
author: Michael M. Tiller ([Xogeny](https://www.xogeny.com))
category: modelica-association
---

The FMI project collects and publishes so-called "cross check" data.  As part of this process, each vendor
publishes data about their FMI compliant tools along with FMUs exported from those tools.  This allows other
vendors to test those FMUs by importing.  In this way, the vendors work together to detect any non-compliant
implementations in an effort to boost FMI compliance.

This process used to involve one very large SVN repository where *all* vendors published not only their
tool data and FMUs but the results of their attempts to import other FMUs.  Needsless to say, with all
the large binary files and data files associated with this compliance checking process, the repository
got to be very large.  Furthermore, the Modelica Association had to manage users, permissions, disk
space, *etc.* for this effort.

In an attempt to streamline the process, it was decided to give every vendor their own repository.  In
these repositories, vendors compile data about themselves, their tools, sample FMUs and results of 
importing FMUs from other tools.  In this way, each vendor repository is a more manageable size and since
each vendor is managing the repository themselves, the Modelica Association doesn't need to get involved
in the management of users, permissions, *etc.*.

To facilitate this process, the Modelica Association established the [`fmi-crosscheck` organization]
(https://github.com/fmi-crosscheck) on GitHub.  Each vendors existing FMI data was broken out into
individual vendor-specific repositories.  Furthermore, these repositories use a technology called 
[webhooks](https://developer.github.com/webhooks/) to signal when they have been updated.  Using these
webhooks, the entire process of generating the FMI web site has been automated.  Now, when any vendor
pushes changes to their repository, a completely rebuild of the FMI web site is triggered using the very
latest vendor data.

But there were changes beyond simply creating vendor specific repositories.  The scripts that process
the data were completely rewritten.  While the previous pages on the FMI web site were static
HTML pages generated while processing the cross check data, the new process involves compiling all
the cross check data into a machine readable form and then rendering it *dynamically* on the web site.
This allows visitors to the site to search and filter the FMI compliance data interactively.  Instead of
long tables and horizontal scrollbars, the new dynamic visualization encourages users to search,
filter and zoom to explore the data which generally fits on a single page.  Users can even bookmark
specific search, filter and selection settings and/or email their results to others as a single URL.

If you are a vendor and you have not yet taken ownership of your new repository, please [contact me]
(mailto:michael.tiller@gmail.com) so you can be added as an admin to your repository.  A preview of
the new dynamic web site can be found at [https://preview.fmi-standard.org](https://preview.fmi-standard.org).
If you find any issues, please report them in the [`fmi-crosscheck-tools` issue tracker](https://github.com/modelica/fmi-crosscheck-tools/issues).
