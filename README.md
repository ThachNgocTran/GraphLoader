# GraphLoader
A **client-side Graph Loader** for visualization purposes.

## Introduction

The site can be reached at [GraphLoader](https://thachngoctran.github.io/GraphLoader/).

The CSV file should have the following columns: `Source`, `Target`, `SourceType`, `TargetType`, `SourceId`, `TargetId`, `LinkType`.

The meaning of each column is self-explanatory. Nevertheless, an example is:

| Source        | Target                | SourceType  | TargetType    | SourceId      | TargetId  | LinkType  |
| ------------- |:---------------------:| -----------:| -------------:| -------------:| ---------:| ---------:|
| Finance.xls   | SummaryTemplate.xls   | File        | File          | fh24382       | keef49t   | REFER_TO  |
| Revenue.xls   | SummaryTemplate.xls   | File        | File          | 3uh2k3f       | keef49t   | REFER_TO  |

The graph is *interactive* (drag-drop, highlight, zoom in/out).

By default, the drawn graph's size is approximately the viewport of the site, which can be challenging to see individual nodes in case of having a large graph. Thus, users can reset the size of the graph to, e.g. '4000px' or '3000px 4000px' (width x height). The graph can also be saved into a static image, *given its current size*. The resizing is most meaningful for saving into static images.

## Development Environment

+ Vis.js Network v4.21 (https://visjs.org/).
+ Papa CSV Parser v5.0.2 (https://www.papaparse.com/).
