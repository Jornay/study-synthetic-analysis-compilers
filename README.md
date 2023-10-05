# Compilador Simples com Análise Sintática Dirigida pela Sintaxe (SDT)

Este é um exemplo de um compilador simples implementado em Python, que realiza análise sintática e semântica básica. O compilador lê um arquivo de código-fonte, realiza a análise léxica, gera uma lista de tokens e, em seguida, realiza a análise sintática para verificar a estrutura do código.

## Descrição do Código

O código fornecido consiste em duas partes principais:

1. **Analisador Léxico (AFD):** O código implementa funções AFD (Autômato Finito Determinístico) para reconhecer tokens, como números inteiros, strings, identificadores, operadores, delimitadores, tipos de variáveis e palavras-chave.

2. **Analisador Sintático (Parser):** O código implementa um analisador sintático que verifica a estrutura do código-fonte com base na gramática da linguagem. Ele constrói uma tabela de símbolos para rastrear variáveis e realiza análises semânticas simples, como verificação de duplicação de variáveis.

## Utilização

Para utilizar o compilador, siga estas etapas:

1. Crie um arquivo de código-fonte com a extensão `.x` (por exemplo, `codigo_sdt.x`) com código na linguagem suportada pelo compilador.

2. Execute o script Python fornecido, que fará a análise léxica e sintática do código.

3. O script produzirá mensagens de saída indicando os tokens reconhecidos e quaisquer erros sintáticos ou semânticos encontrados no código.

## Exemplo de Código

Aqui está um exemplo de código que pode ser processado por este compilador:

```x
init {
    int a;
    int b;
    a = 5;
    b = 3;
    int c;
    c = a + b;
}
```
