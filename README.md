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

------------------------------------------------------------------------------

/*O IMC Indice de Massa Corporal 
