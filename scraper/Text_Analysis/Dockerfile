FROM fokkodriesprong/docker-pyspark

ENV http_proxy http://wwwproxy.unimelb.edu.au:8000
ENV https_proxy http://wwwproxy.unimelb.edu.au:8000

RUN mkdir /workspace
WORKDIR /workspace
ADD . /workspace

RUN pip install -r docker_requirements.txt

CMD [ "python", "./stream_analyzer.py"]