# 💳 Cartão de Crédito - Gerenciador de Compras

![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)

> Aplicação console desenvolvida em Java para simular o controle de limite, saldo e lançamentos de compras em um cartão de crédito em tempo real.

## 📌 Sobre o Projeto

Este projeto foi desenvolvido como um desafio prático para consolidar conceitos fundamentais de **Programação Orientada a Objetos (POO)** e manipulação de estruturas de dados em Java. 

A aplicação interage com o usuário via console, permitindo definir um limite de crédito inicial e realizar múltiplas compras. O sistema valida o saldo disponível antes de aprovar cada transação e, ao finalizar, exibe o extrato consolidado com todas as compras **ordenadas de forma crescente pelo valor**.

## 🛠️ Tecnologias e Conceitos Aplicados

- **Java SE (Standard Edition)**
- **Orientação a Objetos:** Encapsulamento, classes, atributos e métodos bem definidos.
- **Estruturas de Dados:** Uso de `List` e `ArrayList` para o gerenciamento dinâmico do histórico de compras.
- **Ordenação:** Implementação da interface `Comparable` na regra de negócio para ordenação de objetos personalizados através do `Collections.sort()`.
- **Interação via Console:** Utilização da classe `Scanner` para captura e processamento seguro de entradas do usuário.

## 🏗️ Arquitetura do Sistema

O projeto é estruturado de forma limpa e coesa, dividido nas seguintes responsabilidades:

1. **`Compra`**: Entidade que representa o produto/serviço adquirido, contendo `descricao` e `valor`. Implementa `Comparable` para permitir a ordenação nativa por preço.
2. **`CartaoDeCredito`**: Classe de negócio responsável por gerenciar o `limite`, o `saldo` disponível e a lista de compras realizadas. Possui o método principal de validação de crédito (`lancaCompra`).
3. **`Principal` (Main)**: Classe controladora do fluxo da aplicação, responsável pelo menu iterativo, captura de dados do teclado e exibição dos resultados.

---

## 🚀 Como Executar o Projeto

### Pré-requisitos
Antes de começar, você vai precisar ter instalado em sua máquina:
- **Java JDK** (versão 17 ou superior recomendada).
- Uma IDE de sua preferência (ex: **IntelliJ IDEA**, Eclipse ou VS Code).

### Passos para Execução:

1. **Clone o repositório:**
   ```bash
   git clone [https://github.com/seu-usuario/2914-java-desafio.git](https://github.com/seu-usuario/2914-java-desafio.git)
