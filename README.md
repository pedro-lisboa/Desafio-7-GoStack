# Desafio-7-GoStack - Banco de dados e upload de arquivos no Node.js
![GoStack Bootcamp](https://camo.githubusercontent.com/d25397e9df01fe7882dcc1cbc96bdf052ffd7d0c/68747470733a2f2f73746f726167652e676f6f676c65617069732e636f6d2f676f6c64656e2d77696e642f626f6f7463616d702d676f737461636b2f6865616465722d6465736166696f732e706e67)

## Sobre o desafio 🚀

Nesse desafio, foi desenvolvido a aplicação de gestão de transações, a GoFinances. Praticando o que aprendi até agora no React.js junto com TypeScript, utilizando rotas e envio de arquivos por formulário.

Essa é uma aplicação que irá se conectar ao seu backend do Desafio 06, e exibir as transações criadas e permitir a importação de um arquivo CSV para gerar novos registros no banco de dados.

## Funcionalidades da aplicação

- **Listar as transações da sua API:** Sua página Dashboard deve ser capaz de exibir uma listagem através de uma tabela, com o campo title, value, type e category de todas as transações que estão cadastradas na sua API.

**Dica:** Você pode utilizar a função Intl para formatar os valores. Dentro da pasta utils no template você encontrará um código para te ajudar.

- **Exibir o balance da sua API:** Sua página Dashboard, você deve exibir o balance que é retornado do seu backend, contendo o total geral, junto ao total de entradas e saídas.

- **Importar arquivos CSV:** Na sua página Import, você deve permitir o envio de um arquivo no formato csv para o seu backend, que irá fazer a importação das transações para o seu banco de dados. O arquivo csv deve seguir o seguinte modelo.

**Dica:** Deixamos disponível um componente chamado Upload na pasta components para você ter já preparado uma opção de drag-n-drop para o upload de arquivos. PS: Caso você esteja no windows e esteja sofrendo com algum erro ao tentar importar CSV, altere o tipo de arquivo dentro do arquivo components/upload/index.ts de text/csv para .csv, application/vnd.ms-excel, text/csv.

**Dica 2:** Utilize o FormData() para conseguir enviar o seu arquivo para o seu backend.

### Rotas da aplicação

As informações da categoria, devem ser retornadas junto com a transação do seu backend no formato como o seguinte:
```
{
  "id": "c0512e43-6589-4dc8-bd0c-2a3f71b347aa",
  "title": "Loan",
  "type": "income",
  "value": "1500.00",
  "category_id": "d93eccc7-64bb-4268-b825-9200103f3a8b",
  "created_at": "2020-04-20T00:00:49.620Z",
  "updated_at": "2020-04-20T00:00:49.620Z",
  "category": {
    "id": "d93eccc7-64bb-4268-b825-9200103f3a8b",
    "title": "Others",
    "created_at": "2020-04-20T00:00:49.594Z",
    "updated_at": "2020-04-20T00:00:49.594Z"
  }
}
```


## Instalação

Utilize os comandos para instalar as dependencias:

```sh
npm install 
or
yarn
or
yarn instal
```

## Configuração para Desenvolvimento

Para executar a aplicação:

```
yarn start
```

Para executar os testes:

```
yarn test
```

## Meta

Pedro Lisboa – [@Pedro-lbrt](https://www.linkedin.com/in/pedro-lbrt/...) – pegu_lisboa@hotmail.com

[https://github.com/pedro-lisboa/GoBarber-backend](https://github.com/pedro-lisboa/)
