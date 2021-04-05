# Publish Obsidian Notes with MkDocs (template)

## How to get started?

1. Create a new github repository using [this template](https://github.com/jobindj/obsidian-mkdocs/generate)
    - Give a name to your public notes repository in this step. By default your notes will be published your public notes will be available at `<https://username.github.io/repo-name/>`
    - You need to copy only the `main` branch while create the repo from the template
2. Clone the repository you generated into your Obsidian folder.
3. Move the notes you would like to make public to the `repo-name/docs` folder.
4. Commit and push the changes. Github actions will publish your notes using MkDocs, with the Material theme. 

## Configuring your website

### How do I arrange the section and pages?

By default, the sections and pages will follow the folder structure within `/docs`. 
- If you would like to arrange the pages manually, then use the `nav` option in the `mkdocs.yml` [configuration file to set the page navigation](https://www.mkdocs.org/#adding-pages).
    - For example, see the setup for [the Blue Book](https://lyz-code.github.io/blue-book/) at [github](https://github.com/lyz-code/blue-book/blob/master/mkdocs.yml). Managing each page using `nav` can become cumbersome when the number of your notes increase though!
- The Materials theme provides multiple options to arrange [sections](https://squidfunk.github.io/mkdocs-material/setup/setting-up-navigation/#navigation-sections), use [navigation tabs](https://squidfunk.github.io/mkdocs-material/setup/setting-up-navigation/#navigation-tabs), and many other helpful [navigation setups](https://squidfunk.github.io/mkdocs-material/setup/setting-up-navigation/)

## Alternatives

- [kmaasrud/oboe](https://github.com/kmaasrud/oboe): tool to convert an Obsidian vault into a static directory of HTML files.
- [Jackiexiao/foam-mkdocs-template](https://github.com/Jackiexiao/foam-mkdocs-template): template for Obsidian/Foam using mkdocs/mkdocs-material/mkdocs-roamlinks-plugin
- [foambubble/foam-template](https://github.com/foambubble/foam-template):Foam workpace template