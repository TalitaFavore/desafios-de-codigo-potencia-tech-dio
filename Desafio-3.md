# Desafio 3: Escolha do Pokémon Inicial

## Descrição:
No mundo dos jogos Pokémon, os treinadores começam sua jornada escolhendo um dos três Pokémons iniciais: Bulbasaur, Charmander e Mewtwo. Seu desafio é criar uma solução que permita ao jogador escolher um dos Pokémons iniciais e exibir uma mensagem de boas-vindas e o Pokémon escolhido.

## Entrada:
Você receberá um número inteiro que representa a escolha do treinador: 1 para Bulbasaur, 2 para Charmander, 4 para Pikachu e 5 para Mewtwo.

## Saída:
A saída deve ser uma mensagem de boas-vindas que inclua o nome do Pokémon escolhido.

## Exemplos:
| Entrada |                                Saída                                       |
|:-------:|:------------------------------------------------------------------------:|
|    1    | Você escolheu o Bulbasaur como seu Pokémon inicial.                      |
|    2    | Você escolheu o Charmander como seu Pokémon inicial.                     |
|    4    | Você escolheu o Pikachu como seu Pokémon inicial.                        |
|    5    | Você escolheu o Mewtwo como seu Pokémon inicial.                         |


### Resolução
```
// Entrada de dados.
let escolhaDoTreinador = parseInt(gets());
let pokemonEscolhido;

//TODO: Implemente as condições necessárias para a solução do desafio.
if (escolhaDoTreinador === 1) {
    pokemonEscolhido = "Bulbasaur";
} else if (escolhaDoTreinador === 2) {
    pokemonEscolhido = "Charmander";
} else if (escolhaDoTreinador === 4) {
    pokemonEscolhido = "Pikachu";
} else if (escolhaDoTreinador === 5) {
    pokemonEscolhido = "Mewtwo";
} else if {
    print("Número inválido")
}

//Imprime o Pokémon escolhido:
if (pokemonEscolhido) {
    print("Você escolheu o " + pokemonEscolhido + " como seu Pokémon inicial.");
}
```
