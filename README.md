# lein-gnome

A Leiningen plugin using using ClojureScript to create native Gnome3 applications.

## Status - Currently informational only - no working code.

## Libraries required (Ubuntu)

 - build-essential
 - gjs (dev?)
 - ???

## TODO

 - Check if necessary source libraries are installed
 - Generate wrapper library from gjs xml descriptions
 - make resources/icons
 - add build logic
 - fix run and test - (work around imports and *print-fn* stuff)
 - ensure clj 1.4?
 - add package step that wraps it all up
 - add upload to ppa step

Commands: gen-wrapper, run, test?, package, upload-ppa?

## Someday

seesaw like wrapper for Gnome3 library.

## Usage

Put `[lein-gnome "0.1.0-SNAPSHOT"]` into the `:plugins` vector of your project.clj.

FIXME: and add an example usage that actually makes sense:

    $ lein gnome

## License

Copyright © 2012 Jason Whitlark(jason@whitlark.org)

Distributed under the Eclipse Public License, the same as Clojure.
