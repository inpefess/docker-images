FROM ocaml/opam:debian-11-ocaml-4.14-flambda
USER root
RUN apt-get -qq update
RUN apt-get -qqy install libgmp-dev python3 zlib1g-dev cmake
USER opam
RUN opam install -qy ocamlfind ocamlgraph z3 zarith yojson
RUN git clone https://github.com/Z3Prover/z3
WORKDIR /home/opam/z3
RUN git checkout z3-4.12.2
RUN mkdir build
WORKDIR /home/opam/z3/build
RUN cmake -DCMAKE_BUILD_TYPE=Release -DZ3_BUILD_LIBZ3_SHARED=FALSE ..
RUN make
WORKDIR /home/opam
