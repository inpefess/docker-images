FROM inpefess/multipython:latest
RUN wget https://github.com/vprover/vampire/releases/download/v4.7/vampire4.7.zip -O vampire.zip
RUN unzip vampire.zip
RUN rm vampire.zip
RUN mv vampire_z3_rel_static_HEAD_6295 ${HOME}/.local/bin/vampire
RUN chmod u+x ${HOME}/.local/bin/vampire
RUN wget https://gitlab.com/api/v4/projects/39846772/jobs/artifacts/2023.04.10/download?job=build-job -O iprover.zip
RUN unzip iprover.zip
RUN mv iproveropt ${HOME}/.local/bin/iproveropt
RUN chmod u+x ${HOME}/.local/bin/iproveropt
