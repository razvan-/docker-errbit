== Errbit Docker ( yet another )

```docker run -d --name mongo1 mongo```
```docker run -d --name errbit1 --link mongo1:mongo -p 18080:8080 itnovate/errbit```
```docker exec -ti errbit1 rake assets:precompile```
```docker exec -ti errbit1 rake errbit:bootstrap```

Note the credentials and you're good to go.


