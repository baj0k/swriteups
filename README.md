# sWriteups
A minimal blogging theme for Hugo static site generator.
The name comes from the words simple and writeups combined together thus sWriteups. Also when you read the name in English pronunciation and Polish meaning it greatly references the quality of the project.

Real-life example can be found at https://bajok.kretes.xyz.

## Features
- Extremely fast
- HTML/CSS only, no JS
- Dark theme
- RSS support

## Installation
```
git clone https://github.com/baj0k/debloat.git /your/hugo/themes/directory
```
Add the following lines to the hugo site config file (TOML format).
```
baseURL = "https://website.example.com"
languageCode = "en-us"
title = "Title"
theme = "debloat"
disableHugoGeneratorInject = true
pygmentsCodefences = true
pygmentsCodefencesGuessSyntax = true
pygmentsStyle = "native"

# Markup
[markup]
  [markup.tableOfContents]
    startLevel = 2
    endLevel = 3
    ordered = false

  [markup.highlight]
    lineNumbersInTable = false
    style = 'nord'
    tabWidth = 4

# Parameters
[params]
    subtitle = "Subtitle"
    dateFmt = "02.01.2006"
    mainSections = ['writeups', 'posts']

# Header
[menu]
  [[menu.main]]
        identifier = "about"
        name = "About"
        url = "/about"
        weight = 1 

  [[menu.main]]
        identifier = "posts"
        name = "Posts"
        url = "/posts/"
        weight = 2 

  [[menu.main]]
        identifier = "writeups"
        name = "Writeups"
        url = "/writeups/"
        weight = 3 

  [[menu.main]]
        identifier = "categories"
        name = "Categories"
        url = "/categories/"
        weight = 4 

  [[menu.main]]
        identifier = "tags"
        name = "Tags"
        url = "/tags/"
        weight = 5

# Footer
  [[menu.footer]]
        name = "Git"
        url = https://github.com/example
        weight = 1 

  [[menu.footer]]
        name = "Mail"
        url = "mailto://user@example.com"
        weight = 2 
        # RSS

# RSS
  [[menu.rss]]
        name = "RSS"
        url = "https://example.com/rss.xml"
        weight = 1
```
