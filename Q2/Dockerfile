FROM mcr.microsoft.com/mmlspark/release:latest

RUN apt-get update && apt-get install -y git && pip install notebook

WORKDIR /app

EXPOSE 8888

ENV JUPYTER_TOKEN=''

CMD ["sh", "-c", "jupyter notebook --ip=0.0.0.0 --port=$PORT --no-browser --allow-root --NotebookApp.token=''"]

