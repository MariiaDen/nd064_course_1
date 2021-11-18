FROM python:2.7
LABEL maintainer="Mariia Denysenko"

WORKDIR /app
COPY ./techtrends/requirements.txt ./
COPY ./techtrends ./

RUN pip install -r requirements.txt
RUN python init_db.py

EXPOSE 3111

CMD ["python", "app.py"]