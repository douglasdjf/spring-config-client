# Acesso 

### endpoint para teste : http://localhost:8080/greeting

### A alteração do profile do config server está no arquivo application.yml:

### QA
```
  cloud:
    config:
      profile: qa
```

### DEV
```
  cloud:
    config:
      profile: dev
```

### HML
```
  cloud:
    config:
      profile: hml
```


### Para que alguma alteração em tempo de execução seja refletida na aplicação cliente é necessário fazer uma requisição simples do tipo POST para :http://localhost:8080/actuator/refresh
Com isso, o spring config server vai atualizar e buscar as configurações do github