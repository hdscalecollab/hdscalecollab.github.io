---
title: Adding a New Post to the Blog
description:
categories: resource
header-img:
author: Jay Yang
tags: [Lab Resource]
---

(Edited from the Jekyll documentation: https://jekyllrb.com/docs/posts/)

### The Posts Folder

The ```_posts``` folder is where all blog posts live. You typically write posts in Markdown, HTML is also supported.

<br>

### Creating Posts

To create a post, add a file to the  ```_posts``` folder in the lab's GitHub repository directory with the following format:

```
YEAR-MONTH-DAY-title.md
```

Where ```YEAR``` is a four-digit number, ```MONTH``` and ```DAY``` are both two-digit numbers, and ```.md``` is the file extension representing the format used in the file. For example, the following are examples of valid post filenames:

```
2011-12-31-new-years-eve-is-awesome.md
2012-09-12-how-to-write-a-blog.md
```
<br>

### Front Matter

All blog post files must begin with a structured front matter which is typically used to set a layout and define meta data of the post. A simple example would look like:

```
---
layout: post
title: "My Post's Title"
categories: categories
author: Author 1, Author 2
tags: [tag 1, tag 2]
---

<<Your post content starts here...>>
```

- ```layout```: Use ```layout: post```
- ```title``` : This is the title that will show up in the blog list.
- ```categories``` : Refer to the list of categories [here]().
- ```author``` : List the author(s) of your post, separated by comma
- ```tags``` : Refer to the list of tags [here]().
