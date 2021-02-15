# graph-explorer
POC demo for graph visualization platform

## Usage

1. Start web app via Python SimpleHTTPServer or http.server

For Python 2.X

```
$ python -m SimpleHTTPServer
```

For Python 3.X

```
$ python -m http.server
```

Output:

```
Serving HTTP on 0.0.0.0 port 8000 ...
```

2. Access via URL (preferred browser: Google Chrome): 

```
http://localhost:8000
```

## Loading GEXF file

Required file format: GEXF (Graph Exchange XML Format)
Link: https://gephi.org/gexf/format/viz.html

1. Place gexf file in `graph-explorer/data` directory

2. Load file via the upload button in UI

## Loading GEXF file on Startup

Modify initial gexf file in `config.js` file

1. Edit `graph-explorer/config.js`

2. Change graphFile value:

```
GexfJS.setParams({
    graphFile : "data/miserables.gexf",
    ...
    ...
 ```
