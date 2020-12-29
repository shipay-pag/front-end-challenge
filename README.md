# Shipay Front-end Challenge

***Nota: Utilizaremos os seguintes critérios para a avaliação: Desempenho, Testes, Manutenabilidade, Separação de responsabilidades e boas práticas de engenharia de software.***

1. Foi levantado uma tarefa pelo time de produto para a criação de um painel de de monitoramento integrações pró-ativo, e por alguns motivos o time de arquitetura e segurança da informação sugeriram que esse novo portal fosse desenvolvido em AngularJS porém “Server Side-Rendering”, e coube a você desenhar a estrutura inicial do projeto. O frontend “Server Side-Rendering” deverá fazer chamadas para um serviço no endpoint `shipay-intergration-synthetic-health.sre.svc.cluster.local:8080/all`. Com essas informações em mão, desenvolva um portal “Server Side-Rendering” que atenda aos requisitos descritos acima versionando o codigo no git. 

Para auxiliar nesse desafio, desponibilizamos o seguinte endpoint:

```
# request:
GET https://5da3e170-21ce-4dd0-ae72-ad757f7864a6.mock.pstmn.io/health

# response:
{
    "message": "all services are up and running",
    "status":"200"
}
```




Você foi convidado a participar de um time/squad que será responsável pelo novo sistema de back-office web da empresa, e por alguns motivos o time de arquitetura e segurança da informação sugeriram que esse novo portal fosse desenvolvido em AngularJS porém “Server Side-Rendering”, e coube a você desenhar a estrutura inicial do projeto. 
Descreva como você organizaria esse projeto, lembrando que o Front-End será apenas a interface dos usuários com as API’s que farão o CRUD com o banco de dados no back-end. Descreva como seria a estrutura e organização do código, componentes e frameworks que você pretende utilizar.

2. Descreva como você implementaria uma solução de busca para um e-commerce com um catálogo de aproximadamente quinhentos mil produtos, descreva os itens necessários para termos uma listagens dos produtos com imagens filtradas por categoria, a barra de busca deverá permitir buscas de itens por nome, categoria, funcionalidade e marca. 
O resultado exibirá uma página de detalhe do item (quando o match for assertivo o suficiente) ou uma lista de possíveis itens para quando o match for aproximado. Descreva os componentes, frameworks, e  implementações necessárias no front-end para permitir o funcionamento da busca, a renderização de thumbnails na pagina de listagem, renderização imagens de alta resolução na página de detalhes bem como suas sugestões de infraestrutura para otimizar o funcionamento da necessidade.

3. Descreva como você codificaria os testes referentes as suas entregas da sprint na reunião de review. Quais componentes e frameworks que você utilizaria. E na sua visão quais seriam os testes mínimos que o desenvolvedor deveria escrever?

4. Você foi selecionado para ser o mentor dos desenvolvedores juniors durante a próxima sprint. Ao final da primeira daily meeting um dos desenvolvedores questionou quais seriam os motivos para utilizarmos os seguintes componentes na nossa aplicação: Responsive Front-end framework e o CSS Preprocessor. Como você justificaria a necessidade e utilização dos referidos componentes?


BOA SORTE!
