# 📚 Trabalho P1 – Estrutura de Dados - Samuel-Medeiros

## Sistema de Gerenciamento de Fila de Atendimento

---

## 👨‍🏫 Objetivo
Desenvolver um sistema simples que simule uma fila de atendimento, utilizando **obrigatoriamente o conceito de lista encadeada**.

O objetivo do trabalho é avaliar a compreensão de **estruturas de dados dinâmicas** e sua adaptação a diferentes linguagens de programação.

---

## 🧩 Contexto do Problema
Você deverá implementar um sistema que simula uma fila de atendimento, como por exemplo:

- Atendimento em banco  
- Fila de hospital  
- Atendimento em suporte técnico  
- Restaurante ou fila de pedidos  

---

## ⚙️ Funcionalidades obrigatórias
O sistema deve permitir:

- Inserir pessoa na fila  
- Atender próxima pessoa (remoção do início)  
- Exibir fila atual  
- Buscar pessoa na fila  
- Contar quantidade de elementos  

---

## 🧠 Requisito Obrigatório
A estrutura de dados **DEVE ser implementada manualmente como lista encadeada**.

### ❌ Não é permitido (salvo exceções conforme a linguagem):
- Arrays  
- Listas prontas da linguagem (`List`, `Vec`, `ArrayList`, etc.)  

### ✔ Deve existir:
- Estrutura de nó (`Node`)  
- Referência para o próximo elemento  
- Controle da lista (`head`)  

---

## 🖥️ Interface
Você pode escolher:

- Interface via terminal (CLI) → mais simples  
- Interface web simples → mais complexa (**pontuação extra**)  

---

## 👨‍💻 Linguagens por aluno

| Aluno   | Linguagem |
|--------|----------|
| Mahgid | Elixir   |
| Samuel | Rust     |
| Robert | Crystal  |
| João   | Java     |
| Rafael | Nim      |
| Alberto| Julia    |
| Caio   | Lean     |

---

## 🧠 Sobre ponteiros e referências

Nem todas as linguagens utilizam ponteiros da mesma forma.  
A implementação deve respeitar o paradigma de cada linguagem:

| Linguagem | Modelo |
|----------|--------|
| Rust     | Ponteiros seguros (`Box`, `Option`) |
| Java     | Referências de objetos |
| Crystal  | Referências |
| Elixir   | Estrutura recursiva imutável |
| Nim      | Ponteiros ou referências (`ref`) |
| Julia    | Estruturas mutáveis com referência |
| Lean     | Tipo indutivo recursivo |

---

## 📦 Entrega

### 🔹 Estrutura
Será utilizado um modelo com:

- 1 repositório principal  
- 1 repositório por aluno  

---

### 🔹 Repositório principal
Deve conter:

- Este enunciado  
- Lista de links para os repositórios dos alunos  
- Passo a passo de como instalar e rodar o projeto  

#### Exemplo:

```markdown
## Repositórios dos alunos

- Mahgid (Elixir): https://github.com/usuario/edc-p1-2026-projeto-elixir  
- Samuel (Rust): https://github.com/usuario/edc-p1-2026-projeto-rust  
- Robert (Crystal): https://github.com/usuario/edc-p1-2026-projeto-crystal  
- João (Java): https://github.com/usuario/edc-p1-2026-projeto-java  
- Rafael (Nim): https://github.com/usuario/edc-p1-2026-projeto-nim  
- Alberto (Julia): https://github.com/usuario/edc-p1-2026-projeto-julia  
- Caio (Lean): https://github.com/usuario/edc-p1-2026-projeto-lean  
```
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# 📋 Sistema de Fila - Trabalho 1 (Rust) 🚀

Um sistema simples de gerenciamento de fila desenvolvido em **Rust**, utilizando estruturas de dados dinâmicas para empilhar e atender usuários de forma sequencial (FIFO - First-In, First-Out).

---

## 🛠️ Guia de Instalação do Rust (Windows)

