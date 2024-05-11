# **Desafio Dio - Criando um Sistema de Rastreamento de Preços de Criptomoedas**



Este projeto tem como objetivo criar um sistema abrangente e fácil de usar para rastrear os preços das criptomoedas. O sistema permitirá aos usuários monitorar os preços de suas criptomoedas favoritas, definir alertas de preço e receber notificações quando os preços atingirem certos níveis.



## **Descrição**

O sistema de rastreamento de preços de criptomoedas será uma aplicação web hospedada em um servidor. O sistema será acessível por meio de um navegador da web e incluirá uma interface de usuário intuitiva. O sistema permitirá aos usuários monitorar os preços de suas criptomoedas favoritas, definir alertas de preço e receber notificações quando os preços atingirem certos níveis.

A requisição de dados de uma API de criptomoedas é uma tarefa relativamente simples, mas é fundamental que você entenda como fazer isso corretamente para evitar erros e obter os dados que você precisa.

Para requisitar dados de uma API de criptomoedas, você precisará de algumas informações:

- O nome da API que você deseja usar.
- A chave de API da API.
- A URL da API.

Uma vez que você tiver essas informações, você pode seguir os seguintes passos para fazer uma requisição:

1. Criar uma nova sessão HTTP.
2. Definir a URL da API na sessão HTTP.
3. Definir a chave de API na sessão HTTP.
4. Definir o tipo de método de requisição (GET, POST, PUT, DELETE).
5. Definir os parâmetros da requisição.
6. Enviar a requisição.

Abaixo, você encontrará um exemplo de código que mostra como fazer uma requisição à API de dados de criptomoedas da CoinMarketCap:

```plaintext
import requests

api_url = "https://pro.coinmarketcap.com/api/v1/ticker/"

headers = {"Authorization": "Bearer YOUR_API_KEY"}

params = {"limit": 10}

response = requests.get(api_url, headers=headers, params=params)

data = response.json()

print(data)
```

Esta requisição irá retornar os dados de 10 das principais criptomoedas, incluindo o nome, o símbolo, o preço, o volume de negociação e a capitalização de mercado.

Você pode encontrar mais informações sobre como requisitar dados de uma API de criptomoedas na documentação da API.



## **Estruturando o Projeto**

O projeto será estruturado em vários módulos, cada um responsável por uma tarefa específica. Os módulos serão organizados de forma lógica e reutilizável.

## Estrutura do Projeto

```
criptomoedas/
│
├── models/
│   ├── __init__.py
│   └── criptomoeda.py
│
├── services/
│   ├── __init__.py
│   └── coingecko.py
│
├── tests/
│   ├── __init__.py
│   └── test_coingecko.py
│
├── main.py
└── README.md
```

### **Documentando**

O projeto será extensivamente documentado usando docstrings e comentários. A documentação incluirá exemplos de código e explicações claras de como usar cada função.

### **Definindo Modelos**

O projeto usará um modelo orientado a objetos para representar criptomoedas, usuários e outras entidades. Os modelos fornecerão uma interface consistente para trabalhar com esses dados.

### **Definindo Serviços**

O projeto definirá uma série de serviços que executarão tarefas comuns de rastreamento de preços de criptomoedas. Os serviços serão projetados para serem eficientes e fáceis de usar.

- `models/criptomoeda.py`: Este arquivo define a classe `Criptomoeda`, que representa uma criptomoeda. Cada instância desta classe tem atributos como `nome`, `preco`, `volume`, etc.
- `services/coingecko.py`: Este arquivo define a classe `CoinGeckoAPI`, que é responsável por fazer requisições para a API CoinGecko. Esta classe tem métodos como `get_price()`, `get_volume()`, etc.
- `main.py`: Este é o ponto de entrada do nosso programa. Ele cria uma instância da classe `CoinGeckoAPI`, faz requisições para a API e imprime os resultados.

## **Definindo Regras de Negócio**

O projeto definirá um conjunto de regras de negócios que governarão como o sistema rastreia os preços das criptomoedas. As regras de negócio serão documentadas e testadas para garantir sua precisão.

## **Integrando**

O projeto será integrado com várias APIs de criptomoedas para obter dados de preços em tempo real. O sistema também será integrado com um serviço de notificação para enviar alertas de preço aos usuários.

## **Testando**

O projeto será extensivamente testado para garantir sua funcionalidade e precisão. Os testes serão automatizados para garantir a consistência.

- `tests/test_coingecko.py`: Este arquivo contém testes unitários para a classe `CoinGeckoAPI`. Usamos uma biblioteca de testes como `pytest` para escrever e executar os testes.



# API Coin Market Cap

Requisitando dados de uma API de criptomoedas com **JavaScript**. Esse projeto foi uma ampliação da aula ministrada por **Bárbara Casac** na **Digital Innovation One**.

![Alt text](https://github.com/lucasdealmeidadev/API-de-criptomoedas/blob/main/coins.png?raw=true "API Coin Market Cap")

### Melhorias implementadas:

- Interface do projeto totalmente remodelada utilizando Bootstrap v5.0;
- Adiconado a primeira e última data histórica;
- Inclusão do ranking de criptomoedas.

### Requisitos e Documentações

[Gerar a API KEY no Portal do desenvolvedor](https://pro.coinmarketcap.com/account) <br>
[Documetação de autenticação](https://coinmarketcap.com/api/documentation/v1/#section/Authentication)<br>
[Documentação da API](https://coinmarketcap.com/api/documentation/v1/#)<br>
[Instalar e Habilitar a extensão para o Google Chrome](https://chrome.google.com/webstore/detail/moesif-origin-cors-change/digfbfaphojjndkpccljibejjbppifbc)

## Licença

* Licenciado sob a licença MIT - veja [LICENSE](https://github.com/lucasdealmeidadev/API-de-criptomoedas/blob/main/LICENSE) para mais informações.

----------



## **Aprendizado**

Este projeto proporcionará uma oportunidade de aprender sobre os seguintes tópicos:

- Rastreamento de preços de criptomoedas
- Desenvolvimento de software
- Documentação de software
- Teste de software

## **Aplicabilidade Prática**

Este projeto pode ser usado em uma variedade de aplicações práticas, tais como:

- Rastreamento de preços de criptomoedas pessoais
- Rastreamento de preços de criptomoedas para fins de negociação
- Fornecendo dados de preços de criptomoedas para outras aplicações



## **Conclusão**

Este projeto resultará em um sistema de rastreamento de preços de criptomoedas abrangente, fácil de usar e eficiente. O sistema será valioso para investidores e traders de criptomoedas que precisam monitorar os preços de suas criptomoedas favoritas.