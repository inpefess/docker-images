FROM inpefess/multipython:latest
RUN wget https://github.com/vprover/vampire/releases/download/v4.7/vampire4.7.zip -O vampire.zip
RUN unzip vampire.zip
RUN rm vampire.zip
RUN mv vampire_z3_rel_static_HEAD_6295 ${HOME}/.local/bin/vampire
RUN chmod u+x ${HOME}/.local/bin/vampire
