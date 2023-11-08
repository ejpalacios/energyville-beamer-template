# EnergyVille LaTeX Beamer template

LaTeX Beamer style following (as close as possible) the official EnergyVille MS Powerpoint template.

> This template was produced for personal use and it is provided as it is. Contributions are welcome.

## Usage

### Selecting the mother institution logo

To select the logo of the mother institution the options are:

- `kul` for KU Leuven
- `vito` for VITO
- `imec` for IMEC
- `uhasselt` for UHasselt

Example:

```LaTeX
\usetheme[kul]{energyville}
```

### Display table of contents before each section

To display the progress in the table of contents before each section the option `tocsection` can be used as:

```LaTeX
\usetheme[kul, tocsection]{energyville}
```

### Title page logos

By default, the title page defines `titlegraphic` as EnergyVille logo. A custom graphic can be defined with:

```LaTeX
\titlegraphic{ \includegraphics[height=45px]{mytitlelogo.png} }
```

If you would like to keep both logos, the following snippet can be used.

```LaTeX
\titlegraphic{
    \hfill
    \includegraphics[height=45px]{graphics/energyville}
    \hspace{40px} % you might need to adjust this space
    \includegraphics[height=45px]{mytitlelogo.png}
    \hfill
}
```

### Additional commands

Three additional commands are provided in the template.

Text indicating the level of confidentiality (will appear on the bottom left)

```LaTeX
\confidentiality{Confidential}
```

Logo of the project (will appear on the top right)

```LaTeX
\projectlogo{\includegraphics[height=15px]{graphics/project}}
```

Logo of the funding body (will appear on the top right under the project logo)

```LaTeX
\fundinglogo{\includegraphics[height=15px]{graphics/funding}}
```
