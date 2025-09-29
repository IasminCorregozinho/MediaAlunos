
-----

# 🤖 Calculadora Simples de Média e Situação

Este é um projeto simples em **JavaScript (Node.js)** que calcula a média de cinco notas inseridas pelo usuário e determina se o aluno foi Aprovado (média $\ge 7$) ou Reprovado (média $< 7$).

## 🚀 Funcionalidades

  - **Entrada de Dados:** Solicita ao usuário cinco notas individualmente.
  - **Tratamento de Vírgula:** Converte a vírgula (`,`) para ponto (`.`) para garantir o cálculo correto de números decimais.
  - **Cálculo da Média:** Calcula a média aritmética das cinco notas.
  - **Arredondamento:** Exibe a média final arredondada para duas casas decimais.
  - **Situação do Aluno:** Determina a situação com base na regra de aprovação (Média $\ge 7$).

## 🛠️ Tecnologias Utilizadas

  - **JavaScript:** Linguagem principal.
  - **Node.js:** Ambiente de execução.
  - **`readline-sync`:** Módulo para receber entrada síncrona do usuário no console.

## ⚙️ Como Executar o Projeto

Para rodar este código, você precisa ter o **Node.js** instalado em sua máquina e o pacote `readline-sync` instalado localmente.

### Pré-requisitos

1.  Instale o [Node.js](https://nodejs.org/en/download/).
2.  Clone este repositório para sua máquina local.

### 1\. Instalação do Módulo

Abra o terminal na pasta do projeto e instale o pacote `readline-sync`:

```bash
npm install readline-sync
```

### 2\. Execução

Execute o script `media.js` usando o Node.js:

```bash
node media.js
```

O programa irá então solicitar a inserção de cinco notas no console.

## 📝 Código Fonte (`media.js`)

O código para cálculo e lógica está contido no arquivo principal:

```javascript
const readline = require('readline-sync');

console.log("-- Digite suas notas abaixo: -- ")

let nota1 = parseFloat(readline.question("Primeira nota: ").replace(',', '.'));
let nota2 = parseFloat(readline.question("Segunda nota: ").replace(',', '.'));
let nota3 = parseFloat(readline.question("Terceira nota: ").replace(',', '.'));
let nota4 = parseFloat(readline.question("Quarta nota: ").replace(',', '.'));
let nota5 = parseFloat(readline.question("Quinta nota: ").replace(',', '.'));

const media = nota1+nota2+nota3+nota4+nota5
const mediaFinal = media/5
console.log(`Sua média é: ${mediaFinal.toFixed(2)}`)

if (mediaFinal >= 7) {
    console.log("Parabéns, você foi aprovado!")
}
else {
    console.log("Você foi reprovado!")
}
```

-----

## 👨‍💻 Autor

  - **Lucas Corregeino** (Seu Nome/Usuário) - [Link para seu GitHub]

## 📜 Licença

Este projeto está licenciado sob a Licença MIT - veja o arquivo `LICENSE.md` para mais detalhes.
