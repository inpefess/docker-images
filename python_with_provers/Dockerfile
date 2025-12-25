FROM inpefess/multipython:3.14
# Vampire
RUN wget https://github.com/vprover/vampire/releases/download/v5.0.0/vampire-Linux-X64.zip -O vampire.zip
RUN unzip vampire.zip
RUN rm vampire.zip
RUN mv vampire ${HOME}/.local/bin
RUN chmod u+x ${HOME}/.local/bin/vampire
# iProver
RUN wget https://gitlab.com/korovin/iprover/-/jobs/artifacts/master/download?job=build -O iprover.zip
RUN unzip iprover.zip
RUN mv iprover-build/iproveropt ${HOME}/.local/bin/iproveropt
RUN rm -rf iprover-build iprover.zip
RUN chmod u+x ${HOME}/.local/bin/iproveropt
