# example_rmd

Example of using Rmarkdown to generate a report using [gapminder](https://www.gapminder.org/) data.

## Data

The gapminder data is stored as CSV file in `data/gapminder.tsv`.

## Summary of what the code does

The code in the Rmarkdown file (`report.Rmd`) loads the gapminder data, cleans the data, builds a model of life expectancy by year for each country in the dataset, then plots the estimated increase in life expectancy per year as a barplot.

## Generating the report

The first time you open this project, you will need to install packages with `renv`:

```r
renv::restore()
```

Next, make the report:

```r
rmarkdown::render("report.Rmd")
```

The report will be saved as "report.docx". You can open it MS Word.

## Licenses

- Gapminder data: [Creative Commons (CC) Attribution 3.0 Unported license](https://creativecommons.org/licenses/by/3.0/) (see their [terms of use](https://www.gapminder.org/privacy/terms-of-use/)).

- Other content: [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/)
