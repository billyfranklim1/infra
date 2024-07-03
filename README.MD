# Infra

Este projeto configura um contêiner MySQL utilizando Docker. Siga as instruções abaixo para baixar e rodar o projeto.

## Pré-requisitos

- [Docker](https://www.docker.com/get-started) instalado na máquina.

## Configuração

1. Clone o repositório para a sua máquina local:

```bash
git clone https://github.com/billyfranklim1/infra.git
```

2. Navegue até o diretório do projeto:

```bash
cd infra
```

3. Renomeie o arquivo `.env.example` para `.env` e configure as variáveis de ambiente conforme necessário. Por padrão, o conteúdo do arquivo é:

```env
MYSQL_ROOT_PASSWORD=password
MYSQL_VOLUME_PATH=/Users/billy/Documents/codes/infra-local/db/mysql
```

Certifique-se de ajustar o `MYSQL_VOLUME_PATH` para um caminho válido no seu sistema.

## Executar o projeto

Para iniciar o contêiner MySQL, execute o comando abaixo:

```bash
docker-compose up -d
```

Isso iniciará o contêiner em segundo plano. O banco de dados MySQL estará disponível na porta `3306`.

## Parar o projeto

Para parar o contêiner MySQL, execute o comando abaixo:

```bash
docker-compose down
```

Isso encerrará e removerá o contêiner.

## Links úteis

- [Repositório do projeto](https://github.com/billyfranklim1/infra)
