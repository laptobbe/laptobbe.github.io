+++
date = "2015-03-10T17:12:44+01:00"
title = "Simple website with Hugo"
+++

As you might see I have changed the design of my website (more likely this is your first time here, in any case welcome). I first got the idea when the site generation engine [Hugo](http://gohugo.io/) was mentioned on [Kodsnack](http://kodsnack.se/). They said they used it to generate the website for their podcast and it sounded very easy and convenient to use. So here it is.

In this post I will write a bit about Hugo and what I think about the approach.

<!--more-->

### About Hugo

*”A Fast & Modern Static Website Engine”*

Hugo likes to brag about how fast they generate sites. I was really sceptical to this a first, not doubting that it would be fast, but how necessary it was for it to be that fast. But as I am writing this I am tabbing between my [markdown](http://daringfireball.net/projects/markdown/syntax) editor of choose [Byword](http://bywordapp.com/) and my website that is regenerated each time I save. I suspect I can’t go back to working in any other way.

``` bash
hugo server -w
```
So this is no tutorial on how to use Hugo to create your site. They provide excellent [tutorials](http://gohugo.io/overview/introduction/) for that. What I want to write about is the concept itself.

Since Hugo sites are actually just old HTML and CSS sites with no dynamic elements or server side loading the sites load extremely fast in the viewers browser. Again with the speed you say, yes it’s important! How much do you resent websites that load slowly? I for one can’t stand it, so why should my readers.

### Mobile

Hugo generates it’s sites from markdown as I mentioned earlier, this is great because that is just a basic textile. Making it easy to edit it from anywhere on any device. Fits me perfectly. One thing I need to solve with my setup is the fact that I host the site as a [Github page](https://pages.github.com/). Not that I want a different host but I need to find a good markdown editor with a git client. Hmm maybe I will just build one myself.

Anyway what I am thinking of doing now is to put the entire site into dropbox so I can easily get the files on my iPhone and iPad. Would be great to be able to review and write on the subway on the way to town.

### Themes

Hugo has a limited number of themes and they can be quite difficult to browse through. But it is open source and more are being added all the time. I actually added my theme as a submodule and it has been working great so far.

``` bash
git submodule add https://github.com/keichi/vienna
```
And it’s so easy to override the CSS, Images, etc., from the theme. Just add your version of the file you want to replace in your tree at the same relative path as in the theme and Hugo will pick that resource instead. 

### Conclusion

To conclude. I think that if your website ”Needs” one of these big, evil content management systems, like [Wordpress](https://wordpress.com/website/), you are doing it wrong!





