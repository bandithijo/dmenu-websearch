# dmenu-websearch

Shorthand for web search based on each own query with dmenu.

## 📦 Dependencies

0. [dmenu](https://tools.suckless.org/dmenu), is a dynamic menu for X
1. [jq](https://github.com/stedolan/jq), is a lightweight and flexible command-line JSON processor

## 🌎 Web Search Queries

`.urlquery`

```
[ "Arch:Manpage",        "https://man.archlinux.org/search?q=" ],
[ "Arch:Wiki",           "https://wiki.archlinux.org/index.php?search=" ],
[ "Arch:Packages",       "https://archlinux.org/packages/?q=" ],
[ "Arch:Packages:AUR",   "https://aur.archlinux.org/packages/?K=" ],
[ "DuckDuckGo:Search",   "https://duckduckgo.com/?q=" ],
[ "GitHub:Search",       "https://github.com/search?q=" ],
[ "Google:Search",       "https://duckduckgo.com/?q=!g+" ],
[ "Google:Search:Image", "https://duckduckgo.com/?q=!gi+" ],
[ "Google:Translate",    "https://translate.google.com/?sl=auto&tl=id&text=" ],
[ "Ruby:Gems",           "https://rubygems.org/gems/" ],
[ "Ruby:Toolbox",        "https://www.ruby-toolbox.com/search?q=" ],
```

## 🏗️ How to add new query?

Just add new URL query via **Add:New:Query** menu. It will asking about value of **prefix menu** & **URL query**.

## 🍱 How to use?

Call `dmenu-websearch`. Choose your prefix menu, or you able to complete the **perfix menu** with <kbd>Tab</kbd>, and write down your keywords.

The form should be like this,

```
Arch:Packages libreoffice still
^^^^^^^^^^^^^ ^^^^^^^^^^^^^^^^^
 prefix menu      keywords
```

**TIP**: You're free to define the **prefix menu**. My example is just for ease to explaining.

## 💃 Demo

![demo-01](.image/gambar-01.gif)

![demo-02](.image/gambar-02.gif)

## 🗒️ TODO

- [x] Create a menu to add a query
- [x] Retrieve query url value from urlquery file
- [x] Create urlquery.example and enter the urlquery into gitignore
- [x] If urlquery does not exist, create new from urlquery.example
- [x] Do not put in the urlquery file if the menu prefix & query url are empty
- [x] Create a menu to delete the selected data url query from the urlquery file
- [ ] Create a menu to edit the selected data url query from the urlquery file

## 🍻 Related Project

\* **NOTE**: Feel free to add your project (if related) here.

0. link:https://github.com/m0rphism/haskell-dmenu-search[haskell-dmenu-search^], dmenu script for searching the web with customizable search engines.
1. link:https://gitlab.com/surfraw/Surfraw/[surfraw^], Shell Users' Revolutionary Front Rage Against the Web.

## 🏛️ Copyright and License

Copyright © 2021 Rizqi Nur Assyaufi.

Free use of this software is granted under the terms of the MIT License.

See [LICENSE](LICENSE) for details.
