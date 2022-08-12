# Working with Tabtree files of Geroontology

Tabtree is a language/format convenient to use for coding OWL ontologies and knowledge graphs, as it makes code more compact and readable.

This manual will help you to install all the necessary tools, and commence a happy development of Geroontology through tabtree files.

## Short instruction

* Install Atom code editor
  * Add Tabtree plugin
* Install Git client
* Clone git repository from GitHub

## Detailed instruction

### Install and set up Atom

- Download and launch Atom installer [from here](https://atom.io/)

#### Set Light theme

I recommend to set the greyish-white background as the Tabtree syntax highlighter we install in the next step is optimized exactly for this color mode.

After downloading and installation of the Atom code editor, choose Light theme by these steps:
 - Press `Ctrl-,`
 - Choose `Themes`
 - In `UI Theme` and `Syntax Theme` choose `Atom Light`

#### Install Tabtree plugin

  - Press `Ctrl-,`
  - Choose `Install`
  - In the search field type in `tabtree`
  - Press `Install` button in `language-tabtree` bar

Now you've got something like this:

<img src="working_with_tabtree/atom_code_editor_1.png" alt="Tabtree with syntax highlighting" width=500px />

### Install Git client for Windows

#### Install Git support

- Download and run installer [from here](https://git-scm.com/download/win). Choose standalone installer, and most probably you would need 64-bit Git

#### Install GitHub Desktop - a Git client

- Download and run installer [from here](https://desktop.github.com/)
- Launch GitHub Desktop
- Choose `New` from the top menu
- Choose `Clone from URL`
- In `Source URL` type in Geroontology repository address: `git@github.com:prozion/geroontology.git`
- Choose folder where to upload the files from the repository
- Press `Clone`

### Open a project to work in Atom

Now, when you have downloaded Geroontology files, let's go back to Atom editor

- In the top menu: `File` - `Add Project Folder...`
- Navigate to the folder with downloaded repository and select this folder, press `Ok`

In the tree view pane you will see this folder with all the files inside it. You can double-click `geroontology/tabtree/geroontology.tree` to open the file and start working over ontology!

### Update ontology

To make changes accessible to the colleagues, you'll need:

- Make new commit
- Push it on github

While changes were made to geroontology.tree, at push Github launches translation script and saves resulted Turtle file into another git branch. [Check this file here.](https://github.com/prozion/geroontology/blob/builds/turtle/geroontology.ttl). This file is perfectly fitted to be imported into ontology applications, such as Protege.

<img src="working_with_tabtree/save_raw_ttl_file.png" alt="Save a raw Turtle file from GitHub" width=500px />

 Don't forget to download [a raw .ttl file](https://raw.githubusercontent.com/prozion/geroontology/builds/turtle/geroontology.ttl) rather than a webpage from GitHub.
