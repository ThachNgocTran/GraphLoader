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

## Development Environment

+ Vis.js Network v4.21 (https://visjs.org/).
+ Papa CSV Parser v5.0.2 (https://www.papaparse.com/).
