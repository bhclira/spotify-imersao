# Conversor de Moedas


<p>Tela de preview do App</p>

![Preview](images/preview.png)

Este repositório contém um projeto de um conversor de moedas simples que permite converter valores em Real (R$) para Dólar (USD), Euro (EUR) e Bitcoin (BTC). A aplicação é responsiva e se adapta a diferentes tamanhos de tela, incluindo celulares, tablets e computadores.

## Funcionalidades / Functionalities

- Conversão de valores em Real (R$) para Dólar (USD), Euro (EUR) e Bitcoin (BTC).
- Limpeza dos campos de entrada e do valor convertido.
- Interface responsiva que se adapta a diferentes tamanhos de tela.

## Tecnologias Utilizadas / Tools

- HTML
- CSS
- JavaScript

## Estrutura do Projeto

### index.html

O arquivo `index.html` contém a estrutura básica da página, incluindo os elementos de entrada, botões e áreas de exibição dos resultados.

Exibe um container com:
* título, subtítulo e um campo input do tipo número.
*  No campo destinado ao usuário digitar o valor a ser convertido, eu usei um título e um atributo "placeholder" que se mostra para o usuário como uma legenda de exemplo dentro dele;
*  Em cada botão "button" (um para cada moeda) usei o atributo "onclick" que invoca as funções respectivas de converter os valores digitados para as moedas de cada botão;
*  Adidionei um botão extra  que contém uma função para resetar os campos de valor para os seus valores iniciais para caso o usuário quiser usar o programa mais de uma vez.
  

### script.js

O arquivo script.js contém as funções JavaScript para realizar as conversões de moeda e limpar os campos de entrada:

* para cada função eu atribui um objeto document DOM a uma variável que foi responsável por pegar o valor ".value" do input fornecido pelo usuário na formulário HTML
* De posse desse valor, cada função de moeda multiplica pela sua cotação estipulada para calcular o valor resultante;
* Esse valor então é devolvido para o HTML no campo "valorConvertido" através da propriedade de objeto document.innerText;

### style.css

O arquivo style.css contém os estilos para a página, incluindo a configuração de uma imagem de fundo, estilos para os elementos de entrada e botões, e media queries para tornar a aplicação responsiva:

* Alinhei o conteiner vertical e horizontalmente
* removi a margem padrão com margin:0;
* Usei um background color com transparência no container para contrastar com a imagem de fundo;
* Apliquei sombras e raios de borda;
* Estilizei os botões e acrescentei margens e paddings, aprendi a estilizar as bordas;
* Pedi ao Co-Pilot para fazer os media-queries do projeto e implementei depois de testes usando a inspeção do navegador.

## Como contribuir / How Contribute

```bash
# Clone the project
$ git clone https://github.com/bhclira/conversor_moedas
```
