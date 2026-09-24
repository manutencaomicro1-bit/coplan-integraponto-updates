# Coplan IntegraPonto — Atualizações

Canal público de distribuição das atualizações oficiais do **Coplan IntegraPonto**.

Este repositório armazena somente:

- o manifesto `latest.json`, consultado pelo aplicativo;
- os instaladores publicados na área **Releases**;
- as notas de cada versão.

O código-fonte, configurações internas e credenciais corporativas não devem ser publicados aqui.

## Estrutura do manifesto

```json
{
  "version": "1.1.0",
  "installerUrl": "https://github.com/manutencaomicro1-bit/coplan-integraponto-updates/releases/download/v1.1.0/Coplan-IntegraPonto-Setup.exe",
  "sha256": "HASH_SHA256_DO_INSTALADOR",
  "releaseNotes": "Descrição das alterações.",
  "mandatory": false
}
```

O aplicativo compara `version` com sua versão instalada, baixa o instalador indicado por `installerUrl` e confere o arquivo usando `sha256` antes de executá-lo.

> A chave da API do RH nunca deve ser adicionada a este repositório.
