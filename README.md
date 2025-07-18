# Modelagem de um Sistema de Celulares em C#

![C#](https://img.shields.io/badge/c%23-%23239120.svg?style=for-the-badge&logo=c-sharp&logoColor=white) ![.Net](https://img.shields.io/badge/.NET-5C2D91?style=for-the-badge&logo=.net&logoColor=white)

## 📖 Sobre o Projeto

Este projeto é uma solução para um desafio de programação que visa demonstrar a aplicação prática dos pilares da **Programação Orientada a Objetos (POO)**. O objetivo foi criar uma abstração de um celular, permitindo que diferentes marcas (como Nokia e iPhone) herdem características comuns, mas implementem comportamentos específicos, como a instalação de aplicativos.

---

## 🚀 Principais Conceitos de POO Aplicados

O núcleo deste projeto é a demonstração clara dos seguintes conceitos:

### 1. Abstração
- Foi criada uma `abstract class Celular` que serve como um "contrato" ou molde para todos os celulares.
- Ela define propriedades e métodos que são comuns a qualquer celular (Ex: `Numero`, `Ligar()`), garantindo uma base sólida e reutilizável.

### 2. Herança
- As classes `Nokia` e `Iphone` **herdam** da classe `Celular`.
- Ao herdar, elas automaticamente ganham todo o comportamento e características da classe base, o que promove o **reuso de código** e evita repetições.

### 3. Polimorfismo
- A classe `Celular` possui um método `abstract void InstalarAplicativo()`. Um método abstrato força as classes filhas a criarem sua própria implementação.
- Tanto `Nokia` quanto `Iphone` **sobrescrevem** (`override`) este método, cada uma com seu comportamento único (uma instala pela "Loja Ovi", a outra pela "App Store").
- Isso permite que, ao chamar o mesmo método, a ação executada seja diferente dependendo do tipo do objeto, que é a essência do polimorfismo.

---

## 🛠️ Tecnologias Utilizadas

- C# 12
- .NET 8.0
- Git e GitHub para versionamento

---

## ⚙️ Como Executar o Projeto

### Pré-requisitos

Antes de começar, você vai precisar ter instalado em sua máquina as seguintes ferramentas:
* [.NET 8.0 SDK](https://dotnet.microsoft.com/pt-br/download/dotnet/8.0)
* [Git](https://git-scm.com/downloads)

### Rodando a Aplicação

1.  **Clone este repositório:**
    ```bash
    git clone [https://github.com/tarxdev/sistema-celular-oop-csharp.git](https://github.com/tarxdev/sistema-celular-oop-csharp.git)
    ```

2.  **Navegue até a pasta do projeto:**
    ```bash
    cd sistema-celular-oop-csharp/src
    ```

3.  **Execute o aplicativo:**
    ```bash
    dotnet run
    ```
O terminal exibirá a saída dos testes, demonstrando os métodos comuns sendo executados e, mais importante, o método `InstalarAplicativo` se comportando de maneira diferente para cada marca de celular.

---

## 👨‍💻 Autor

Feito por **[Tarciso Ferreira]**.

