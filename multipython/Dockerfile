FROM cimg/python:3.9.13
USER root
RUN apt-get update && apt-get install -y libopenblas-dev
USER circleci
RUN pyenv install 3.7.13
RUN pyenv install 3.8.13
RUN pyenv install 3.10.4
