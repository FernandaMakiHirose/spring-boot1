<h2>O que é o Spring Boot</h2>

* Fazer o build do projeto (comando **mvn clean install**).
* Explorar o conteúdo do arquivo .jar gerado.
* Executar o projeto no terminal com o comando **java -jar**.
* Trocar o formato do artefato para .war.

## Requisitos
- IDE e Java instalados.

## Licença
Distribuido sob a licença MIT License. Veja `LICENSE` para mais informações.

## Comandos
Para executar o projeto no após o build, digite o seguinte comando:

```shell script
java -jar target/springboot.jar 
```

Após executar o comando acima, basta apenas abrir o seguinte endereço e visualizar a execução do projeto:

```
http://localhost:8080
```

Para executar o projeto no tomcat, siga os seguintes passos:

```shell script
java -jar target/springboot.jar 
```

Após executar o comando acima, basta apenas abrir o seguinte endereço e visualizar a execução do projeto:

```
http://localhost:8080
```

<h3>Execução do projeto no format war através do Tomcat.</h3>

Para executar o projeto no Tomcat, siga os passos abaixo:

* No arquivo pom.xml, troque o valor da tag:

```xml
<packaging>jar</packaging>
```

* pelo seguinte valor:

```xml
<packaging>war</packaging>
```

* Faça o build do projeto:

```xml
mvn clean install
```

* Copie o o arquivo .war gerado para a pasta do Tomcat.

```shell script
mv target/springboot.war ../apache-tomcat-9.0.26/webpaps
```

* Inicie o Tomcat.

```shell script
bash apache-tomcat-9.0.26/bin/start.sh
```

Após executar o comando acima, basta apenas abrir o seguinte endereço e visualizar a execução do projeto:

```
http://localhost:8080/springboot
```
