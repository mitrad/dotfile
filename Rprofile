## Don't ask me for my CRAN mirror every time
#options("repos" = c(CRAN = "http://cran.revolutionanalytics.com/"))
options("repos" = c(CRAN = "https://cran.rstudio.com/"))

options(digits.secs=2)              # show sub-second time stamps
options(max.print=500)             # do not print more than 1000 lines
options(digits=4, show.signif.stars=FALSE)

# From http://kevinushey.github.io/blog/2015/02/02/rprofile-essentials/
# warn on partial matches
#options(warnPartialMatchAttr = TRUE,
#        warnPartialMatchDollar = TRUE,
#        warnPartialMatchArgs = TRUE)

# enable autocompletions for package names in
# `require()`, `library()`
utils::rc.settings(ipck = TRUE)

# warnings are errors
#options(warn = 2)

# fancy quotes are annoying and lead to
# 'copy + paste' bugs / frustrations
options(useFancyQuotes = FALSE)

## Set output width & digits number
## options(width = 80, digits = 5)


## If you ever delete all objects in your global environment, then the aliases above will also be deleted. You can prevent that by hiding these in an environment.

.startup <- new.env()
assign("h", utils::head, envir = .startup)
assign("n", base::names, envir = .startup)
assign("ht", function(d) rbind(head(d,6),tail(d,6)) , envir = .startup)
assign("s", base::summary, envir = .startup)
attach(.startup)

## .First() run at the start of every R session.
#.First <- function() {
#  Sys.setlocale(category = "LC_ALL", locale = "en_US.UTF-8")
#  Sys.setenv(LANG = "en_US.UTF-8", LC_CTYPE = "en_US.UTF-8")
#  Sys.setlocale("LC_MESSAGES", "en_US.UTF-8")
#  cat("\nSuccessfully loaded .Rprofile at", date(), "\n")
#}

