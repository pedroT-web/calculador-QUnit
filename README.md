# Utilizando a ferramenta de teste "QUnit"

#### Exportando a função como um modulo para poder ser acessada no outro arquivo
- Esta linha de código deve ser escrita no arquivo onde se encontra a sua função
```js
module.exports = suaFunção;
```

#### Chamando a função no arquivo de test
- Esta linha de código deve ser escrita no arquivo de teste
```js
const suaFunção = require("caminho/arquivo-função");
```

#### Coletando o módulo que exportamos no arquivo da função
```js
QUnit.module("suaFunção");
```

#### Função para executar o teste e retornar se deu certo ou não
```js
QUnit.test("Mensagem que vai exibir", (variavelDeResultado) => {
    variavelDeResultado.equal(suaFunção(valor1, valor2), resultadoEsperar)
})
```

## Executar o teste pelo prompt de comando

```js
npm test
```

## 