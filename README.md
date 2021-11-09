# CSS: Tableless
**Tableless** é uma metodologia de desenvolvimento de páginas web que não utiliza tabelas para disposição de conteúdo na página sugerido pela W3C. 
O objetivo dessa metodologia é tornar o código fonte HTML o mais semântico, aproveitando as propriedade de posionamento da linguagem CSS.

## Dimensões
### width: largura
``` css
.boxe {
  width: 100px; 
}
```
### height: altura
``` css
.boxe {
  height: 100px; 
}
```
### Espaçamento interno / externo
#### padding: espaçamento interno
``` css
.boxe {
  padding: 10px; 
}
/*
  Nota: Por padrão o valor de espaçamento interno é somado ao valor final.

  Considerando a largura / altura de 100px, nosso boxe passaria ter largura / altura de 120px.
  width: 100px; + padding-left: 10px + padding-right: 10px; = 120px;
  heiht: 100px; + padding-top: 10px + padding-bottom: 10px; = 120px;  
*/
```
#### margin: espaçamento externo
``` css
.boxe {
  margin: 10px; 
}
/*
  Nota: Apesar de não alterar a dimensão interna, o espaçamento externo é calculado no momento do posicionamento, 
  podendo ocasionar quebras de linha.

  Considerando a largura / altura de 100px, nosso boxe passaria ter largura / altura de 120px.
  width: 100px; + margin-left: 10px + margin-right: 10px; = 120px de espaço ocupado horizontal;
  heiht: 100px; + margin-top: 10px + margin-bottom: 10px; = 120px de espaço ocupado na vertical;  
*/
```
## Personalização
### background-color: cor
### border: espessura estilo cor
``` css
.boxe {
  border-width: 5px;
  border-color: white;
  border-style: solid;
}
/*
  Nota: Por padrão o valor de borda é somado ao valor final.

  Considerando a largura / altura de 100px, nosso boxe passaria ter largura / altura de 110px.
  width: 100px; + border-width-left: 5px + border-width-right: 5px; = 110px;
  heiht: 100px; + border-width-top: 5px + border-width-bottom: 5px; = 120px;  
*/
```
**Nota:** Por padrão a propriedade `border` é somada a dimensão do boxe.
### font-family: 'Fonte 1', 'Fonte 2'...
### font-size: tamanho
``` css
.titulo {
  font-size: 24px; 
}
```
## Posicionamento
### text-align: center | left | right | justify
``` css
.boxe {
  text-align: center; 
}
```
### float: left | right
``` css
.boxe {
  float: left; 
}
```
### clear: none | left | right | both
``` css
.boxe {
  clear: left; 
}
```
### overflow: visible | hidden | scroll | auto | inherit
