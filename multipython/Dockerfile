FROM cimg/python:3.13.8
USER root
RUN apt-get update && apt-get install -y libenchant-2-2
USER circleci
RUN cd /home/circleci/.pyenv/plugins/python-build/../.. && git pull && cd -
RUN pyenv install 3.10.18
RUN pyenv install 3.11.13
RUN pyenv install 3.12.11
RUN pyenv install 3.14.0
