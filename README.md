# Willkommen!

Dies ist eine wiki-artige Dokumentation zu Website ([vcp-mitteldeutschland.de](https://www.vcp-mitteldeutschland.de)) und Öffentlichkeitsarbeit im VCP Mitteldeutschland (Stand Frühjahr 2023). Zielsetzung ist, 

* bisherige Absprachen und Workflows festzuhalten 
* neuen Mitarbeitenden auf Landesebene einen einfachen Einstieg in die Arbeit mit der Website zu ermöglichen. 

Falls die Kapazitäten ausreichen, sollen zudem

* Tipps zur Öffentlichkeitsarbeit und
* ein Veranstaltungsleitfaden 

implementiert werden. 

## Box mit Warnung

Mit der Syntax 

```
::: {.warnung}
Hier kommt der Text.
:::
```

kann eine Box mit rotem linken Rand ausgegeben werden. Sie ist für Warnungen gedacht.

## Hervorhebung von Wörtern

Einzelne Wörter und Textpassagen können mit `<span class="hl"> Hervorgehoben </span>` hervorgehoben werden (gelber hintergrund, braune Schrift).



## Markdown-Syntax

Die Markdown-Syntax ist sehr einfach und intuitiv - das ist ihr Vorteil. Eine nützliche Übersicht mit den allerwichtigsten Befehlen bietet der Wikipedia-Artikel zu Markdown: [Hier geht's lang!]([Markdown – Wikipedia](https://de.wikipedia.org/wiki/Markdown#Auszeichnungsbeispiele "Yeah, Markdown!")









# Credits

Das Projekt basiert auf **R Markdown** and **bookdown** (https://github.com/rstudio/bookdown). 

### Weitere Informationen:

* Das Buch zu **bookdown**: https://bookdown.org/yihui/bookdown/
* Die **bookdown**-Package-Website: https://pkgs.rstudio.com/bookdown

# Additional Information - How to handle bookdown

> aus der ursprünglichen index-Datei kopiert
> This is a _sample_ book written in **Markdown**. You can use anything that Pandoc's Markdown supports; for example, a math equation $a^2 + b^2 = c^2$.

## Usage

Each **bookdown** chapter is an .Rmd file, and each .Rmd file can contain one (and only one) chapter. A chapter *must* start with a first-level heading: `# A good chapter`, and can contain one (and only one) first-level heading.

Use second-level and higher headings within chapters like: `## A short section` or `### An even shorter section`.

The `index.Rmd` file is required, and is also your first book chapter. It will be the homepage when you render the book.

## Render book

You can render the HTML version of this example book without changing anything:

1. Find the **Build** pane in the RStudio IDE, and

2. Click on **Build Book**, then select your output format, or select "All formats" if you'd like to use multiple formats from the same book source files.

Or build the book from the R console:

```{r,
bookdown::render_book()
```

To render this example to PDF as a `bookdown::pdf_book`, you'll need to install XeLaTeX. You are recommended to install TinyTeX (which includes XeLaTeX): <https://yihui.org/tinytex/>.

## Preview book

As you work, you may start a local server to live preview this HTML book. This preview will update as you edit the book when you save individual .Rmd files. You can start the server in a work session by using the RStudio add-in "Preview book", or from the R console:

```{r
bookdown::serve_book()
```

```{r
# automatically create a bib database for R packages
knitr::write_bib(c(
  .packages(), 'bookdown', 'knitr', 'rmarkdown'
), 'packages.bib')
```
