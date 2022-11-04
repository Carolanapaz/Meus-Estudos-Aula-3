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
