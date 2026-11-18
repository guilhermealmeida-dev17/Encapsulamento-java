# Exercícios de encapsulamento em Java

Aplicação de console que reúne três exemplos de modelagem com atributos privados, métodos de acesso e regras de validação.

## Módulos

- **Carros:** dados do veículo, ações de ligar/desligar/buzinar, cálculo de tempo de trajeto e valor para encher o tanque.
- **Contas bancárias:** consulta de saldo, depósitos, saques e transferências com validações.
- **Produtos:** alteração de preço e quantidade em estoque com validação de valores não negativos.

## Tecnologias e conceitos

- Java e JDK
- Encapsulamento com campos privados e métodos públicos
- Classes, construtores e validação de regras
- Menus interativos com `Scanner`

## Como executar

O código-fonte fica em `src/main/java` e não há configuração Maven ou Gradle neste repositório. Com um JDK instalado, compile os arquivos pelo PowerShell:

```powershell
$sources = Get-ChildItem .\src\main\java -Recurse -Filter *.java | ForEach-Object { $_.FullName }
New-Item -ItemType Directory -Force out | Out-Null
javac -d out $sources
java -cp out br.edu.fatecpg.encapsulamento.view.Main
```

Este projeto é um exercício acadêmico de console; não usa persistência em banco de dados.
