## START CONTAINER
 - `docker-compose up -d --remove-orphans`
 - `docker-compose logs -f {service name}` -- to see the logs

## RUN POST QUERY
 - `curl -d "@data.json" -X POST http://localhost:8080/transactionservice/transactions/ -H "Content-Type: application/json"` *each request have incremented index, starting from 1 
 
## RUN GET QUERY
 - `curl http://localhost:8080/transactionservice/transactions/{id}` *need to specify `id`
