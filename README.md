
# Shiny-phyloseq

[Shiny-phyloseq](http://joey711.github.io/shiny-phyloseq/)
is an interactive web application that provides 
a graphical user interface to the microbiome analysis package for R,
called [phyloseq](http://joey711.github.io/phyloseq/).
For details about using the phyloseq package directly,
see [The phyloseq Homepage](http://joey711.github.io/phyloseq/).

## Citation
Shiny-phyloseq is provided under a free-of-charge, open-source license (A-GPL3).
All we require is that you cite/attribute the following
in any work that benefits from this code or application.

### The App

McMurdie and Holmes (2014) Shiny-phyloseq: Web Application for Interactive Microbiome Analysis with Provenance Tracking. *Submitted*.

### "Under the Hood"

McMurdie and Holmes (2013)
[phyloseq: An R package for reproducible interactive analysis and graphics of microbiome census data](http://dx.plos.org/10.1371/journal.pone.0061217). 
PLoS ONE 8(4):e61217.

## Launching Shiny-phyloseq Local Session

While it is possible to host the server "back end" somewhere
so that users only need to point their web browser to a link,
the following instructions apply to running both the back and front "ends" on your local machine.
The server back end will be an R session on your own machine,
while the front end is your web browser, pointed to the appropriate local URL.

### Auto-Install/Launch Shiny-phyloseq (Recommended)

Simply launching Shiny-phyloseq should also install missing/old packages.

The following R code will launch Shiny-phyloseq on most systems.


```r
install.packages("shiny")
shiny::runGitHub("shiny-phyloseq","joey711")
```

See the [Shiny-phyloseq installation instructions](http://joey711.github.io/shiny-phyloseq/Install.html),
for further details.


### Launch using RStudio's IDE

Alternatively, you can launch a Shiny app from within RStudio.
This is not necessary if you launch the app using the R code above.

See the "[Running an App](http://shiny.rstudio.com/tutorial/lesson1/)" section 
of [the Shiny Tutorials](http://shiny.rstudio.com/tutorial).

If you are using RStudio (recommended) you can 
launch Shiny-phyloseq with the click of a button
after opening one of the main source files (e.g. `server.R`)
in the Shiny-phyloseq directory.
Note that the best behavior (uploads, downloads, etc.)
comes from **not-using the RStudio built-in browser**,
but instead clicking the "open in browser" button at the top. 

Your default browser will then open at the live (local) URL. Then click away!

Brief steps:

1. (Re)start RStudio by opening `server.R` or `ui.R`
2. Click the "Run App" button that appears.
3. Click the "Open in Browser" button above the new RStudio window that just launched.

Note that any R installation/session can launch a Shiny app.
For alternative launch methods that don't use RStudio,
see "[Running an App](http://shiny.rstudio.com/tutorial/lesson1/)".
