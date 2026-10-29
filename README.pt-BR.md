# OpenAPI da Raims

Especificação OpenAPI oficial da API pública da Raims.

[English](README.md) · [Documentação da API](https://docs.raims.com/br/api)

## Arquivos

A pasta `latest/` contém o contrato da API publicada:

| Arquivo | Formato |
| --- | --- |
| [openapi.spec3.json](latest/openapi.spec3.json) | OpenAPI 3.1 em JSON |
| [openapi.spec3.yaml](latest/openapi.spec3.yaml) | O mesmo contrato em YAML |
| [manifest.json](latest/manifest.json) | Versão da API, revisão publicada e hashes dos arquivos |
| [SHA256SUMS](latest/SHA256SUMS) | Checksums SHA-256 |

Baixe o [JSON](https://raw.githubusercontent.com/raimshq/openapi/main/latest/openapi.spec3.json)
ou o [YAML](https://raw.githubusercontent.com/raimshq/openapi/main/latest/openapi.spec3.yaml)
para importar a API em ferramentas compatíveis ou gerar um cliente na sua
linguagem. Os exemplos são ilustrativos. Não use uma credencial ou um link de
checkout de exemplo como valor real de uma integração.

## Fixar uma revisão

`latest` muda conforme a API publicada evolui. Para reproduzir uma geração,
escolha um commit deste repositório e substitua `COMMIT_SHA` nesta URL:

```text
https://raw.githubusercontent.com/raimshq/openapi/COMMIT_SHA/latest/openapi.spec3.json
```

O mesmo formato vale para o arquivo YAML. Consulte o manifesto ou os checksums
para conferir um arquivo baixado.

## Integração

A URL-base da API é `https://api.raims.com`. A credencial seleciona Sandbox ou
Produção. Siga o [guia de autenticação](https://docs.raims.com/br/integracoes/autenticacao)
e mantenha as credenciais no seu servidor, fora do código versionado e do navegador.

Um cliente gerado pertence à sua integração; ele não é um SDK oficial da Raims.
Consulte a documentação para autenticação, retries, resultados assíncronos e
o significado das respostas.

## Atualizações e licença

Os arquivos são gerados a partir do contrato da API publicada. Informe problemas
da especificação nas [Issues do GitHub](https://github.com/raimshq/openapi/issues),
sem credenciais ou dados de clientes. Não edite as definições dos endpoints
diretamente neste espelho.

Os arquivos deste repositório estão disponíveis sob a [licença MIT](LICENSE).
