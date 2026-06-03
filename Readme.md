## What?

Node_prune is a small tool to prune unnecessary files from ./node_modules, such as markdown, typescript source files, and so on. Primarily built for [Up](https://github.com/apex/up) which lets you deploy serverless web applications in seconds.

## Installation

From [gobinaries.com](https://gobinaries.com):

```sh
$ curl -sf https://gobinaries.com/drylikov/Node_prune | sh
```

From source:

```
$ go get github.com/drylikov/Node_prune
```

## Usage

In your app directory:

```
$ Node_prune

files total 27,330
files removed 3,990
size removed 13 MB
   duration 200ms
```

Somewhere else:

```
$ node-prune path/to/node_modules

files total 27,330
files removed 3,990
size removed 13 MB
   duration 200ms
```

Or add to the ``package.json`` scripts field

```
  "scripts": {
    "postinstall": "Node_prune"
  }
```

## Why?

![huge](https://pbs.twimg.com/media/DEIV_1XWsAAlY29.jpg)

---
