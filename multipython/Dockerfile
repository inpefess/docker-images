FROM cimg/python:3.11.5
USER root
RUN apt-get update && apt-get install -y libenchant-2-2
USER circleci
RUN cd /home/circleci/.pyenv/plugins/python-build/../.. && git pull && cd -
RUN pyenv install 3.8.18
RUN pyenv install 3.9.18
RUN pyenv install 3.10.13
RUN pyenv install 3.12.0
