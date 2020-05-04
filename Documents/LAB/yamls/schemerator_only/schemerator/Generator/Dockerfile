FROM python:3

# the docker build needs to run from the home schemerator directory. i dont know how to fix it
COPY Generator/ /home/Generator/
COPY SharedUtils/ /home/SharedUtils/

WORKDIR /home/Generator/

ENV PYTHONPATH /home/

RUN pip install -r /home/Generator/requirements.txt &&
    chmod -R 777 /home/db

CMD ["python", "/home/Generator/main.py"]
