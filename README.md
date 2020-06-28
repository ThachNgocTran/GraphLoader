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

## Extensibility

In the `icons` folder, there are a few icons used to draw the nodes, e.g. when `LinkType` is `Database`, the icon `Database.png` will be used. Given a new unknown `LinkType`, the icon `question.png` is used.

One way to extend the icon set is to check out this repository to local disk, then add more icons as needed. Mount a web server, e.g. `python -m http.server 8080` and access the site as `http://localhost:8080/`.

## Development Environment

+ Vis.js Network v4.21 (https://visjs.org/).
+ Papa CSV Parser v5.0.2 (https://www.papaparse.com/).

## Sample Run

![Sample Run](/SampleRun.png)
