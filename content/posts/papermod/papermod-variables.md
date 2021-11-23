---
draft: true
title: "Variables | Front Matter"
summary: List of Front Matter variables used by PaperMod
date: 2021-01-20
tags: ["PaperMod"]
series: ["PaperMod"]
author: "Aditya Telange"
weight: 5
cover:
    image: "https://images.unsplash.com/photo-1637441319442-943119624c2d?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2075&q=80"
    # can also paste direct link from external site
    # ex. https://i.ibb.co/K0HVPBd/paper-mod-profilemode.png
    alt: "<alt text>"
    caption: "<text>"
    relative: false # To use relative path for cover image, used in hugo Page-bundles
---

**Below are variables used with this theme...**

---

### Site Variables under `Params`

| name                                   | type          | example                  | Description                                                                               |
| -------------------------------------- | ------------- | ------------------------ | ----------------------------------------------------------------------------------------- |
| `env`                                  | string        | 'production'             | To set env to production                                                                  |
| `title`                                | string        | 'My Blog'                | To set title                                                                              |
| `description`                          | string        | 'This is a blog of mine' | To set site description                                                                   |
| `author`                               | string \|list | 'Me' \| ['Me','You']     | To show multiple Authors                                                                  |
| `images`                               | string        | 'myimage.png'            | Link or path of image for opengraph, twitter-cards                                        |
| `keywords`                             | list          | [blog, page]             | Add keywords for Home page                                                                |
| `DateFormat`                           | string        | "January 2, 2006"        | The format of date strings in the website. [Details](https://gohugo.io/functions/format/) |
| `languageAltTitle`                     | string        | "English"                | Alternate title in Multilingual Mode                                                      |
| `ShowReadingTime`                      | boolean       | true \| false            | To show read time in post meta                                                            |
| `ShowShareButtons`                     | boolean       | true \| false            | To show/hide share buttons under post                                                     |
| `ShowCodeCopyButtons`                  | boolean       | true \| false            | To show/hide Code Copy button                                                             |
| `ShowFullTextinRSS`                    | boolean       | true \| false            | To show Content in RSS feed                                                               |
| `defaultTheme`                         | string        | light \| dark \| auto    | To set default theme                                                                      |
| `disableThemeToggle`                   | boolean       | true \| false            | To disable theme toggle icon shown besides label                                          |
| `disableSpecial1stPost`                | boolean       | true \| false            | To disable no-card special appearance of 1st post                                         |
| `disableScrollToTop`                   | boolean       | true \| false            | To disable ScrollToTop button                                                             |
| `disableAnchoredHeadings`              | boolean       | true \| false            | To disable Anchored Headings                                                              |
| `hideMeta`                             | boolean       | true \| false            | To Hide meta elements : date, read-time, author and available-translations for page       |
| `hideSummary`                          | boolean       | true \| false            | To Hide summary being shown in list pages                                                 |
| `showtoc`                              | boolean       | true \| false            | To show/hide Table of Contents                                                            |
| `tocopen`                              | boolean       | true \| false            | To keep open ToC by default on page load                                                  |
| `ShowPostNavLinks`                     | boolean       | true \| false            | Show Previous and Next Posts below a Post                                                 |
| `ShowBreadCrumbs`                      | boolean       | true \| false            | Show BreadCrumb Navigation above single post/page                                         |
| `comments`                             | boolean       | true \| false            | To show/hide comments                                                                     |
| `analytics.google.SiteVerificationTag` | string        | "XYZabc"                 | Site Verification Tag for Google Analytics                                                |
| `analytics.bing.SiteVerificationTag`   | string        | "XYZabc"                 | Site Verification Tag for Bing                                                            |
| `analytics.yandex.SiteVerificationTag` | string        | "XYZabc"                 | Site Verification Tag for Yandex                                                          |
| `schema`                               | -             | -                        | [Details](#schema)                                                                        |
| `fuseOpts`                             | -             | -                        | [Details](#fuseOpts)                                                                      |
| `socialIcons`                          | -             | -                        | [Details](#socialIcons)                                                                   |
| `label`                                | -             | -                        | [Details](#label)                                                                         |
| `assets`                               | -             | -                        | [Details](#assets)                                                                        |
| `cover`                                | -             | -                        | [Details](#cover)                                                                         |
| `profileMode`                          | -             | -                        | [Details](#profilemode)                                                                   |
| `editPost`                             | -             | -                        | [Details](#editPost)                                                                      |

### Site Variables

| name        | type   | example                                    | Description                                                                                                                   |
| ----------- | ------ | ------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------- |
| `copyright` | string | `**[example.site](https://example.site)**` | This is [HUGO's site variable](https://gohugo.io/variables/site/#site-variables-list), which can also render markdown content |

#### label

| name               | type    | example                 | Description                                      |
| ------------------ | ------- | ----------------------- | ------------------------------------------------ |
| `label.text`       | string  | 'Home'                  | To display different label text other than title |
| `label.icon`       | string  | '/apple-touch-icon.png' | To display a logo image in label                 |
| `label.iconHeight` | integer | 35                      | To set size of label logo image                  |

#### profileMode

| name                      | type    | example                                        | Description                                          |
| ------------------------- | ------- | ---------------------------------------------- | ---------------------------------------------------- |
| `profileMode.enabled`     | boolean | true \| false                                  | For enabling profileMode, needs to be explicitly set |
| `profileMode.title`       | string  | "Title"                                        | Title                                                |
| `profileMode.subtitle`    | string  | "subtitle here"                                | Subtitle                                             |
| `profileMode.imageUrl`    | string  | "image.png" \| "https://example.com/image.jpg" | Image URL or Link                                    |
| `profileMode.imageWidth ` | string  | "150"                                          | Width of image                                       |
| `profileMode.imageHeight` | string  | "150"                                          | Height of image                                      |
| `profileMode.imageTitle`  | string  | "This image is a picture of .."                | Title of image                                       |
| `profileMode.buttons`     | -       | -                                              | [Details](#profileModebuttons)                       |

##### profileMode.buttons

```yml
profileMode:
    buttons:
        - name: Archive
        url: "/archive"
        - name: Github
        url: "https://github.com/"
```

#### assets

| name                           | type    | example       | Description                                  |
| ------------------------------ | ------- | ------------- | -------------------------------------------- |
| `assets.favicon`               | string  | 'icon.ico'    | To set favicon, can be path or external link |
| `assets.disableHLJS`           | boolean | true \| false | To disable Highlight.js loading              |
| `assets.disableFingerprinting` | boolean | true \| false | To disable Sub-Resource integrity for assets |

#### cover

| name                     | type    | example       | Description                                             |
| ------------------------ | ------- | ------------- | ------------------------------------------------------- |
| `cover.linkFullImages`   | boolean | true \| false | To open full size cover images on click on cover        |
| `cover.responsiveImages` | boolean | true \| false | To enable/disable generation of responsive cover images |
| `cover.hidden`           | boolean | true \| false | To hide everywhere but not in structured data           |
| `cover.hiddenInList`     | boolean | true \| false | To hide on list pages and home                          |
| `cover.hiddenInSingle `  | boolean | true \| false | To hide on list pages and home                          |

#### schema

| name                   | type   | example          | Description                   |
| ---------------------- | ------ | ---------------- | ----------------------------- |
| `schema.publisherType` | string | 'Organization'   | https://schema.org/publisher  |
| `schema.sameAs`        | list   | ["URL1", "URL2"] | Set https://schema.org/sameAs |

#### fuseOpts

Refer: https://fusejs.io/api/options.html

```yml
fuseOpts:
  isCaseSensitive: false
  shouldSort: true
  location: 0
  distance: 1000
  threshold: 0.4
  minMatchCharLength: 0
  keys: ["title", "permalink", "summary", "content"] ##  can be less but not more than shown in list
```

#### socialIcons

```yml
socialIcons:
    - name: "<platform>"
        url: "<link>"
    - name: "<platform 2>"
        url: "<link2>"
```

#### editPost

```yml
editPost:
  URL: "https://github.com/<path_to_repo>/content"
  Text: "Suggest Changes" # edit text
  appendFilePath: true # to append file path to Edit link
```

> Note: Same format is being used by Page Variables

---

### Page Variables

| Name                      | Type          | Example                         | Description                                                                         |
| ------------------------- | ------------- | ------------------------------- | ----------------------------------------------------------------------------------- |
| `showtoc`                 | boolean       | true \| false                   | To show/hide Table of Contents                                                      |
| `tocopen`                 | boolean       | true \| false                   | To keep open ToC by default on page load                                            |
| `hidemeta`                | boolean       | true \| false                   | To Hide meta elements : date, read-time, author and available-translations for page |
| `comments`                | boolean       | true \| false                   | To show/hide comments                                                               |
| `description`             | string        | 'description text'              | Show Post Description under Title                                                   |
| `canonicalURL`            | string        | "https://canonical.url/to/page" | To add canonical URL to posts                                                       |
| `disableShare`            | boolean       | true \| false                   | To hide/show share icons under a page                                               |
| `disableHLJS`             | boolean       | true \| false                   | To disable Highlight.js loading                                                     |
| `disableAnchoredHeadings` | boolean       | true \| false                   | To disable Anchored Headings                                                        |
| `searchHidden`            | boolean       | true \| false                   | Hide page from search                                                               |
| `hideSummary`             | boolean       | true \| false                   | To Hide summary being shown in list pages                                           |
| `ShowReadingTime`         | boolean       | true \| false                   | To show read time in post meta                                                      |
| `ShowBreadCrumbs`         | boolean       | true \| false                   | Show BreadCrumb Navigation above single post/page                                   |
| `ShowPostNavLinks`        | boolean       | true \| false                   | Show Previous and Next Posts below a Post                                           |
| `author`                  | string \|list | 'Me' \| ['Me','You']            | To show multiple Authors                                                            |
| `cover.image`             | string        | 'featured.jpg'                  | To add a cover image                                                                |
| `cover.caption `          | string        | 'caption for image'             | To add caption to cover image                                                       |
| `cover.alt`               | string        | 'this is cover image'           | Alternate text to show if image doesn't load/show up                                |
| `cover.relative`          | boolean       | true \| false                   | To use relative path for cover image, used in hugo Page-bundles                     |
| `cover.hidden `           | boolean       | true \| false                   | To hide on current single page                                                      |
| `weight `                 | integer       | 5                               | To set page order or to pin a post to Top of list                                   |