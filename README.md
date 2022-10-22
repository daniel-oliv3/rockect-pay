<h1 align="center"> RocketPay </h1>



### Pré-Requisitos.

HTML, CSS, JavaScript, DOM, Node.

### Ferramentas do programador.

**Visual Studio Code**
- Instalar e configurar
- Site: https://code.visualstudio.com/download
- Extenções
    - `Material Icons Theme`
    - `Omni Theme`
    - `Prettier - Code Formatter` 

**Git Bash**
- Windows
- Instalar e configurar
- Site: https://git-scm.com/downloads


**Git Hub**
- Verificar versão do git
- Configurar o Git

```
git --version
```
```
git config --global user.name "Daniel Oliveira"
```
```
git config --global user.email "xxxxxxxx@gmail.com"
```
- Clonar o repositorio inicial boilerplate
```
gh repo clone rocketseat-education/explorer-lab-01
```

**Git Cli**
- Instalar e configurar
- Site: https://cli.github.com/


**Node.Js**
- Instalar e configurar LTS
- Site: https://nodejs.org/en/


**Vite**
- Instalar e configurar
- Site: https://vitejs.dev/

```
npm create vite@latest
```
- NPM `node_modules` `package.lock.json`
```
npm install 
```
- Rodar o projeto
```
npm run dev
```

### Figma
- Projeto: https://www.figma.com/file/bTxGv6aemqQ0yKzTI5P2k7/Explorer-Lab-%2301-(Copy)?node-id=0%3A1

### O que é DOM
**Document Object Model**
- Modelagem do documento como objeto javascript

**Representação do HTML em objetos javascript**
- Atributos (Propriedades) e métodos (Funcionalidades)

**Criado pelo navegador (Browser)**
- É uma interface (API) usada no navegador

**DevTools**
- Através das ferramentas do desenvolvedor `Dev Tools`, observaremos a DOM.
```js
//Objeto global presente em qualquer página no navegador
window

//Representação do documento
document
```

**Primeiros passos na DOM**
- Pegar elementos HTML
- Substituição de atributo
- Disponibilizando funções globais


##

**Imask.js**
- Site: https://imask.js.org/guide.html
- http://vanilla-js.com/


- Instalar
```
npm install imask
```
- import
```
import IMask from 'imask';
```
- Simple use case:
```js
//Exemplo documentação
var element = document.getElementById('selector');
var maskOptions = {
  mask: '+{7}(000)000-00-00'
};
var mask = IMask(element, maskOptions);
```

- Para máscaras aninhadas complexas, há uma opção de blocos disponível:

```js
//Exemplo de Blocks
var blocksMask = IMask(element, {
  mask: 'Ple\\ase fill ye\\ar 19YY, month MM \\and v\\alue VL',
  lazy: false,  // make placeholder always visible

  blocks: {
    YY: {
      mask: '00',
    },

    MM: {
      mask: IMask.MaskedRange,
      from: 1,
      to: 12
    },

    VL: {
      mask: IMask.MaskedEnum,
      enum: ['TV', 'HD', 'VR']
    }
  }
});
```

- Pegar o '22' de 2022
```js
String(new Date().getFullYear()).slice(2);
```
**Expressões regulares**
- Regex com JavaScript

Expressões regulares

Também conhecida como `Regular Expression` ou ` Regex` é uma tecnologia usada para buscar padrões dentro de textos e funciona em diversas linguagens

- Exemplo: Busque por todos os caracteres numéricos dentro de algum texto

Como pensar ?

Existe uma maneira correta de pensar ao utilizar essa tecnologia para buscar de padrões
- Leitura da esquerda para direita
- Ler um caractere de cada vez, um após o outro
- Conhecer os caracteres reservados da tecnologia

- Criando regex no JavaScript
```js
//Exemplo

const re = /foo/;

const re = new RegExp(/foo/);
```

- Funções usadas em Strings

Existem diversas maneiras de usar expressões regulares em uma string no javaScript. Abaixo, vamos verificar 3

```js
//Agrupa os padrões em um array
const matches = 'aBC'.match(/[A-Z]/g);
//Output: Array [B, C]

//Pesquisa se existe ou não o padrão
const index = 'aBC'.search(/[A-Z]/);
//Output: 1

//Substitui os padrões por novo valor
const next = 'aBC'.replace(/a/, 'A');
//Output: ABC

```

**Cheatsheet**

Básico
- `/ expression / flags`
  Exemplo: `/[A-Z]+/g`
- `\` Usar caracteres especiais
  Exmplo: `/ Oi\?\*\\/`
- `()` Agrupador
- `|` OU lógico
- `Fala Dev` pesquisa extra
- `^Fala` Start of the string
- `Dev$` End of the string

Colchetes
- `[XYZ]` Qualquer um, x, y, z
- `[J-Z]` Qualquer caracter entre J e Z
- `[^xyz]` Nenhum X, Y, Z

Classes de caracteres
- `\w` Palavra `\d` dígito `\s` espaços em branco(tabs, quebras de linha)
- `\w` NÃO palavra `\D` NÃO dígito `\S` NÃO espaços em branco
- `\t` tabs, `\n` quebra de linha
- `.` Qualquer caracter (exceto nova linha)
- `?` Zero ou uma ocorrências
- `*` Zero ou múltiplas ocorrências
- `{n}` n ocorrências
- `{min, max}` Mínima / Máxima ocorrências

Testando Expressões

Podemos testar de diversas formas, desde diretamente no código, ou:

- Direto no Editor (VSCODE)
  Search and Replace
- Online
  RegExr: Learn, Build, & Test RegEx


Referências

- https://www.youtube.com/watch?v=sa-TUpSx1JA
- https://www.fireship.io/lessons/regex-cheat-sheet-js/
- https://www.debuggex.com/cheatsheet/regex/javascript



```txt
Expressões regulares.

Visa: ^4\d{0, 15}
Inicia com 4 seguido de mais 15 dígitos

Mastercard:
Inicia com 5, seguido de um dígito entre 1 e 5, seguido de mais 2 dígitos
Ou

Inicia com 22, seguido de um dígito entre 2 e 9, seguido de mais 1 dígitos
Ou

Inicia com 2, seguido de um dígito entre 3 e 7, seguido de mais 2 dígitos seguido de mais 12 dígitos
```











##
### 
##

- By:  **Daniel Oliveira**

  - `Instagram` - https://www.instagram.com/danieloliv3/
  - `Facebook` - https://web.facebook.com/danielsapup3/
  - `Twitter` - https://twitter.com/danielsapup3/
  - `Linkedin` - https://www.linkedin.com/in/danielsapup3/

  ##