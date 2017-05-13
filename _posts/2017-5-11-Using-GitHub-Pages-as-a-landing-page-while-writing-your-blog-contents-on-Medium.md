---
layout: post
title: Using GitHub Pages as a landing page while writing your blog contents on Medium
description: Start blogging with flexibility with beautiful themes, Jekyll, custom domain and DNS provider of your choice.
image: assets/images/blog-img/camera-1215600_640-low.jpg
medium: https://medium.com/@evanzhoe/using-github-pages-as-a-landing-page-while-creating-blog-contents-on-medium-7efd4028bec0
---

After setting up a working site on GitHub pages, I realized that even though GitHub Pages are simple but personally, blogging on Medium would be much simpler when I can quickly add images onto my blog contents without worrying about sorting my image files in the correct folder and renaming them correctly.

>In this way, I could focus on writing and styling easily. Essentially, it is sort of a hybrid of Medium+ GitHub pages.


For those who want to take advantage of Medium’s large audience base, while, at the same time, want to keep a landing page, you could easily set a predefined variable at the front matter between the triple dashes like so:

Finally, add a href tag in your _includes file (or anywhere logically) with the link
```
<h3><a href=”{{ post.medium }}” class=”link”>{{ post.title }}</a></h3>
```
(Note: ‘post’ is just my file html layout file & I have a file for my tiles which displays the post titles and their images).

Also, check out Jekyll’s documentation on Front Matter!

To sum up, using Medium as my tool for content creation, I could:

* Add images & links quickly  
* Have better visualization on the layout without running Jekyll on my localhost  
* Have access to Medium users  
* Your blog visitors could benefit from the interaction tools on Medium such as recommending, commenting and especially bookmarking!

Alternatively, you could blog on GitHub pages and also create links to medium for your blog readers to redirect to Medium to read your contents.

So, it is not an either-or situation but rather, I have plans to design my blog on GitHub pages without images optimized for those who are using limited mobile data.

>Your challenge for the day: Try setting up a blog post on GitHub Pages, create a blog post, and then add add a link to your Medium blog in the front matter section!

Feel free to comment below if you need help. Good luck!
