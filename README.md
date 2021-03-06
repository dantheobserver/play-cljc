## Introduction

A library for making games that run in both OpenGL and WebGL. There's no black box `wasm` trickery going on here; just good old fashioned [cljc files](https://clojure.org/guides/reader_conditionals), some macro magic, and absolutely zero social life. Every coffee shop barista near me agrees that this game library is basically the greatest one ever. Other game libraries? Total disasters! Everyone agrees. Believe me.

## Getting Started

You can generate a new project with the [The Clojure CLI Tool](https://clojure.org/guides/getting_started#_clojure_installer_and_cli_tools):

`clj -Sdeps '{:deps {leiningen {:mvn/version "2.9.0"}}}' -m leiningen.core.main new play-cljc hello-world`

This will start you off with a little platformer. It will contain a README with all the commands you need to use. To make music, [edna](https://github.com/oakes/edna) is a good companion library, and the template above is preconfigured with it.

## Documentation

* Check out [the example games](https://github.com/oakes/play-cljc-examples)
* Read [the dynadocs](https://oakes.github.io/play-cljc/cljs/play-cljc.gl.core.html)
  * Check out the interactive [2D](https://oakes.github.io/play-cljc/cljs/play-cljc.gl.examples-2d.html) and [3D](https://oakes.github.io/play-cljc/cljs/play-cljc.gl.examples-3d.html) examples
* Join the discussion on [r/playcljc](https://www.reddit.com/r/playcljc/)
* Watch my [intro screencast](https://www.youtube.com/watch?v=y6WpUdECwmA)

## Development

* Install [the Clojure CLI tool](https://clojure.org/guides/getting_started#_clojure_installer_and_cli_tools)
* To develop the web version with figwheel: `clj -A:dev dev.clj`
* To develop the native version: `clj -A:dev dev.clj native`
  * On Mac OS, you will need to run `clj -A:dev -J-XstartOnFirstThread dev.clj native`
* To install the release version: `clj -A:prod prod.clj install`

## Licensing

All files that originate from this project are dedicated to the public domain. I would love pull requests, and will assume that they are also dedicated to the public domain.
