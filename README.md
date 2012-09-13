# lein-gnome

A Leiningen plugin using using ClojureScript to create native Gnome3 applications.

## Status - Currently informational only - no working code.

## Libraries required (Ubuntu)

Fixme: verify/update details.

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

FIXME: and add an example usage once we get some working code:

    $ lein gnome

## Reference

### Gnome Javascript engine and bindings page
https://live.gnome.org/Gjs

### Gnome Javascript examples
http://git.gnome.org/browse/gjs/tree/examples

gtk.js is the first one I successfully translated.

### Tutorials for just about everything javascript on Gnome
http://developer.gnome.org/gnome-devel-demos/3.5/js.html.en

### Best Code References I've found
http://www.roojs.com/seed/gir-1.2-gtk-3.0/gjs/Gtk.Application.html

## Notes

There are two Javascript bindings to gnome.  gjs based on Mozilla
SpiderMonkey, and seed based of Webkit.  See
https://live.gnome.org/GObjectIntrospection/BindingsDocumentation for
more details.

Note that some of the above documentation is from seed projects, and
so isn't quite what we need, (I'm assuming gjs, for the moment), but
is very close.  Be aware.

## License

Copyright © 2012 Jason Whitlark(jason@whitlark.org)

Distributed under the Eclipse Public License, the same as Clojure.
