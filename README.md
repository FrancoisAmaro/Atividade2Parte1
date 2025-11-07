# Atividade2Parte1
Primeira parte da segunda atividade da disciplina Linguagens de Script - IFPB

## Questões práticas ##

## 1. Explique o que é JSON e por que ele se tornou tão popular para troca de dados entre aplicações. ##

JSON é a sigla de JavaScript Object Notation que traduzida significa Notação de Objeto JavaScript, sendo um formato de representação de dados que é muito utilizado para API e também arquivos de configuração, dentre suas características:  utiliza o formato de chave e valor, é leve para ser enviado por requisições, sendo uma forma de escrever objetos JavaScript que pode ser interpretada por outras linguagens de programação sendo baseada em texto.
JSON se tornou tão popular para troca de dados entre aplicações porque tem um formato leve, simples, legível e independente de linguagem, que facilita a troca de dados entre sistemas. Ele é mais rápido de processar e consome menos largura de banda que alternativas como o XML, tornando-o ideal para a comunicação em tempo real em aplicações web. 

## 2. Qual a diferença fundamental entre JSON.stringify() e JSON.parse()? Dê um exemplo prático de quando usar cada um. ##

Quando o JSON é transferido para API, é transferido como texto, e o método JSON.stringify() garante que seja um texto com JSON válido. Já o JSON.parse() é o método que converte JSON em um objeto válido.
Exemplo: Vários aplicativos contêm informações valiosas, O instagram por exemplo, possui vários usuários e um banco de dados, e para manter a segurança dessas informações do banco de dados ele utiliza um API (Application Programming Interface) com vários regras de acesso, quem pode pedir tal informação, qual informação será fornecida, login, token de autenticação, entre outras. Tudo isso para manter o banco de dados seguro, pois se alguém tivesse como acessar diretamente, o tal aplicativo ficaria muito vulnerável. Essa requisição geralmente é feita através de JSON.

## 3. Considerando a string "JavaScript é baseada em ECMA Script", quais métodos você usaria para: ##
- Verificar se contém a palavra "Script";
- Remover a palavra "JavaScript" e gerar uma nova string;
- Substituir "baseada" por "tem origem"


## 4. Qual a vantagem de usar template strings (``) em vez de concatenação com + para criar strings complexas? ##
