FROM python:latest
WORKDIR /app
COPY . .
RUN pip3 install -r requirements.txt
# ENV DB_HOST=database-1.cih2s8syc3z0.us-east-1.rds.amazonaws.com
# ENV DB_USER=admin
# ENV DB_PASSWORD=Root1234
# ENV DB_NAME=dev

CMD ["python3" ,"app.py"]


