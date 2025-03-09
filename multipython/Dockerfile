FROM cimg/python:3.13.2
USER root
RUN apt-get update && apt-get install -y libenchant-2-2
USER circleci
RUN cd /home/circleci/.pyenv/plugins/python-build/../.. && git pull && cd -
RUN pyenv install 3.9.21
RUN pyenv install 3.10.16
RUN pyenv install 3.11.11
RUN pyenv install 3.12.9
