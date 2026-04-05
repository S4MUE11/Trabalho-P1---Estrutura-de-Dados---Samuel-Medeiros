# Trabalho-P1---Estrutura-de-Dados---Samuel-Medeiros

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
