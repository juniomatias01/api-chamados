# API de chamados de suporte

**Estudante:** José Junio de Souza Matias  
**Matrícula:** 2025014028

## Objetivo

Criar a estrutura inicial de uma API de chamados de suporte usando Python e Flask. Nesta etapa, a aplicação disponibiliza apenas a rota inicial; não há cadastro de chamados nem banco de dados.

## Instalação

Com o [uv](https://docs.astral.sh/uv/) instalado, na pasta do projeto execute:

```bash
uv sync --locked
```

## Execução

Inicie a aplicação com:

```bash
uv run flask --app app run --host=0.0.0.0 --port=5000
```

## Rota inicial

Acesse `http://localhost:5000/` com o método `GET`. A rota responde com status HTTP `200`, cabeçalho `Content-Type: application/json` e o seguinte corpo:

```json
{
  "mensagem": "API de chamados em funcionamento"
}
```

Também é possível conferir pelo terminal:

```bash
curl -i http://localhost:5000/
```

## Site no GitHub Pages

A documentação estática do projeto é publicada em <https://juniomatias01.github.io/api-chamados/> pela esteira do GitHub Actions. O Pages não hospeda o servidor Flask; para acessar a API, execute-a localmente ou em um serviço compatível com Python.