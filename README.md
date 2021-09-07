<h1 align="center">barks</h1>

**barks** is a simple, minimalistic theme for the static website generator [Hugo](https://gohugo.io). Its was primarily developed as a theme for personal (academic) websites, although it may also be useful for other purposes 🙃



<br>

<p align="center">
  <img width="80%" src="images/mockup.png">
</p>
<br>



## ⚡️ Quickstart

If you already have a Hugo site, you can use **barks** as your theme by calling:

```bash
git submodule add https://github.com/timothygebhard/barks
```

in your `themes` directory, and changing the `theme` parameter in your `config.toml` to `"barks"`.

Otherwise, you might want to check out the [Hugo quickstart guide](https://gohugo.io/getting-started/quick-start/).



## 📄 Layout for landing page

If you want to use the landing page as shown in the screenshot above, put `layout: landing_page` into the header of your `_index.md` file.  Additionally, you need to add `image: <image_url>` to specify the image that should be used.



## ⚙️ Configuration

**barks** comes with a number of customization options to personalize its looks through the `[params]` section in the `config.toml` file. Most options should be rather self-explanatory; nevertheless, here is a quick overview:



**Navigation and footer:**

You can disable the navigation (e.g., if all your content fits onto a single page) and the footer (e.g., if you don’t need the social media icons or a copyright notice) using:

```toml
[params.navigation]
	  show_navigation = true

[params.footer]
    show_footer = true
```



**Typography:**

You can choose the font for the website title (i.e., the header), as well as the main text using:

```toml
[params.typography]
    title_font = "Bree Serif"
    body_font = "Source Sans Pro"
```

You can use *any* [Google Font](https://fonts.google.com/) here; **barks** will load them automatically.



**Colors:**

Change the colors of the [theme](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/meta/name/theme-color), the background, the text, and the links in the navigation using:

```toml
[params.colors]
    theme_color = "#333333"
    background_color = "#fcfbf9"
    text_color = "#333333"
    link_color = "#60c17d"
```



**Social media:**

If you link your social media profiles or contact options, they will automatically be displayed in the footer (using icons from [FontAwesome](https://fontawesome.com)). The following platforms are currently supported:

```toml
[params.social]
    email = "<email_address>"
    github = "<github_url>"
    google_scholar = "<google_scholar_url>"
    instagram = "<instagram_url>"
    institution = "<institution_url>"
    linkedin = "<linkedin_url>"
    orcid = "<orcid_url>"
    skype = "<skype_url>"
    twitter = "<twitter_url>" 
```

Remove any fields you don’t need, or leave them empty.



**Disabling page titles:**

By default, each page prints the `title` that is specified in the header as a `<h1>`-level heading at the top of the page. You can disable this for any given page by adding `hide_title: true` to the header.



## 🤓 LaTeX support

You can enable LaTeX support (via [KaTeX](https://katex.org/)) by adding `math: true` to the header section of each page or post in which you want to use it. (That way the corresponding JS is only loaded when it is needed.)

Use single dollar signs for inline formulas, and double dollar signs for typesetting math in a new paragraph.



## 🦄 Contributing

Direct contributions and pull requests to improve **barks** are always welcome! Otherwise, you can of course also help the development by creating issues for bugs that you have encountered, or for new features that you would like to see implemented 🙃



## ⚖️ License

**barks** is released under the [MIT license](https://opensource.org/licenses/MIT); see [LICENSE](https://github.com/timothygebhard/barks/blob/main/LICENSE) file.

