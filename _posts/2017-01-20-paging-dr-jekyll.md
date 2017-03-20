---
layout: post
title: Paging Dr. Jekyll
---
It may be meta to describe how I built my portfolio site, but I still can't get over how it transformed within a week.

Since I'm approaching the end of my [full stack web development program](https://www.bloc.io/), I started turning my attention to my portfolio site last week. Out of the two standard Jekyll portfolio themes provided, I chose [Portfolio Kami](http://madebymunsters.github.io/Lannister/). But the more I tinkered with the theme, the more I wanted something a little more eye-catching. No offense, Kami.

I scrolled through many [Jekyll themes](http://themes.jekyllrc.org/), but my heart stopped at [Agency](https://startbootstrap.com/template-overviews/agency/). It was slick and definitely eye-catching, but missing a blog section. Super easy to add one, right? Wrong.

Over the course of a few days, one thing was clear to me: Jekyll is not as intuitive as you think. It took a little research, but I managed to build out a blog without interfering with the portfolio, through the use of categories. But I was tormented that I could somehow display all blog post titles and excerpts, and yet the link to each one was broken.

![snippet]({{site.baseurl}}/img/jekyll.png){:class="img-responsive"}

I investigated Jekyll categories and posts on Stack Overflow and [Jekyll Talk](https://talk.jekyllrb.com/), but I could not find a quick fix to what seemed to be a simple problem. After consulting with my mentor and reviewing other implementations of the Agency theme, I asked the experts at Jekyll Talk. Unfortunately, the friendly suggestion I received did not pan out. After another consultation with my mentor, I decided it would be best to spend my time customizing my original portfolio theme.

Within a day, I made the following changes:

#### 1. Color
Reviewed many [website color schemes](https://designschool.canva.com/blog/website-color-schemes/) and narrowed it down to the deep blue and yellow palette, Elegant and Sophisticated.

#### 2. Typography
Incorporated Agency's use of Montserrat, Droid Serif, and Kaushan Script.

#### 3. Cover Image
Searched [StockSnap.io](https://stocksnap.io/) for an image that resonated with me and could not believe my luck: a workspace that radiates the warmth of my color scheme.

#### 4. Skills Section
Replicated Agency's Services section with [Font Awesome](http://fontawesome.io/) icons in a three column responsive layout.

#### 5. Favicon
Created a code favicon to replace the provided pencil favicon. Such a minor detail, but it makes me smile when I see my blog as a tab in my browser.

Ultimately, I am thankful I crossed paths with the Agency theme. It not only gave me the confidence to experiment within a Jekyll theme, it renewed my respect for CSS. I favor Backend development over Frontend, but I cannot deny that CSS completely transformed a generic theme into something very personal. Building my portfolio site also allowed me to revisit Frontend and responsive design fundamentals.

The cherry on top is that I now feel comfortable troubleshooting Jekyll errors. Just today, another student posted a pesky Jekyll error in Slack and I was able to help him troubleshoot it (an extra character in his `_config.yml` file).

I'm officially a Jekyll fan.
