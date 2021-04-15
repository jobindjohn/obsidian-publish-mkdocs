# Publish Obsidian Notes with MkDocs (template)

Would you like to make some of your [Obsidian](https://obsidian.md/) notes public?

This template gives you an easy way to publish your Obsidian notes on your Github pages.

With this template, you get these **out-of-the-box**:

- an awesome website based on Material theme, complete with a search bar (Checkout this template published [here](https://jobindj.github.io/obsidian-mkdocs/))
- get the Obsidian/Roam style `[[wikilinks]]` from your vault in your published notes
- Toggle between light and dark mode


## How to get started?

1. Create a new github repository using [this template](https://github.com/jobindj/obsidian-mkdocs/generate)
    - In this step, give a name to your repository. By default your notes will be published at `<https://username.github.io/repo-name/>`
    - You need to copy only the `main` branch while create the repo from the template
2. Clone the repository you generated into your Obsidian folder/vault.
3. Move the notes you would like to make public to the `repo-name/docs` folder.
    - Easiest way to do this would be using drag and drop within Obsidian
4. Commit and push the changes. Github actions will publish your notes using [MkDocs](https://www.mkdocs.org/), with the [Material theme](https://squidfunk.github.io/mkdocs-material/). 

**Not working for you?** Open an [issue](https://github.com/jobindj/obsidian-mkdocs/issues/new/choose) and let me know what went wrong.

## Configuring your website

### How do I arrange notes as sections and pages?

By default, the sections and pages will follow the folder structure within `/docs`. The folders and sub-folders will show up as sections. Try not to have white spaces in your folder and file names, as these will be converted to HTML links. The webpage heading will be the same as the first-level heading in the markdown note.

- If you would like to arrange the pages manually, then use the `nav` option in the `mkdocs.yml` [configuration file](https://www.mkdocs.org/#adding-pages) at the root of this repo  to set custom page navigation.
    - For example, see the setup for [the Blue Book](https://lyz-code.github.io/blue-book/) at [github](https://github.com/lyz-code/blue-book/blob/master/mkdocs.yml). Managing each page using `nav` can become cumbersome as the number of notes increase though!
- The Materials theme provides multiple options to arrange [sections](https://squidfunk.github.io/mkdocs-material/setup/setting-up-navigation/#navigation-sections), use [navigation tabs](https://squidfunk.github.io/mkdocs-material/setup/setting-up-navigation/#navigation-tabs), and many other helpful [navigation setups](https://squidfunk.github.io/mkdocs-material/setup/setting-up-navigation/)

## Alternatives

- [kmaasrud/oboe](https://github.com/kmaasrud/oboe): tool to convert an Obsidian vault into a static directory of HTML files.
- [Jackiexiao/foam-mkdocs-template](https://github.com/Jackiexiao/foam-mkdocs-template): template for Obsidian/Foam using mkdocs/mkdocs-material/mkdocs-roamlinks-plugin
- [foambubble/foam-template](https://github.com/foambubble/foam-template): Foam workpace template