FROM alpine:3.10

RUN apk add --update py2-pip

COPY requirements.txt /user/src/app/
RUN pip install --no-cache-dir -r /user/src/app/requirements.txt

COPY app.py /user/src/app/
COPY templates/index.html /user/src/app/templates/

EXPOSE 5000

CMD ["python", "/user/src/app/app.py"]