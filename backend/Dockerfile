FROM python:latest
WORKDIR /app
COPY . .
RUN pip3 install -r requirements.txt

# --- Credentials (hardcoded for dev) -----------------------------------
# Baked directly into the image. Fine for a throwaway dev environment,
# but note: anyone who can pull or `docker history` this image can read
# these values back out, and they'll be committed if this Dockerfile
# goes into git. For anything beyond local dev, prefer passing these at
# runtime instead (`docker run --env-file backend/.env backend`) so they
# never end up in the image itself.
ENV DB_HOST=database-1.cih2s8syc3z0.us-east-1.rds.amazonaws.com
ENV DB_USER=admin
ENV DB_PASSWORD=Root1234
ENV DB_NAME=dev

CMD ["python3" ,"app.py"]


