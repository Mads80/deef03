+++
date = '2026-06-25T15:40:26+02:00'
draft = false
title = 'My First Post'
tags = ['hugo', 'blowfish', 'shortcodes', 'zed', 'html']
showAuthor = false
+++

This is my first post. Website is made with [Hugo](https://gohugo.io) and the theme is [Blowfish](https://github.com/dirkolbrich/blowfish).
I will be updting this post with stuff I learn along the way.

Below is a short list of tools I used to develop this website.

> [!NOTE] [Favicon.io](https://favicon.io)
> I used this very handy website to generate logo and favicon.
{icon="star"}

> [!NOTE] [Dashboardicons.com](https://dashboardicons.com/)
> Very cool website with lots of icons.
{icon="dashboard-icons"}

> [!NOTE] [Zed.dev](https://zed.dev)
> My editor of choice.
{icon="zed-editor"}

---

## Hiding Related Content

I wanted to hide my [About]({{< ref "/about" >}}) page from the Recent Posts section.

Start by creating `related.html in your `layouts/partials` directory. Paste the following code into it:

```html
{{ if .Params.showRelatedContent | default
(.Site.Params.article.showRelatedContent | default false) }} {{ $related :=
.Site.RegularPages.Related . }} {{ $related = where $related "Params.noRelated"
"!=" true }} {{ $related = $related | first
.Site.Params.article.relatedContentLimit }} {{ with $related }}
<h2 class="mt-8 text-2xl font-extrabold mb-10">
    {{ i18n "article.related_articles" | emojify }}
</h2>
<section class="w-full grid gap-4 sm:grid-cols-2 md:grid-cols-3">
    {{ range . }} {{ partial "article-link/card-related.html" . }} {{ end }}
</section>
{{ end }} {{ end }}
```

On the page you want to hide insert the following in the top section:

```toml
+++
noRelated = true
+++
```

## Shortcodes

I wanted to add a shortcode that shows current year.

If you don't already have a `shortcodes` directory in your `layouts` directory, create one.
Then create a file called `year.html` in the `shortcodes` directory and paste the following code into it:

```go
{{- now.Format "2006" -}}
```

Now you can use the `year` shortcode in your content like this:

```html
{{</* year */>}}
```

This is very handy for places like the footer where you want to display the current year. Which btw is `{{< year >}}` at the time you read this.
