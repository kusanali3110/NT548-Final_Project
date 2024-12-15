# Base image
FROM mongo:6.0

# Copy JSON file into container
COPY dummy_statistics.json /tmp/dummy_statistics.json

# Import data from JSON file
CMD ["sh", "-c", "mongoimport --uri 'mongodb://mongo-service.mongodb.svc.cluster.local:27017/covid-19' --collection covid_statistics --file /tmp/dummy_statistics.json"]