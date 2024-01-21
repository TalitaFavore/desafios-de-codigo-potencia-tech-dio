# Desafio 1: Jornada pela Floresta

## Descrição:
Você é um jovem herói que embarca em uma jornada épica para derrotar o temido dragão que aterroriza o reino. No entanto, você precisa atravessar uma floresta perigosa para chegar à caverna do dragão. Cada passo é crucial, e sua jornada será determinada pela lógica afiada que você possuir.

## Tarefa:
Escreva um algoritmo que simule a jornada do herói pela floresta. O herói começa em uma posição inicial e deve dar uma série de passos para atravessar a floresta até a caverna do dragão.

## Entrada:
A posição inicial do herói na floresta (um número inteiro).
O número total de passos que o herói deve dar (um número inteiro).

## Saída:
Imprima a posição final do herói após dar a quantidade de passos especificada.

## Exemplos:
| Entrada |          Saída               |
|:-------:|:---------------------------:|
|    2    | Posição final do herói: 5   |
|    3    | Posição final do herói: 18  |
|   10    | Posição final do herói: 16  |


### Resolução
```
const posicaoInicial = parseInt(gets());
const totalPassos = parseInt(gets());

//TODO: Calcule a posição final do herói:
const posicaoFinal = posicaoInicial + totalPassos;

// Imprime a posição final
print("Posição final do herói: ", posicaoFinal);
```

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

# Desafio 5: Mineração de Minérios

## Descrição:
Você é um mestre construtor em um mundo de blocos e tem a tarefa de gerar biomas em diferentes regiões do mundo. Cada bioma tem características únicas, como tipos de solo, vegetação e clima.

## Tarefa:
Sua tarefa é coletar minérios enquanto ataca uma rocha com sua picareta. Use loops e lógica de programação para representar cada golpe na rocha e determinar qual minério foi obtido.

## Entrada:
O programa irá solicitar que você digite um número inteiro positivo representando a quantidade de golpes que você deseja dar com a picareta.

## Saída:
Para cada golpe que você der, o programa exibirá uma mensagem indicando o resultado do golpe. Será mostrado o número do golpe e o minério obtido, que pode ser 1: Carvao, 2: Ferro, 3: Diamante e 4: Pedra.

## Exemplos:
| Entrada |                          Saída                                |
|:-------:|:------------------------------------------------------------:|
|    4    | 1: Carvão 2: Ferro 3: Diamante 4: Pedra                     |
|    3    | 1: Carvão 2: Ferro 3: Diamante                               |
|    2    | 1: Carvão 2: Ferro                                           |


### Resolução
```
// Lê a quantidade de golpes informada pelo usuário.
// O parseInt(()) vai converter os valores de entrada(string) para um valor numérico(Int).
const quantidadeGolpes = parseInt(gets());

// TODO: Defina aqui os tipos de minerais Carvao, Ferro, Diamante e Pedra
let minerais = ["Carvão", "Ferro", "Diamante", "Pedra"];

// Loop para cada golpe, de 1 até a quantidade informada
for (let i = 1; i <= quantidadeGolpes; i++) {
    // Calcula o índice do mineral usando o operador de módulo (%) para garantir que o índice esteja dentro do tamanho do array
    let minaIndex = (i - 1) % minerais.length;

    // TODO: Agora exiba o índice i, concatene com o caractere ":", após, concatene com tipo de minerais[minaIndex]:
    print(i + ": " + minerais[minaIndex]);
}
```
