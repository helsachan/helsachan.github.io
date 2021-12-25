---
title:  "How I built my first website"
excerpt: It has always been my childhood dream to create a website or blog on my own! Here's a little post on how this site started.
date:   2021-08-28
categories: coding
header:
  overlay_image: /assets/images/2021-08-28/194160470.jpg
  overlay_filter: rgba(50, 40, 45, 0.85) 
---

## The story

Building a website is a childhood dream come true.

The closest I achieved as a child, in terms of building a website, was [Xanga][xanga]. Xanga used to be where I hung around during my teenage days. I had had many lovely memories browsing each other's blogs with my friends; we spent days and nights writing and sharing our happiness and sorrows. It's been a good 8 years until Facebook and Instagram took over and people migrated to newer social platforms looking for more "immediate and dynamic" social interactions. While I celebrate these new technologies like everyone else, the nostalgic feeling does sometimes come back to me.

{% include figure image_path="/assets/images/2021-08-28/xanga.png" caption="Xanga 2.0 -- let me know if you're still using it!" %}
{% include figure image_path="/assets/images/2021-08-28/194160470.jpg" caption="My profile picture back then" %}

For a brief period of time, I continued blogging on WordPress in a more private manner, but I did not really feel attached to it: it could be the lack of connection with people I used to blog with, the themes that I did not felt much connected to, or simply reminiscence that "everything used to be better". It was not until I started my career in the IT industry that I finally recalled what became my best memories from my Xanga days. I loved that my creativity flowed freely and I could decorate my site in any way as if it were a cozy home of mine: my site would be waiting for guests to come by, always ready to provide them with the warmest welcome I could ever give. I loved that I could visit others' places as well, and that I also got to learn things about them: what they were thinking, what struggles they were facing, and what kind of future they were looking forward to. It was a heartwarming paradise -- sometimes fun, sometimes overwhelming, sometimes silly, sometimes intellectual...

So here I am, a little grown-up: I still wholeheartedly like to think a lot, build and create as before, and aspire to innovation. One day I sat down and thought, "Am I ready to reform something I've made before and create something better?" 

Yes, I have felt much more confident and assured compared with the teenage self, and there goes the process of getting to make something happen. And here comes [https://helsachan.github.io][sitename]! My lovely site's born.

## Working it out

I wanted my site to become my dedicated platform to share a few hobbies of mine: coding, artsy things, random food I cook / bake, books. I have *a lot of passion* in all of them; that said, I often forget what I have learned; if I have written a few notes here, I could probably refresh my memory from time to time.

I was looking for a site layout similar to what [Medium][medium] provides, with a few customizable page layouts and modules: something likely textual for coding and books, and something more visual for artsy things and food. Of course, I wanted something free of charge too.

It turned out Jekyll would make the perfect fit for me. As I already owned a GitHub account, my site automatically came along with the domain name [https://helsachan.github.io][sitename]. The key's to use `helsachan.github.io` as my repo name and follow the [GitHub Pages][github-pages] documentation. Simple!

### Choosing a theme

I did a bit of search online, and found [Minimal Mistakes][minimal-mistakes] to be just right for me. It is free, compatible with GitHub Pages and comes up a couple of color themes and preset layouts, with different supports like optional commenting, video embedding, and header images. I am happy with the simplistic design, the flexibility and the clear documentation it provides. 

A favicon is the little remarkable icon appearing right beside your web address when you browse a website. For a company website it is usually the company logo; as for a personal website, it's usually just a cool add-on feature to make it a little more personalized. I browsed [https://favicon.io/][favicon] for a favicon I like: pancakes! 

{% include figure image_path="/android-chrome-512x512.png" caption="Yum yum" %}

### Playing around with `Gemfile` and `_config.yml`

This is essentially the most techy part of all! 

First, the `Gemfile` has to be tweaked to make sure you have the right setups. The `Gemfile` collects the packages we need, and we would run `bundle exec jekyll serve` to build the site and make it run on a local server. It almost feels magical, as you could essentially browse a functional, decent-looking site already. We will edit the `Gemfile` to add packages we need as we go.

Then, we can customize the `_config.yml` for additional configurations and features, e.g. LinkedIn username, breadcrumbs, and whether or not to show reading time. Remember to add the remote theme you have chosen into the `_config.yml` and the corresponding packages into `Gemfile`.

One tricky thing with `_config.yml` is that it does not get updated automatically as you refresh the site; by design, you can only see the updated changes as you restart the local server to serving the site. Besides that, the site will update automatically as you add, edit and remove pages. You would probably want to keep adding posts under the `_posts` directory.

### Editing the layout

Taking this post as an example, it's located under `_posts`, and the layout template comes from `_layouts/posts.html`. The tags that I have customized for this particular post includes:

```
title:  "How I built my first website" # my post title
excerpt: It has always been my childhood dream to create a website or blog on my own! Here's a little post on how this site started. # what text to show as the preview
date:   2021-08-28 # date of writing the article
categories: coding # which category/categories to put this under
header:
  overlay_image: /assets/images/2021-08-28/194160470.jpg # path to the header overlay image
  overlay_filter: rgba(50, 40, 45, 0.85) # color of overlay filter on the image
---
```

The above snippet is put at the very beginning of the posts markdown file. Then, the post content follows the same way as how you write a markdown file.

## Wrapping up

The building of website is really much easier than I thought and I am happy with its outcome. I'm off to a great start -- of course this is only the beginning of the journey and there will be lots that I could improve and learn! So thankful for Jekyll and Minimal Mistakes for making this happen, and please stay tuned for my upcoming posts! :)

[xanga]: http://xanga.com/
[sitename]: https://helsachan.github.io
[medium]: https://medium.com/
[github-pages]: https://docs.github.com/en/pages
[minimal-mistakes]: https://jekyllthemes.io/theme/minimal-mistakes
[favicon]: https://favicon.io/