Para rodar este projeto, você precisa ter o ecossistema Rust instalado em sua máquina. Siga os passos abaixo:

### 1. Instalar o Rust via Rustup
O **Rustup** é o instalador oficial.
1. Acesse o site oficial: [rust-lang.org](https://www.rust-lang.org/tools/install).
2. Baixe o executável `rustup-init.exe` para Windows (64-bit ou 32-bit conforme seu sistema).
3. Execute o arquivo e siga as instruções no terminal:
   - Se ele pedir para instalar o **Visual Studio Build Tools**, aceite (necessário para o compilador).
   - Escolha a opção padrão (geralmente digitando `1` e dando Enter).
4. Após a conclusão, **feche e abra novamente seu terminal** (PowerShell ou Prompt de Comando) para que as variáveis de ambiente sejam carregadas.

### 2. Verificar a Instalação
No terminal, digite os comandos abaixo para garantir que tudo está ok:
```powershell
rustc --version
cargo --version
```
Se ambos retornarem uma versão, o Rust está pronto para uso!

---

## 📂 Como Instalar e Rodar o Projeto

Siga estes passos para configurar e executar o sistema localmente:

### 1. Navegar até a Pasta do Projeto
Abra o terminal e use o comando `cd` para entrar na pasta do projeto:
```powershell
# Exemplo se estiver na pasta samuel
cd trabalho1
```

### 2. Compilar e Rodar
O comando abaixo irá baixar as dependências (se houver), compilar o código e iniciar a aplicação:
```powershell
cargo run
```

### 3. (Opcional) Gerar Executável de Produção
Se quiser apenas o arquivo `.exe` otimizado:
```powershell
cargo build --release
```
O arquivo gerado estará em `./target/release/trabalho1.exe`.

---

## 📋 Comandos do Sistema

Ao iniciar o programa, você verá um menu interativo com as seguintes opções:

| Opção | Comando | Descrição |
| :--- | :--- | :--- |
| **1** | **Inserir** | Adiciona uma nova pessoa ao final da fila. |
| **2** | **Atender** | Remove e exibe o nome da primeira pessoa da fila. |
| **3** | **Exibir** | Mostra toda a fila atual no formato `[Nome] -> ... -> FIM`. |
| **4** | **Buscar** | Verifica se um nome específico está presente na fila. |
| **5** | **Contar** | Exibe a quantidade total de pessoas aguardando. |
| **0** | **Sair** | Encerra a aplicação. |

---

## 🏗️ Estrutura do Projeto
- `src/main.rs`: Código fonte principal com a lógica da Fila.
- `Cargo.toml`: Arquivo de configuração do projeto e dependências.
- `README.md`: Este guia de instruções.

- ---

## ✅ Validação, Testes e Ferramentas Utilizadas

Antes da versão final, o projeto passou por um processo estruturado de desenvolvimento:

- Foi criada uma **primeira versão para testes**, com foco em validar a lógica da lista encadeada e o funcionamento das operações da fila  
- Após validação completa, o código foi **reescrito (refatorado) em um novo projeto**, aplicando melhorias de organização, legibilidade e boas práticas  

### 🧪 Testes realizados
- Inserção e remoção de elementos na fila  
- Busca por elementos  
- Consistência da estrutura encadeada  
- Contagem correta dos nós  

---

## Video do Desenvolvimento

https://youtu.be/acEX4n2vHFc

---

## ☁️ Ferramentas e Tecnologias de Apoio

Durante o desenvolvimento, foram utilizadas ferramentas de apoio para acelerar o aprendizado e validação de ideias:

- ☁️ Ambiente em nuvem para execução e testes  
- 🤖 ChatGPT – suporte na compreensão de conceitos e revisão de lógica  
- 🤖 Gemini – apoio complementar na implementação e validação  

> ⚠️ Importante: Todo o código final foi **escrito manualmente**, sem cópia direta de soluções prontas, garantindo o entendimento completo da implementação.

---
