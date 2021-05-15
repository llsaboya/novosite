---
title: content
excerpt: content
categories:
  - Notas
tags:
  - Code
header:
  overlay_image: /img/breves-notas.png
  overlay_filter: 0.5
  teaser: /img/breves-notas-th.png
toc: false
toc_sticky: true
---

bundle exec jekyll serve --livereload

![breves-notas-th](/img/breves-notas-th.png)

![breves-notas](/img/breves-notas.png)

The preferred way of using images is placing them in the `/assets/images/` directory and referencing them with an absolute path. Prepending the filename with `{% raw %}{{ site.url }}{{ site.baseurl }}/assets/images/{% endraw %}` will make sure your images display properly in feeds and such.

Standard image with no width modifier classes applied.
{: .notice} 

**mm:**

```html
{% raw %}

{% include video id="XsxDH4HcOWA" provider="youtube" %}

header:
  video:
    id: XsxDH4HcOWA
    provider: youtube


{% include figure image_path="path" alt="content" caption="content" %}


{% endraw %}
```



**or Kramdown:**

```markdown
{% raw %}![alt]({{ site.url }}{{ site.baseurl }}/assets/images/filename.jpg){% endraw %}
```

![Unsplash image 9]({{ site.url }}{{ site.baseurl }}/assets/images/unsplash-image-9.jpg)

Image that fills page content container by adding the `.full` class with:

**HTML:**

```html
{% raw %}<img src="{{ site.url }}{{ site.baseurl }}/assets/images/filename.jpg" alt="" class="full">{% endraw %}
```

**or Kramdown:**

```markdown
{% raw %}![alt]({{ site.url }}{{ site.baseurl }}/assets/images/filename.jpg)
{: .full}{% endraw %}
```

**Watch out!** This paragraph of text has been [emphasized](#) with the `{: .notice}` class.
{: .notice}

**Watch out!** This paragraph of text has been [emphasized](#) with the `{: .notice--primary}` class.
{: .notice--primary}

**Watch out!** This paragraph of text has been [emphasized](#) with the `{: .notice--info}` class.
{: .notice--info}

**Watch out!** This paragraph of text has been [emphasized](#) with the `{: .notice--warning}` class.
{: .notice--warning}

**Watch out!** This paragraph of text has been [emphasized](#) with the `{: .notice--success}` class.
{: .notice--success}

**Watch out!** This paragraph of text has been [emphasized](#) with the `{: .notice--danger}` class.
{: .notice--danger}

bundle exec jekyll serve --livereload
