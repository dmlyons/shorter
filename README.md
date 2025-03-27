A simple url shortener

Have a redis address either on localhost:6379 or put an address into the environment variable `REDIS_ADDRESS`


```
go run main.go
```

Then you can

```
curl  -X POST -H 'Content-Type: application/json' localhost:8080/manage --data-raw '{"long_link":"https://cnn.com"}' 
{"short_link":"og6HR0vIwi"}
```

Then go to localhost:8080/<<whatever you got back from `short_link`>>

