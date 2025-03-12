# spring-webflux-demo

wg https://howtodoinjava.com/spring-webflux/spring-webflux-tutorial/

## budowanie
bedac w katalogu zrodel wykonac polecenie

```
mvn -U clean package
```

## zainstalowac bazde danych MongoDb z domyslnym portem 27017

## uruchomienie
bedac w katalogu zrodel przejsc do katalogu

```
deploy\spring-webflux-demo
```

wykonac polecenie

```
java -jar spring-webflux-demo-0.0.1-SNAPSHOT.jar
```

powinien sie wyswietlic napis na konsoli

```
13:19:09.361 [main] INFO  o.s.b.w.e.n.NettyWebServer - Netty started on port(s): 8080
```

oznaczajacy uruchomnienie lokalnie serwera aplikacji ktora mozna teraz
testowac

## operacje http

inicjalne zaladowanie miliona rekordow do bazy
```
POST http://localhost:8080/all
```

utworzenie rekordu o ile mozliwe w bazie wg json
```
POST http://localhost:8080/create
```

wyszukanie rekordu o podanym id
```
GET http://localhost:8080/777777
```
