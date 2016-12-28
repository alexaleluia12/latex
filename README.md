## Ajudar com a escrita de conteúdo usando latex no [sharelatex](https://www.sharelatex.com)

Indico colocar os imports de pacotes todos no mesmo lugar e usar comentarios.

### lista automática de simbolos
1 - Importe o pacote (dentro de main.tex)

```tex
% ---
% ###############################
% # seus pacotes ################
% ###############################
% lista automatica --
\usepackage{nomencl}
% --
% # end pacote      #############
```
--
2  - Imprimir a lista de abreviatura (deve estar no mesmo fluxo dos outros conteúdos)

```tex
\makenomenclature
\renewcommand{\nomname}{LISTA DE SÍMBOLOS E ABREVIATURAS}
\printnomenclature
\cleardoublepage
```
![saida-simbolos](img/listagem.png)

--
3 - Usar a nomenclatura

```text
%% usar a nomeclatura automatica
%% (vai ser ordenado por ordem alfabética
%%  o que estiver dentro \nomenclature{CB}{Caixa Branca} vai para o área de impresão
%% )

Eis uma previsão incomum nos dias atuais, mas feita de forma categórica: A computação em nuvem, tal como a conhecemos hoje, será obsoleta dentro de poucos anos. A conjectura é de ninguém menos que Peter Levine, Análise Fundamentalista (AF) \nomenclature{AF}{Análise Fundamentalista}.

Outro ponto é o RSI \nomenclature{RSI}{Índice de Força Relativa (Relative Strength Indicator)}

```
![uso-texto](img/uso-nomenclatura.png)

### fórmulas

### tabelas

### algoritmo em pt
