# Desafio 4: Exploração da Masmorra

## Descrição:
Sua missão é vasculhar as salas da masmorra em busca de recompensas lendárias e desafios perigosos. Cada sala pode conter monstros formidáveis, tesouros preciosos ou ambos. Use suas habilidades estratégicas para enfrentar as ameaças e coletar os tesouros!

## Entrada:
O número total de salas no dungeon (um número inteiro).

## Saída:
Sempre que encontrar um tesouro, imprima " Tesouro na sala X!".
Sempre que encontrar um monstro, imprima "Monstro na sala X!".

## Exemplos:
| Entrada |                                   Saída                                  |
|:-------:|:-----------------------------------------------------------------------:|
|    3    | Tesouro na sala 2! Monstro na sala 3!                                 |
|    4    | Tesouro na sala 2! Monstro na sala 3! Tesouro na sala 4!              |
|    2    | Tesouro na sala 2!                                                    |


### Resolução
```
// Entrada de dados.
const totalSalas = parseInt(gets());
// Aqui temos uma demonstração de array com valores já predefinidos:
const salasComTesouro = [2, 4, 7];
const salasComMonstro = [3, 6, 8];

// Aqui temos uma forma de loop para percorrer cada sala da masmorra:
for (let sala = 1; sala <= totalSalas; sala++) {
    // Utilizamos o .includes() para verificar se um número está presente nos arrays:
    const temTesouro = salasComTesouro.includes(sala);
    const temMonstro = salasComMonstro.includes(sala);

    // TODO: Agora implemente uma condição necessária para verificar e exibir se há tesouro na sala e se há monstro na sala:
    if (temTesouro) {
        print("Tesouro na sala " + sala + "!");
    } else if (temMonstro) {
        print("Monstro na sala " + sala + "!");
    }
}
```
