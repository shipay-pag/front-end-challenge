# Shipay Front-end Challenge

***Nota: Utilizaremos os seguintes critérios para a avaliação: Desempenho, Testes, Manutenabilidade, Separação de responsabilidades e boas práticas de engenharia de software.***

1. Foi levantado uma tarefa pelo time de produto para a criação de um painel de monitoramento pró-ativo de integrações, e por alguns motivos o time de arquitetura e segurança da informação sugeriram que esse novo portal fosse desenvolvido em AngularJS porém “Server Side-Rendering”, e coube a você desenhar a estrutura inicial do projeto. O frontend “Server Side-Rendering” deverá fazer chamadas para um serviço no endpoint `shipay-intergration-synthetic-health.sre.svc.cluster.local:8080/health`. Com essas informações em mão, desenvolva um portal “Server Side-Rendering” que atenda aos requisitos descritos acima versionando o codigo no git. 

Para auxiliar nesse desafio, desponibilizamos o seguinte endpoint.

```
# request:
GET https://5da3e170-21ce-4dd0-ae72-ad757f7864a6.mock.pstmn.io/health

# response:
{
    "message": "all services are up and running",
    "status":"200"
}
```
DICA1: utilize o endpoint de teste acima, mas mantenha o codigo parametrizável, seja via variável de ambiente, ou arquivo de configuração.

2.a. O seu time está a desenvolver um e-commerce com um catálogo de aproximadamente quinhentos mil produtos. Você foi designado para desenvolver o painel de pedidos. Utilizando o contrato abaixo, desenvolva um painel de listagem de pedidos, com a possibilidade de busca por `status`, `valor`, `data de atualização` e `carteira de pagamento`. 

```
# request:
GET https://5da3e170-21ce-4dd0-ae72-ad757f7864a6.mock.pstmn.io/pedidos

# response:
{
    "orders": [
        {
            "id": "6be41d4e-5248-43f7-99f9-fbedd78d0db9",
            "status": "cancelled",
            "total_order": 0.51,
            "update_datetime": "29-12-2020 17:19:15",
            "wallet_payment_name": "shipay-ewallet-mock"
        },
        {
            "id": "85ae0937-1d20-4662-8edb-37f287badfc7",
            "status": "cancelled",
            "total_order": 0.52,
            "update_datetime": "29-12-2020 12:43:52",
            "wallet_payment_name": "shipay-ewallet-mock2"
        },
        ...
    ]
}

# request:
GET https://5da3e170-21ce-4dd0-ae72-ad757f7864a6.mock.pstmn.io/pedido/12321321321

{
    "id": "12321321321",
    "status": "cancelled",
    "total_order": 0.51,
    "update_datetime": "29-12-2020 17:19:15",
    "wallet_payment_id": null,
    "product_id": "123456",
    "product_name": "bala de canela",
    "product_description": "bala deliciosa de canela",
    "product_image": "https://www.google.com/logos/doodles/2020/december-holidays-days-2-30-6753651837108830.5-s.png"
}

```

2.b Descreva como você codificaria os testes referentes as suas entregas da sprint na reunião de review. Quais componentes e frameworks que você utilizaria. E na sua visão quais seriam os testes mínimos que o desenvolvedor deveria escrever?  

3. Você foi selecionado para ser o mentor dos desenvolvedores juniors durante a próxima sprint. Ao final da primeira daily meeting um dos desenvolvedores questionou quais seriam os motivos para utilizarmos os seguintes componentes na nossa aplicação: Responsive Front-end framework e o CSS Preprocessor. Como você justificaria a necessidade e utilização dos referidos componentes?


BOA SORTE!
