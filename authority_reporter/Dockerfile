FROM python:2.7
ENV PYTHONUNBUFFERED 1

RUN git clone https://github.com/relwell/WikiaAuthority.git /wikia_authority
WORKDIR /wikia_authority
RUN git checkout $COMMIT

RUN pip install -r requirements.txt

RUN python setup.py install
WORKDIR /wikia_authority/AuthorityReporter