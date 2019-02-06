# Markdown tips
O intuito deste documento é relembrar a sintaxe básica necessária para escrever documentos em extensão Markdown suportada pelo GitHub.

## Recursos contemplados
* Títulos, quebras de linha e linhas horizontais.
* Estilização do texto pleno.
* Listas.
* Mídias e hyperlinks.
* Códigos, citações e outros realces.
* Escapando caracteres Markdown.
* Tabelas.

## Existe algum lugar para revisar meu README antes de dar commit?
Pelo site [Make a Readme](https://www.makeareadme.com/) você pode renderizar em tempo real o seu documento com extensão Markdown.

### Títulos, quebras de linha e linhas horizontais.
#### Títulos
Títulos são indicados pelo caracteres ASCII de valor 35 `#` seguido por mais um espaço em branco tal qual a tag `<?php `. E sua quantidade indica o seu nível de importância de forma crescente.

Ou seja o uso de 1 `#` equivale a tag HTML `<h1>`, o uso de  3 `#` em sequência equivalem a tag HTML `<h3>` e assim por diante.

Você pode usar até 6 `#` em sequência para indicar um título.

#### Quebras de linha
A marcação que indica a quebra de linha pode se dar de duas formas, o uso de espaçamento duplo quebra a linha e preserva o parágrafo. 
Ao deixar um intervalo de uma linha em branco entre as linhas no seu editor de texto resultará em um novo parágrafo.

#### Linhas horizontais
São adicionadas com o propósito de seccionar a página separando diferentes assuntos. Para adicioná-la use 3 caracteres ASCII de valor 95 \_\_\_ precedido por uma quebra de linha.

### Estilização do texto pleno.
Utilize __2__ caracteres ASCII de valor 95 \_\_underline_\_ ao início e fim do texto para __Bold__.  
Utilize __2__ caracteres ASCII de valor 42 \*\*asterisk*\* ao início e fim do texto para **Bold**.

Utilize __1__ caractere ASCII de valor 95 \_underline\_ ao início e fim do texto para _Italic_.  
Utilize __1__ caractere ASCII de valor 42  \*asterisk\* ao início e fim do texto para *Italic*

Utilize __2__ caracteres ASCII de valor 126 \~\~tilde\~\~ ao início e fim do texto para ~~Strikethrough~~.  

Utilize __2__ caracteres ASCII de valor 42 + __1__ caractere ASCII de valor 95 \*\*\_like this\_\*\* ao início e fim do texto para **_Impressive_**.

### Listas.
__Listas ordenadas__ são facilmente criadas indicando o número no ínicio da linha seguido por um ponto e espaço. Pule linhas sem deixar espaços em branco entre os itens para dar sequência. Exemplo:
```
1. alguma coisa.  
1. próximo item.
```
Resulta em:
1. alguma coisa. 
1. próximo item.  

Para adicionar subitens basta não quebrar o parágrafo e adicionar dois espaços duplos ao fim da linha do item __pai__. Exemplo:
```
1. alguma coisa.   
1.1. e mais outra.
1. próximo item.
```
Resulta em:  
1. alguma coisa.  
1.1. e mais outra.
1. próximo item.

__Listas não ordenadas__ seguem o mesmo príncipio, atente-se em substituir os numerais pelo caractere ASCII de valor 42. Exemplo:
```
* alguma coisa.
* próximo item.
```
Resulta em:  
* alguma coisa.  
* e mais outra.

Para adicionar subitens basta não quebrar o parágrafo e adicionar dois espaços duplos ao início da linha do item __filho__. Exemplo:

```
* alguma coisa.   
  * e mais outra.
* próximo item.
```
Resulta em:  
* alguma coisa.
  - e mais outra.
* próximo item.

### Mídias e hyperlinks.
Para adicionar __vídeos__ use o seguinte trecho de código.
```
[![Alt text](https://img.youtube.com/vi/VID/0.jpg)](https://www.youtube.com/watch?v=VID)
```
Onde `VID` deve ser substituído pelo atual ID do vídeo que você deseja postar.

Resultado:

[![Cool beat tapes](https://img.youtube.com/vi/Z6ih1aKeETk/0.jpg)](https://www.youtube.com/watch?v=Z6ih1aKeETk)
___

Para adicionar __hyperlinks__ use o seguinte trecho de código.
```
[Linked text](https://www.thatwebpage.com/) 
```
___

Para adicionar __imagens__ você pode usar a marcação do HTML da seguinte forma.
```
<figure>
  <img src="/pasta/alguma-imagem.jpg" alt="Essa é minha imagem número 01.">	
  <figcaption>Imagem número 01.</figcaption>
</figure>
```
___

Para adicionar __emojis__ utilize a seguinte sintaxe: `:EMOJICODE:`.
Você pode conferir uma lista de emojis clicando [aqui](https://www.webfx.com/tools/emoji-cheat-sheet/).
___

Para adicionar __outras mídias__ como arquivos em pdf, csv, modelos 3D ou geolocalização, visite [esta página](https://github.blog/2015-03-17-pdf-viewing/).

### Códigos, citações e outros realces.
Trechos de código são

Para citações use o caractere ASCII de valor 62 > precedido por uma quebra de linha.

Outros realces

### Escapando caracteres Markdown.
Utilize o caractere ASCII de valor 92 \ antes do caractere Markdown para evitar que o símbolo seja interpretado.

### Tabelas
Exemplo:
```
Manufatura  | Material | Volume (cm³) | Massa (Kg) |
------------- | ------------- | ------------ | ------------- |
Coletor hidráulico (Projeto original - Usinagem)  | Liga de alumínio  | 9600 | 25,6  |
Projeto para 1ª iteração (Manufatura Aditiva)  | Liga de alumínio  | 4650 (-52%) | 12,3  |
Projeto para 2ª  iteração (Manufatura Aditiva) | Aço inoxidável 316L | 2040 (-79%) | 16,3 |
```

## Contribuições
Atualmente somente o [@Bodera](https://github.com/Bodera) atualiza o conteúdo deste repositório. Pull requests neste repositório são bem-vindas, mas peço antes que seja aberta uma issue para discutirmos sobre o que você gostaria de mudar.

## Licença
O conteúdo contido neste repositório ainda não está submetido sob licença alguma.
