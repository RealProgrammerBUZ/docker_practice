FROM python:3.8
RUN apt update && apt install python -y

WORKDIR /app

COPY ./ ./

EXPOSE 8888

CMD ["python", "./project/test.py"]