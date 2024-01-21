# Desafio 2: Ganho de XP após Batalha

## Descrição:
Você é um herói em um mundo mágico repleto de monstros e desafios. Sua missão agora é enfrentar inimigos e ganhar pontos de experiência (XP) para se tornar mais forte. A cada vitória, você ganha XP e se aproxima de se tornar um lendário campeão.

## Tarefa:
Escreva um programa simples que simule o ganho de XP após derrotar um monstro. O programa deve calcular e exibir a quantidade de XP ganhos com base no nível do monstro e na dificuldade da batalha.

## Entrada:
O nível do monstro (um número inteiro).
A dificuldade da batalha, representada por um valor de 1 a 100 (um número inteiro).

## Saída:
Imprima a quantidade de XP ganhos após a batalha.

## Exemplos:
| Entrada |       Saída                |
|:-------:|:-------------------------:|
|   45    | Você ganhou 180000 XP!    |
|   41    | Você ganhou 155800 XP!    |
|   15    | Você ganhou 30000 XP!     |


### Resolução
```
// Entrada de dados.
let num1 = parseInt(gets());
let num2 = parseInt(gets());

//TODO: Implemente a lógica para exibir o xpGanho:
const xpGanho = num1 * num2 * 100;
// Imprime a quantidade de XP ganho
print("Você ganhou " + xpGanho + " XP!");
```

