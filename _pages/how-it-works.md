---
ID: 2052
post_title: How it works
author: Eugene Bushtyrev
post_date: 2014-11-07 23:27:09
post_excerpt: ""
layout: page
permalink: >
  https://symbols.pro/symbol-server/how-it-works/
published: true
post-option:
  - '{"sidebar":"no-sidebar","left-sidebar":"Footer 1","right-sidebar":"Footer 1","page-style":"normal","show-title":"enable","page-caption":"","show-content":"enable","header-background":""}'
above-sidebar:
  - '[]'
content-with-sidebar:
  - |
    [{"item-type":"item","item-builder-title":"Content","type":"content","option":{"page-item-id":"","title-type":"none","title":"","caption":"","content":"[gdlr_process min_height=|gq2|300px|gq2| type=|gq2|vertical|gq2| ]|g1n||g1n|[gdlr_tab icon=|gq2|icon-rss|gq2| title=|gq2|Collecting symbols|gq2| ]|g1n||g1n|When your software is built, the compiler+linker produce different types of artifacts. Executable files are the part of your product itself and it is packed somehow and shipped as a |gq2|new build|gq2| to the team.|g1n||g1n|There are also the debug symbols - files, which are not needed for your customers, but still needed to you when you have to debug your software afterwards.|g1n||g1n|Symbol server provides the command line tool also called as Agent to collect symbols and other binary data.|g1n||g1n|Agent integrates into the build process, collects symbol files and/or executables and sends it to Symbol server.|g1n||g1n|[/gdlr_tab]|g1n||g1n|[gdlr_tab icon=|gq2|icon-flag|gq2| title=|gq2|Symbol processing|gq2| ]|g1n||g1n|Having received the data submission request from Agent, the Symbol server starts packing symbols and executables into the specific format, understandable by debuggers. It places the resulting files into appropriate place on the filesystem.|g1n||g1n|When all the files from the package have been processed, Symbol server checks the validity and correctness of data. This is done to ensure debuggers will really understand your data afterwards. If one of the checks goes wrong - the whole package is considered 'failed'. If all the checks have been passed, the package is 'good'.|g1n||g1n|The email notification is generated at the end of each package processing. Every notification carries the processing verdict and error description if something went wrong.|g1n||g1n|[/gdlr_tab]|g1n||g1n|[gdlr_tab icon=|gq2|icon-fire|gq2| title=|gq2|Exposing symbols|gq2| ]|g1n||g1n|Symbol server exposes processed data via HTTP(s) protocol into your intranet. You may also choose to use SMB share access instead of HTTP(s).|g1n||g1n|[/gdlr_tab]|g1n||g1n|[gdlr_tab icon=|gq2|icon-magic|gq2| title=|gq2|Consuming symbols|gq2| ]|g1n||g1n|When the developer attaches to a process or opens the crash dump, debuggers locate the Symbol server and download the appropriate symbols automatically.|g1n||g1n|This works for all the software which is Symbol server technology aware - for instance, Process Monitor or Xperf.|g1n||g1n|<span style=|gq2|font-size: 14px; line-height: 1.5em;|gq2|>[/gdlr_tab]</span>|g1n||g1n|[/gdlr_process]","margin-bottom":"20px"}}]
below-sidebar:
  - '[]'
---