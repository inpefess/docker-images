FROM inpefess/multipython:3.14
# Vampire
RUN wget https://github.com/vprover/vampire/releases/download/v4.9casc2024/vampire
RUN mv vampire ${HOME}/.local/bin
RUN chmod u+x ${HOME}/.local/bin/vampire
# iProver
RUN wget https://gitlab.com/api/v4/projects/39846772/jobs/artifacts/2025.03.10/download?job=build-job -O iprover.zip
RUN unzip iprover.zip
RUN rm iprover.zip
RUN mv iproveropt ${HOME}/.local/bin/iproveropt
RUN chmod u+x ${HOME}/.local/bin/iproveropt
