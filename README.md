# Api para consultar Cep:
## Serviços para consultar:
    https://viacep.com.br/ws/63050222/json
    http://api.postmon.com.br/v1/cep/63050222
    http://cep.republicavirtual.com.br/web_cep.php?cep=63050222&formato=json
    http://appservidor.com.br/webservice/cep?CEP=63050222

## Técnicas a ser usadas
    Pure Functions
    Currying
    Filter 
    Map
    Compose 
    Semântica no código
    Promise

## Tecnologias 
    NodeJS
    Express

***É requerido que evite smellcode e que o código seja Inglês***

## Pesquisa
    A Api receberá um GET na rota /api/v1/cep?code=" e o cep", vale salientar que a rota deverá ser tratada e possuir
o minímo requerido, que é:
    * 9 caracteres ou 8 (o usuário pode entrar com cep 99999-999 ou 99999999), caso contrário retorne um erro.
    * Retonar o Cep informado em json (caso não foi enconntrado, retornar um error)

    Na api terá que seguir o padrão de status code a seguir:
        * Url não encontrada status 404
        * Requisição Inválida 400
        * Erro interno da api 500
        * Retorno de Sucesso 200
    
    Retorno do JSON 
        {
            "zipcode": "63050-222",
            "street": "Rua Padre José Alves",
            "street_number": "de 59/60 ao fim",
            "neighborhood": "Salesianos",
            "city": "Juazeiro do Norte",
            "state": "CE",
            "ibge": "2307304",
        }

Boa sorte! = )
