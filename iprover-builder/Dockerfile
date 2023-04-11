FROM ocaml/opam:debian-11-ocaml-4.14-flambda
USER root
RUN apt-get -qq update
RUN apt-get -qqy install libgmp-dev python3 zlib1g-dev
USER opam
RUN opam install -qy ocamlfind ocamlgraph z3 zarith yojson
