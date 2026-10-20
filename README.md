# bfunctions package
This is a package that contains some basic LaTeX functions that I use often in my projects and I decided to put together to reduce the size of my preamble and so that I can import them directly to any locally-run LaTeX project.

## Made by: Sergio Martín Nieto
### Contact email: [sergiomartinnieto13@gmail.com](sergiomartinnieto13@gmail.com)
If you find any problems with the package or you have suggestions to improve its functionality, feel free to contact me. 

## Installation
### Overleaf
To get the package to work in Overleaf, dowload the `.sty` file. Then, you have two options. Either you create a new file and paste the contents inside every new project you create, or you create a `New Project` in overleaf whose only file is `bfunctions.sty`. Then click on `New file` -> `From another project` and browse your Overleaf projects until you find `bfunctions.sty` and import it.

### Windows
The steps to run the package locally depend on the distribution you use.

#### MikTeX
Create a folder inside your user folder and call it `texmf`. Create the following structure `User\texmf\tex\latex\bfunctions` and place the `bfunctions.sty` file inside the latter. Then go to MikTeX, `Settings -> Directories` and add the `bfunctions` folder. Finally go to `Tasks` and click on `Refresh file name database`. Now you should be able to call `\usepackage{bfunctions}` inside any project.

See [this link](https://miktex.org/kb/texmf-roots) for more details.

#### TeX Live
Create the same folders as in the previous steps and run the following command inside a command line `mktexlsr`.

### MacOS / Linux
Inside a termninal, run 

```mkdir -p ~/Library/texmf/tex/latex/bfunctions```

to create a folder as above, and create the `bfunctions.sty` file inside that folder as above. Then run `mktexlsr` in the terminal.

See the following [Tex Stack Exchange](https://tex.stackexchange.com/questions/1137/where-do-i-place-my-own-sty-or-cls-files-to-make-them-available-to-all-my-te/1138#1138) for more details on the installation process.

## Detailed explanation
The package can be called with two options: `language` and `font`. The `font` is either `mathb` or `bold`. This controls one of the functions of the package, which is to insert the symbols of some commonly used sets (real, natural, rational numbers etc) faster. Calling the package with the option `mathb` will use the `mathbb` font to display these sets. Then, to get $\mathbb{R}$, one symply types `\R`. Calling the package with the bold font displays `\R` as $\mathbf{R}$




