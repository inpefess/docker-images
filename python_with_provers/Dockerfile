FROM inpefess/multipython:latest
RUN wget https://github.com/vprover/vampire/releases/download/v4.8casc2023/vampire_z3_rel_static_casc2023_6749.zip -O vampire.zip
RUN unzip vampire.zip
RUN rm vampire.zip
RUN mv bin/vampire_z3_rel_static_casc2023_6749 ${HOME}/.local/bin/vampire
RUN rmdir ./bin
RUN chmod u+x ${HOME}/.local/bin/vampire
RUN wget https://gitlab.com/api/v4/projects/39846772/jobs/artifacts/2023.07.13/download?job=build-job -O iprover.zip
RUN unzip iprover.zip
RUN rm iprover.zip
RUN mv iproveropt ${HOME}/.local/bin/iproveropt
RUN chmod u+x ${HOME}/.local/bin/iproveropt
