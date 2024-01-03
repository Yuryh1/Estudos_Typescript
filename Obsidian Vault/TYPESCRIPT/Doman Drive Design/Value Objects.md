Tbm contem regras de negocio independentes, no entanto são identificados pelo seu valor , sendo imutáveis ou seja , a mudança implica na sua substituição 

Características

. Mede , quantifica ou descreve alguma coisa
. Seu valor é imutável
. É substituído quando seu valor mudar 
. Pode ser comparado pelo valor que representa 

Exemplo 
CPF: garante que o numero do documento é valido
Password: Representa uma senha
Email: Representa um Email .


------------------------------------------------

Substituir por um ou mais primitivos

Uma técnica para identificar um Value Object é tentar substitui-lo por um tipo primitivo como uma string ou um numero 

--------------------------------------------------------
exemplo de objeto de valor em TypeScript é o seguinte:

TypeScript

```TypeScript

export class Data {
  constructor(public readonly dia: number, public readonly mes: number, public readonly ano: number) {}

  equals(outraData: Data): boolean {
    return this.dia === outraData.dia && this.mes === outraData.mes && this.ano === outraData.ano;
  }
}
```

Use o código com cuidado. [Saiba mais](https://bard.google.com/faq#coding)

content_copy

Este objeto de valor representa uma data. Ele tem três atributos, `dia`, `mes` e `ano`, que são números inteiros. O método `equals()` é usado para comparar duas datas.

Aqui está um exemplo de como usar este objeto de valor:

TypeScript

```Typescript
const data1 = new Data(19, 7, 2023);
const data2 = new Data(19, 7, 2023);

console.log(data1.equals(data2)); // true
```

Use o código com cuidado. [Saiba mais](https://bard.google.com/faq#coding)

content_copy

Este código imprime `true`, pois as duas datas têm os mesmos valores para `dia`, `mes` e `ano`.

Objetos de valor podem ser usados para representar uma ampla variedade de conceitos no domínio. Eles são uma ferramenta valiosa que pode ajudar a melhorar a qualidade do software.

Características
• Mede, quantifica ou descreve alguma coisa
• Seu valor é imutável
• É substituido quando seu valor mudar
• Pode ser comparado pelo valor que representa

Exemplos Code: Representa uma determinada regra de formação de um número Cpf: Garante que o número do documento é válido Dimension: Abstrai a largura, altura, profundidade e peso de um item Password: Representa uma senha Color: Uma cor no formato RGB Coord: A latitude e longitude Email: Representa um email Position: Representa uma posição geográfica no tempo Segment: Representa duas posições geográficas no tempo


Substituir por um ou mais primitivos Uma técnica para identificar um value object é tentar substituí-lo por um tipo primitivo como uma string ou um número