ARG url_pypi=https://pypi.org/simple/
ARG url_docker=docker.io

FROM ${url_docker}/python:3.12.6-slim-bookworm
ARG url_pypi
ENV url_pypi=${url_pypi}

WORKDIR /app

COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt --index-url ${url_pypi}

COPY . .

CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]