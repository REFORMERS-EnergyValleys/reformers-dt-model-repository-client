# OpenAPI Generator for Model Repository Client

Use [OpenAPI Generator](https://openapi-generator.tech/) for creating the client for the REFORMERS Model Repository, based on the dedicated [OpenAPI specification](https://github.com/REFORMERS-EnergyValleys/reformers-dt-model-api-specs).

## Installation

```
docker pull openapitools/openapi-generator-cli
```

## Generate client

Linux:
```
docker run --rm -v ${PWD}:/spec openapitools/openapi-generator-cli generate -g python --package-name reformers_model_repo_client -i /spec/openapi/bundled.yaml -o /spec

```

Windows:
```
docker run --rm -v %cd%:/spec openapitools/openapi-generator-cli generate -g python --package-name reformers_model_repo_client -i /spec/openapi/bundled.yaml -o /spec
```
