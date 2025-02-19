# HomeAssistantDockerTest1


# Como Executar

## Passo 1: Clonar o Repositório

Execute o comando abaixo para clonar o repositório do GitHub:

```
git clone https://github.com/tome-ferreira/HomeAssistantDockerTest1.git
```

Acesse o diretório do projeto:

```
cd HomeAssistantDockerTest1
```

---

## Passo 2: Executar a Aplicação com Docker

Certifique-se de que o Docker está em execução.

### Na primeira execução:

Execute o comando:
```
docker-compose build
```

Depois execute:
```
docker-compose up -d
```

A aplicação à InfluxDb disponível no endereço: http://localhost:8086.

Criar o utlizador "admin" com uma password à sua escolha, criar "Initial Organization Name": "Teste"; e "Initial Bucket Name": "homeassistant"

Copiar o token e colar-lo no local apropriado em "configuration.yaml". 

Por fim execute o comando 

```
docker-compose restart homeassistant
```
O Home Assistnat está disponível no endereço: http://localhost:8123.

### Nas seguintes execuções:

Execute o comando:

```
docker-compose up -d
```
