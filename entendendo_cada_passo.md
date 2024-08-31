## logica-json-csharp
### Entendendo a lógica da conversão do JSON para C#.
### Exemplo de JSON:
<pre>
    <code>
{
    "habilidades": [
        {
            "habilidade": {
                "nome": "run-away",
                "url": "https://pokeapi.co/api/v2/ability/50/"
            },
            "esta_oculto": false,
            "slot": 1
        },
        {
            "Habilidade": {
                "nome": "guts",
                "url": "https://pokeapi.co/api/v2/ability/62/"
            },
            "esta_oculto": false,
            "slot": 2
        },
        {
            "Habilidade": {
                "nome": "hustle",
                "url": "https://pokeapi.co/api/v2/ability/55/"
            },
            "esta_oculto": true,
            "slot": 3
        }
    ]
}
    </code>
</pre>

<ul><li>A primeira chave é a classe-1.</li></ul>

<pre>
    <code>
{

}
    </code>
</pre>

<ul><li>Contém a propriedade "habilidades".</li></ul>

<pre>
    <code>
{
    "habilidades" :
}
    </code>
</pre>

<ul><li>A propriedade "habilidades" recebe colchetes [ ] que são arrays ou listas.</li></ul>

<pre>
    <code>
{
    "habilidades" : [
        
    ]
}
    </code>
</pre>

<ul><li>segunda chave é a classe-2.</li></ul>

<pre>
    <code>
{
    "habilidades" : [
        {
        
        }
    ]
}
    </code>
</pre>

<ul><li>A classe-2 contém as propriedades "habilidade", "esta_oculto" e "slot".</li></ul>

<pre>
    <code>
{        
    "habilidades" : [
        {
            "habilidade" :
            "esta_culto" :
            "slot" :
        }
    ]
}
    </code>
</pre>

<ul><li>A propriedade "habilidade" recebe a classe-3.</li></ul>

<pre>
    <code>
{        
    "habilidades" : [
        {
            "habilidade" : {
                
            },
            "esta_culto" :
            "slot" :
        }
    ]
}
    </code>
</pre>

<ul><li>A propriedade "esta_oculto" recebe uma valor Boolean "false", e a propriedade "slot" recebe um valor Inteiro "1".</li></ul>

<pre>
    <code>
{        
    "habilidades" : [
        {
            "habilidade" : {
                
            },
            "esta_culto" : false,
            "slot" : 1
        }
    ]
}
    </code>
</pre>

<ul><li>A classe-3 recebe 2 propriedades o "nome" que é uma string e "url" que também é uma string.</li></ul>

<pre>
    <code>
{        
    "habilidades" : [
        {
            "habilidade" : {
                "nome": "run-away",
                "url": "https://pokeapi.co/api/v2/ability/50/"
            },
            "esta_culto" : false,
            "slot" : 1
        }
    ]
}
    </code>
</pre>
