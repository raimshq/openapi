# Raims OpenAPI

Official OpenAPI specification for the Raims public API.

[Português](README.pt-BR.md) · [API documentation](https://docs.raims.com/en/api)

## Files

The `latest/` directory contains the contract for the published API:

| File | Format |
| --- | --- |
| [openapi.spec3.json](latest/openapi.spec3.json) | OpenAPI 3.1 in JSON |
| [openapi.spec3.yaml](latest/openapi.spec3.yaml) | The same contract in YAML |
| [manifest.json](latest/manifest.json) | API version, published revision and file hashes |
| [SHA256SUMS](latest/SHA256SUMS) | SHA-256 checksums |

Download the [JSON](https://raw.githubusercontent.com/raimshq/openapi/main/latest/openapi.spec3.json)
or [YAML](https://raw.githubusercontent.com/raimshq/openapi/main/latest/openapi.spec3.yaml)
to import the API into compatible tools or generate a client for your language.
Examples are illustrative. Never use an example credential or checkout link
as a real integration value.

## Pin a revision

`latest` changes as the published API evolves. For reproducible generation,
choose a commit in this repository and replace `COMMIT_SHA` in this URL:

```text
https://raw.githubusercontent.com/raimshq/openapi/COMMIT_SHA/latest/openapi.spec3.json
```

You can use the same form for the YAML file. Check the manifest or checksums
when verifying a downloaded file.

## Integration

The API base URL is `https://api.raims.com`. Your API credential selects
Sandbox or Production. Follow the [authentication guide](https://docs.raims.com/en/integracoes/autenticacao)
and keep credentials on your server, outside source control and client code.

A generated client is your integration code; it is not an official Raims SDK.
Check the API documentation for authentication, retries, asynchronous results
and the meaning of each response.

## Updates and license

These files are generated from the published API contract. Report specification
issues in [GitHub Issues](https://github.com/raimshq/openapi/issues), without
credentials or customer data. Do not edit endpoint definitions directly in this
mirror.

The files in this repository are available under the [MIT License](LICENSE).
