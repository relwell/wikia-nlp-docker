FROM python:2.7
ENV PYTHONUNBUFFERED 1

RUN git clone https://github.com/Wikia/WikiaAuthority.git /wikia_authority
WORKDIR /wikia_authority
RUN git checkout $COMMIT

RUN pip install gunicorn
RUN pip install -r requirements.txt
RUN pip install celery
RUN pip install flower

RUN python setup.py install
