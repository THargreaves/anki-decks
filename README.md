# Anki Decks

_Anki decks for revision and code memorisation._

## Collaboration Instructions

### Prerequisities

To contribute to these decks you will need installations of the following:

- [Anki Desktop](https://apps.ankiweb.net/)
- [Git Bash](https://gitforwindows.org/) (or the MacOS, Linux equivalent)

### Setup

- Open Git Bash in the location you would like to store your Anki decks by right-clicking in the File Explorer
- Run `git clone https://github.com/THargreaves/anki-decks.git "Anki Decks"` to clone this repository
- Install the [Mini Format Pack](https://ankiweb.net/shared/info/295889520) add-on

### Importing New Cards

- Open Git Bash inside of your local clone of the repository
- Ensure that your copy of the repository is up to date by running `git pull` (you may need to commit your changes first, see below)
- In Anki, use `File > Import...` and select the deck to update. Leave all parameters as defaults apart from allowing HTML in fields (bullet points).

### Updating Cards

- As above but select "Update existing notes..." in dropdown

### Creating New/Modifying Cards

- Edit card using Anki. Make sure to use appropriate tagging
- Confirm your additions/changes are correct by browsing the deck and previewing modified notes
- Export updated deck using `File > Export...` as format "Notes in Plain Text". Include only the deck you've made changes to and include tags/HTML
- Overwrite the existing note `.txt` file with the output
- Open Git Bash in the repository clone
- Check your changes have been made with `git status`
- To stage all change, use `git add .`. Otherwise (preferred), stage a single file with `git add path/to/file`
- Commit changes using `git commit -m "{Message explaining changes in imperative voice}"` (If you forget to add the `-m` flag, Vim will open. Exit this using `:q!`)
- Push changes using `git push`. If this fails, you may need to merge first using `git pull` then `:wq` to close Vim. If this fails, contact me 

Note: by default, Git uses Vim as its text editor. This is quite unfriendly for newcomers and can be changed to the more intuitive Nano using

```
git config --global core.editor "nano"
```

### Card Format

Cards are written using [MathJax](https://www.mathjax.org/). You can create inline maths using `\(...\)` and a math block using `\[...\]`. Most MathJax features are taken directly from LaTeX so you can using LaTeX guides for support.

Bullet points can be entered using the Mini Format Pack.

Tags should be lower case and hyphenated if multi-word.

## Further Resources

- [Anki documentation](https://docs.ankiweb.net/#/)
- [Basic Git tutorial series](https://www.youtube.com/playlist?list=PL-osiE80TeTuRUfjRe54Eea17-YfnOOAx)
- [Interactive Vim tutorial](https://www.openvim.com/)
