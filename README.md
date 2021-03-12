
#  Gerenciador Super Herois digital innovation one - spring webflux - JAVA

## Stack utilizada

  * Java14
  * Spring webflux
  * Spring data
  * Dynamodb
  * Junit
  * Sl4j
  * Reactor
  

### Slides de palestra: https://speakerdeck.com/kamilahsantos/live-coding-dio-api-de-herois-com-spring-webflux

### Palestra garavda: https://www.youtube.com/watch?v=1VllPZYn6RI&t=3257s





### Executar dynamo: 

 na pasta em que o jar está baixado: java -Djava.library.path=./DynamoDBLocal_lib -jar DynamoDBLocal.jar -sharedDb
 
para listar as tabelas criadas:  aws dynamodb list-tables --endpoint-url http://localhost:8000


documentacao gerada pela aplicação: swagger: http://localhost:8080/swagger-ui-heroes-reactive-api.html


### Link Postman Canary Projeto:

https://documenter.getpostman.com/view/14923100/Tz5p6y4m 

Linguagem cURL

curl --location --request GET 'http://localhost:8080/heroes'

curl --location --request GET 'http://localhost:8080/heroes/7'

curl --location --request POST 'http://localhost:8080/heroes' \
--data-raw '{
        "id": "10",
        "name": "Wolverine",
        "universe": "marvel",
        "films": 16
}'

curl --location --request DELETE 'http://localhost:8080/heroes/4'
