# teste-criptografia

# Criptografia Assimétrica com JavaScript

Este projeto usa a biblioteca `node-forge` para realizar operações de criptografia assimétrica com RSA. Ele é dividido em duas páginas:

1. **Página de Criptografia**: Gera um par de chaves (pública e privada) e permite ao usuário criptografar uma mensagem.
2. **Página de Descriptografia**: Permite ao usuário colar a mensagem criptografada e a chave privada para recuperar a mensagem original.

## Como Funciona

1. A **chave pública** é usada para criptografar a mensagem.
2. A **chave privada** é necessária para descriptografar a mensagem e deve ser mantida em segurança.
3. A criptografia assimétrica é ideal para troca de mensagens seguras, pois apenas o detentor da chave privada pode descriptografar o conteúdo.

## Como Executar

Abra `index.html` no navegador para criptografar uma mensagem e copie a chave privada e a mensagem criptografada.
Em seguida, abra `decrypt.html` e cole ambos para recuperar a mensagem original.

## Dependências

A biblioteca `node-forge` é usada para gerar chaves e realizar operações de criptografia/descriptografia. Ela é carregada através de CDN para simplificar o projeto.

## Exemplo

Abaixo, um exemplo de uso:
1. Digite uma mensagem em `index.html`, clique em "Criptografar".
2. Copie a mensagem criptografada e a chave privada.
3. Abra `decrypt.html`, cole a mensagem criptografada e a chave privada, e clique em "Descriptografar" para ver a mensagem original.
