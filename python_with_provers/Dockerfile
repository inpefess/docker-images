FROM inpefess/multipython:3.14
# Vampire
RUN wget https://github.com/vprover/vampire/releases/download/v5.0.0/vampire-Linux-X64.zip -O vampire.zip
RUN unzip vampire.zip
RUN rm vampire.zip
RUN mv vampire ${HOME}/.local/bin
RUN chmod u+x ${HOME}/.local/bin/vampire
# iProver
RUN wget https://gitlab.com/api/v4/projects/39846772/jobs/artifacts/2025.03.10/download?job=build-job -O iprover.zip
RUN unzip iprover.zip
RUN rm iprover.zip
RUN mv iproveropt ${HOME}/.local/bin/iproveropt
RUN chmod u+x ${HOME}/.local/bin/iproveropt
