# Sistemas Distribuídos: trabalho 2 (Protocol Buffers)

> Calculadora e chat cliente-servidor em Java com mensagens serializadas em Protocol Buffers.

![status](https://img.shields.io/badge/status-concluído-success) ![java](https://img.shields.io/badge/Java-8-blue) ![protobuf](https://img.shields.io/badge/Protocol%20Buffers-3.1-green) ![maven](https://img.shields.io/badge/build-Maven-orange)

## Sobre
Trabalho 2 da disciplina de Sistemas Distribuídos (UFC Campus Quixadá, 2016), feito com Dieinison Jack. As mensagens de requisição e resposta são definidas em `.proto` e compiladas para Java; a comunicação é feita por sockets TCP. Inclui o exemplo `AddressBook` do tutorial oficial.

## Estrutura de pastas
```text
proto/calculadora.proto, addressbook.proto   definições das mensagens
src/main/java/ufc/sd/calc/                   Calculadora (gerado), CalculadoraCliente, CalculadoraServidor
src/main/java/ufc/sd/chat/                   Chat (gerado), ChatTCPCliente, ChatTCPServidor, ChatThread
src/main/java/ufc/sd/exemplo/                AddPerson, ListPeople, AddressBookProtos
pom.xml                                      dependência protobuf-java
```

## Como executar
```bash
mvn compile
mvn exec:java -Dexec.mainClass=ufc.sd.calc.CalculadoraServidor
mvn exec:java -Dexec.mainClass=ufc.sd.calc.CalculadoraCliente
```

## Status
Concluído. Trabalho acadêmico; não recebe manutenção.

## Autores
Ronildo Silva · ronildo.comp@gmail.com
Dieinison Jack
