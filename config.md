+++
author = "Fredrik Ekre"
prepath = "FerriteCon"

ignore = ["node_modules/"]
generate_rss = false
+++

\newcommand{\note}[1]{@@note @@title ⚠ Note@@ @@content #1 @@ @@}
\newcommand{\collaps}[2]{
~~~<button type="button" class="collapsible">~~~ #1 ~~~</button><div class="collapsiblecontent">~~~ #2 ~~~</div>~~~
}