# Running

// figure out relative volumes
docker run -it --rm -p 8080:8080 -v C:\pluralsight\wiremock:/home/wiremock --name wiremock wiremock/wiremock:2.35.0 --verbose --local-response-templating

# View Stubs
http://localhost:8080/__admin/mappings

# View Requests
http://localhost:8080/__admin/requests
