FROM cimg/python:3.10.7
RUN cd /home/circleci/.pyenv/plugins/python-build/../.. && git pull && cd -
RUN pyenv install 3.7.15
RUN pyenv install 3.8.15
RUN pyenv install 3.9.15
RUN pyenv install 3.11.0
