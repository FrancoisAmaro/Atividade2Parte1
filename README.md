##### IFPB - Instituto Federal da Paraíba #####
##### Curso: Tecnologia em Sistemas para Internet #####
##### Disciplina: Linguagens de Script #####
##### Professor: Rhavy Maia Guedes #####
##### Aluno: François de Araújo Amaro - 202413810031 #####
##### Data: 07/11/2025 #####

<br>
<br>
  

# Questões práticas sobre JSON #
![](https://github.com/FrancoisAmaro/Atividade2Parte1/blob/main/GIF_JSON.gif?raw=true)
<br>

## 1. Explique o que é JSON e por que ele se tornou tão popular para troca de dados entre aplicações. ##

JSON é a sigla de JavaScript Object Notation que traduzida significa Notação de Objeto JavaScript, sendo um formato de representação de dados que é muito utilizado para API e também arquivos de configuração, dentre suas características:  utiliza o formato de chave e valor, é leve para ser enviado por requisições, sendo uma forma de escrever objetos JavaScript que pode ser interpretada por outras linguagens de programação sendo baseada em texto.
JSON se tornou tão popular para troca de dados entre aplicações porque tem um formato leve, simples, legível e independente de linguagem, que facilita a troca de dados entre sistemas. Ele é mais rápido de processar e consome menos largura de banda que alternativas como o XML, tornando-o ideal para a comunicação em tempo real em aplicações web. 

### Exemplo de JSON
```json
{
  "Nome Completo": "Geraldo Ferreira da Silva",
  "Data de Nascimento": "01/01/1970",
  "Local de Nascimento": "Rio de Janeiro - RJ",
  "Doenças Detectadas": ["Hipertensão", "Diabetes", "Hepatite"],
  "Possui Plano de Saúde": true
}
```

## 2. Qual a diferença fundamental entre JSON.stringify() e JSON.parse()? Dê um exemplo prático de quando usar cada um. ##

Quando o JSON é transferido para API, é transferido como texto, e o método JSON.stringify() garante que seja um texto com JSON válido. Já o JSON.parse() é o método que converte JSON em um objeto válido.
Exemplo: Vários aplicativos contêm informações valiosas, O instagram por exemplo, possui vários usuários e um banco de dados, e para manter a segurança dessas informações do banco de dados ele utiliza um API (Application Programming Interface) com vários regras de acesso, quem pode pedir tal informação, qual informação será fornecida, login, token de autenticação, entre outras. Tudo isso para manter o banco de dados seguro, pois se alguém tivesse como acessar diretamente, o tal aplicativo ficaria muito vulnerável. Essa requisição geralmente é feita através de JSON.

## 3. Considerando a string "JavaScript é baseada em ECMA Script", quais métodos você usaria para: ##
- Verificar se contém a palavra "Script";
- Remover a palavra "JavaScript" e gerar uma nova string;
- Substituir "baseada" por "tem origem"

Considerando a string str = "JavaScript é baseada em ECMA Script", você usaria os seguintes métodos:

(Verificar se contém a palavra "Script")

O método mais direto (introduzido no ES6) é o includes().
- Método: includes()
- Exemplo: str.includes("Script");
- Resultado: true
      Alternativa: Você também poderia usar indexOf(). Se o resultado for diferente de -1, a string contém a palavra. Exemplo: str.indexOf("Script") !== -1;

(Remover a palavra "JavaScript" e gerar uma nova string)

Pode-se usar o método replace() para encontrar a palavra e substituí-la por uma string vazia ("").

- Método: replace()
- Exemplo: str.replace("JavaScript ", "");
- Resultado: "é baseada em ECMA Script"
    Observação: O replace() não modifica a string original, mas sim gera uma nova string com a substituição.

(Substituir "baseada" por "tem origem")

- Método: replace()
- Exemplo: str.replace("baseada", "tem origem");
- Resultado: "JavaScript é tem origem em ECMA Script"

## 4. Qual a vantagem de usar template strings (``) em vez de concatenação com + para criar strings complexas? ##

Deixa o código mais organizado, fácil de visualizar e de manipular, destacando algumas características abaixo, como:
- Legibilidade: Permitindo a inclusão de expressões e variáveis diretamente dentro da string, usando a ${expressão} (placeholders). Isso torna a construção de strings complexas muito mais clara e concisa.
    Template String: `Olá ${nome}. Sua idade é ${idade + 1}.`
    Concatenação: "Olá, " + nome + ". Sua idade é " + (idade + 1) + "."
- Suporte Multilinha: Pode-se criar strings em várias linhas, sem a dependência de utilizar caracteres de escape como concatenção repetida e \n.
- Expressões Inline: É possível executar qualquer código ** JavaScript ** válido dentro do placeholder ${} (incluindo operações matemáticas, chamadas de função, etc.), oferecendo maior flexibilidade para strings dinâmicas.
  
