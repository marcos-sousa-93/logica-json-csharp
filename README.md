# logica-json-csharp
entendendo a lógica da conversão do JSON para C#.
exemplo de JSON:
{
    "abilities": [
        {
            "ability": {
                "name": "run-away",
                "url": "https://pokeapi.co/api/v2/ability/50/"
            },
            "is_hidden": false,
            "slot": 1
        },
        {
            "ability": {
                "name": "guts",
                "url": "https://pokeapi.co/api/v2/ability/62/"
            },
            "is_hidden": false,
            "slot": 2
        },
        {
            "ability": {
                "name": "hustle",
                "url": "https://pokeapi.co/api/v2/ability/55/"
            },
            "is_hidden": true,
            "slot": 3
        }
    ]
}

A primeira chave é a classe-1{}, começa da linha 4 até a linha 31. que contém a propriedade "abilities" que recebe colchetes [] que são arrays ou listas que começa da linha 5 até a linha 30, a segunda chave é a classe-2{}, que começa da linha 6 até a linha 13 que se 
repete separados por vígula da linha 14 até a linha 21 e da linha 22 até a linha 29, ainda na segunda classe-2{} contém a propriedade "ability" que recebe valores da classe-3{} que é a terceira Chave, na clase-2{} além do "ability" temos também as propriedades
"is_hedden" e "slot" assim fechando a chave da segunda classe-2{}. E por último a terceira classe-3{} que começa da linha 7 até a linha 10 e se repete separados por vígulas da linha 15 até a linha 18 e da linha 23 até a linha 26, e contém as propriedades "name" e "url".

{
  "Propriedade 1" : [
    {
    "Propriedade 1.1" : {
        "Propriedade 1.1.1":"Valor1",
        "Propriedade 1.1.2":"Valor2"
        }
    "Propriedade 1.2
    "Propriedade 1.3
    }
  ]
}
