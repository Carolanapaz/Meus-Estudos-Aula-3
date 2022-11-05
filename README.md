# Meus-Estudos-Aula-3

/*Faça um algaritimo que dado as três notas tiradas por um aluno em um semestre de faculdade calcule e imprime a sua média e a sua classificação conforme tabela abaixo:

Média = (nota 1 + nota 2 + nota 3) / 3;

Classificação:
  -Média menor que 5, reprovação;
  -Média entre 5 e 7 , recuperação;
  -Média maior de 7, passou de semestre;*/
  
const nota1 = 5;
const nota2 = 6;
const nota3 = 8.5;
const media = (nota1 + nota2 + nota3) / 3;
console.log(media.toFixed(2));

if (media < 5) {
    console.log('Reprovado');
} else if (media >=5 && media <=7) {
    console.log('Recuperação');
} else {
    console.log('Aprovado');
}

Math.pow(altura,2) /*biblioteca matematica, para calcular potencia*/
------------------------------------------------------------------------------

/*O IMC Indice de Massa Corporal é um critério da Organização Mundial da Saúde para dar uma indicação sobre a condição de peso de uma pessoa adulta .
Formula do IMC:
IMC = peso / (altura * altura)

Elabore um algoritimo que dado o peso e a altura de uma adulto mostre sua condição de acordo com a tabela abaixo:

IMC em adulto. Condições:
  -Abaixo de 18.5: Abaixo do peso;
  -Entre 18.5 e 25: Peso normal;
  -Entre 25 e 30: Acima do peso;
  -Entre 30 e 40: Obeso;
  -Acima de 40: Obesidade grave;
*/

const peso = 69.7;
const altura = 1.59;
const imc = peso / Math.pow(altura,2);
console.log(imc);

if (imc < 18.5) {
    console.log('Abaixo do peso');
} else if (imc >= 18.5 && imc < 25) {
   console.log('Peso normal');
} else if (imc >= 25 && imc < 30) {
    console.log('Acima do peso');
} else if (imc >= 30 && imc < 40) {
    console.log('Obeso');
} else {
   console.log('Obesidade grave');
}

---------------------------------------------------------------------

/*Elabore um algoritmo que calcule o que deve ser pago por um produto , considerando o preço normal de etiqueta e a escolha da condição de pagamento.
Utilize os códigos da tabela a seguir para ler qual a condição de pagamento escolhida e efetuar o calculo adequado.
Código - CONDIÇÃO DE PAGAMENTO:
  - À vista débito, recebe 10% de desconto;
  - À vista no dinheiro ou PIX, recebe 15% de desconto;
  - Em duas vezes, preço normal da etiqueta sem juros;
  - Acima de duas vezes, preço normal da etiqueta mais 10% de juros;
*/

const valor = 100;
const debito = valor - (valor * 0.1);
const dinheiro = valor - (valor * 0.15);
const pix = valor - (valor * 0.15);
const parcelado2X = valor;
const parcelado3XouMais = (valor * 0.1) + valor;

let condicaoPagamento = pix;

if (condicaoPagamento === debito) {
    console.log(debito);
 } else if (condicaoPagamento === dinheiro) {
    console.log(dinheiro);
 } else if (condicaoPagamento === pix) {
    console.log(pix);
 } else if (condicaoPagamento === parcelado2X) {
    console.log(parcelado2X);
 } else if (condicaoPagamento === parcelado3XouMais) {
    console.log(parcelado3XouMais);
 }
 
 -------------------------------------------------------------
 
const precoEtiqueta = 500;
const formaPagamento = 3;

if (formaPagamento === 1) {
    console.log(precoEtiqueta - (precoEtiqueta * 0.1));
} else if (formaPagamento === 2) {
    console.log(precoEtiqueta - (precoEtiqueta * 0.15));
} else if (formaPagamento === 3) {
    console.log(precoEtiqueta + (precoEtiqueta * 0.1));
} else if (formaPagamento === 4) {
    console.log(precoEtiqueta + (precoEtiqueta * 0.15));
}
