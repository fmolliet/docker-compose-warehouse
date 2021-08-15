FROM python:3.7.8-slim

RUN pip install --no-cache-dir matplotlib pandas flask requests numpy sklearn

WORKDIR /USR/APP

COPY . . 

EXPOSE 5000
CMD ["python", "server.py"]