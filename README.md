# Engenharia de Dados - Estudos
Repositório destinado a estudos.

## Dependencias
- Python
- PIP
- Docker
- Docker Compose

## Como executar
Para executar o projeto, vamos primeiramente precisar de um banco de dados PostgreSQL, para isso existe um container já configurado no projeto, que é possível executar via Docker, com o seguinte comando:

```bashrc
$ docker-compose up
```

Com o banco criado, podemos executar os scripts de criação de tabelas que se encontram no diretório `scripts/create_tables.sql`.

Já com as tabelas criadas, vamos instalar as dependencias necessárias para a execução do script em Python, com o auxilio do pip:

```bashrc
$ pip install -r requirements.txt
```

Agora com todas dependencias instalas e configuradas, podemos executar o script:

```bashrc
$ python populate.py
```

Agora é possível verificar no banco de dados que as tabelas foram criadas e possuem os conteudos que estão no diretório `Datasets` nas tabelas formatado.
