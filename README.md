# Notes by loupbrun

A minimal theme for those who like to keep it simple. Makes use of bootstrap.

Based on the [Elephants theme](https://themes.gohugo.io/elephants/) and [Basics](https://github.com/arjunkrishnababu96/basics).

## Features

* Responsive theme
* High contrast
* Focus on content and readability

## Installation

From your hugo site, run:
```
git submodule add https://github.com/loup-brun/hugo-theme-notes.git themes/basics
```

### Writing Posts

Posts that should show up in the home page must be inside `contents/post`. Or you can change this behavior by tweaking `themes/hugo-theme-notes/layouts/_default/list.html`.

You should also add an about page at `contents/about.md`.

Your directory should look something like this:
```
├── archetypes
│   └── default.md
├── config.yaml
├── content
│   ├── about.md
│   └── notes
│       ├── seance00.md
│       └── seance01.md
├── data
├── layouts
├── static
│   └── images
└── themes
    └── hugo-theme-notes
```


### Configurations

#### Add author name

Add author name to the `.Site.Params.author` parameter in your `config.yaml` file.

See below for an example:
```
baseURL: 
languageCode: fr
title: XXX000 – Notes de cours
theme: hugo-theme-notes

params:
    author: Nom de l'auteur
```

#### Add Links to GitHub and GitLab

Add GitHub and GitLab usernames to `.Site.Params.github` and `.Site.Params.gitlab` parameters in your `config.toml` file. Links to these accounts would show up in the top navigation bar. If these parameters are not present or is left blank, the links would disappear.

See below for an example:
```
baseURL:
languageCode: fr
title: XXX000 – Notes de cours
theme: hugo-theme-notes

params:
    author: Nom de l'auteur
    github: username1
    gitlab: username2
```


## License

Released under the [MIT License.](https://github.com/loup-brun/hugo-theme-notes/blob/master/LICENSE.md)
