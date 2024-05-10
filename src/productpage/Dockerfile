FROM python:3.8-slim

WORKDIR /usr/src/app

COPY . .

# Install dependencies
RUN apt-get update && \
    apt-get install -y curl && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/* && \
    pip install --no-cache-dir -r requirements.txt


EXPOSE 9080

ENV NAME ProductPage

CMD ["python", "productpage.py", "9080"]
