<h2>Exercício Juntos - O que é o Spring Boot</h2>


Projeto desenvolvido do tópico Exercício juntos, referente à parte 3 da aula sobre  **O que é o Spring Boot**, gravado para a Digital Innovation One.

Na aula, foram desenvolvidos os seguintes passos:

* Fazer o build do projeto (comando **mvn clean install**)
* Explorar o conteúdo do arquivo .jar gerado
* Executar o projeto no terminal com o comando **java -jar**
* Trocar o formato do artefato para .war

O projeto consta com todos os passos desenvolvidos acima.

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

<h3>Execução do projeto no format war através do Tomcat</h3>

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

* Copie o o arquivo .war gerado para a pasta do Tomcat

```shell script
mv target/springboot.war ../apache-tomcat-9.0.26/webpaps
```

* Inicie o Tomcat

```shell script
bash apache-tomcat-9.0.26/bin/start.sh
```

Após executar o comando acima, basta apenas abrir o seguinte endereço e visualizar a execução do projeto:

```
http://localhost:8080/springboot
```

## Sobre a Autora
Oi, eu sou a Fernanda! Estou aqui para contribuir com meu conhecimento e espero poder ajudar no desenvolvimento profissional de cada um de vocês.

[![Linkedin Badge](https://img.shields.io/badge/-Fernanda_Maki_Hirose-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/fernanda-maki-hirose-801117208/)](https://www.linkedin.com/in/fernanda-maki-hirose-801117208/)  [![Gmail Badge](https://img.shields.io/badge/-femahi2020@gmail.com-c14438?style=flat-square&logo=Gmail&logoColor=white&link=mailto:femahi2020@gmail.com)](mailto:femahi2020@gmail.com)







