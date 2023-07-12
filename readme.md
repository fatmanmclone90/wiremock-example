# Running

```
docker run -it --rm -p 8080:8080 -v ${PWD}:/home/wiremock --name wiremock wiremock/wiremock:2.35.0 --verbose --local-response-templating
```

To run in on a shared network to allow other containers to communicate

```
docker run -it --rm --net wiremock -v ${PWD}:/home/wiremock --name wiremock wiremock/wiremock:2.35.0 --verbose --local-response-templating
```

Use %cd% for CMD.

# View Stubs
http://localhost:8080/__admin/mappings

# View Requests
http://localhost:8080/__admin/requests
