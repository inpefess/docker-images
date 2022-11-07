FROM inpefess/testing_vampire:latest
USER root
RUN apt-get update && apt-get install -y opam
USER circleci
RUN opam init --disable-sandboxing
RUN opam switch create 4.14.0+flambda --package=ocaml-variants.4.14.0+options,ocaml-option-flambda
RUN eval $(opam env)
RUN opam update
RUN opam install -y ocamlfind ocamlgraph z3 zarith yojson
RUN git clone https://gitlab.com/korovin/iprover.git
WORKDIR /home/circleci/project/iprover
RUN git checkout 2022_sockets	  
RUN eval $(opam env); ./configure 
RUN eval $(opam env); make
RUN cp ${HOME}/project/iprover/iproveropt ${HOME}/.local/bin

