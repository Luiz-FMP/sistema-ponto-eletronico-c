# Sistema de Ponto Eletrônico em C ⏱️

[![C](https://img.shields.io/badge/Linguagem-C-blue.svg)](https://en.wikipedia.org/wiki/C_(programming_language))
[![Versão](https://img.shields.io/badge/Vers%C3%A3o-v1.0%20(Inicial)-green.svg)]()
[![Licença](https://img.shields.io/badge/Licen%C3%A7a-MIT-lightgrey.svg)]()

Sistema desenvolvido em linguagem **C** para gerenciamento de funcionários, marcação de ponto e acompanhamento de horas trabalhadas. Projeto acadêmico desenvolvido para a **Universidade Positivo**.

> 📌 **Nota sobre a versão:** Esta é a **primeira versão (v1.0)** do projeto, focada na lógica de negócio essencial, gerenciamento dinâmico de memória e implementação de estruturas de dados e algoritmos clássicos em C.

---

## 🚀 Funcionalidades

- [x] **Cadastrar Funcionários**: Inclusão dinâmica de colaboradores com nome, matrícula e função.
- [x] **Marcar Ponto**: Registro completo dos horários de entrada, intervalo (início e fim) e saída, associados a uma data.
- [x] **Ranking de Horas Trabalhadas**: Listagem ordenada dos funcionários com maior carga horária acumulada, implementada com o algoritmo **QuickSort**.
- [x] **Buscar Ponto**: Consulta de registros de ponto com filtros por funcionário ou por data.
- [x] **Gerenciamento de Memória**: Estruturas alocadas dinamicamente com liberação de memória ao encerrar a aplicação.

---

## 🛠️ Tecnologias e Conceitos Utilizados

- **Linguagem C**: Padrão ANSI/C99.
- **Alocação Dinâmica de Memória**: Uso de `malloc`, `realloc` e `free` para crescimento sob demanda dos vetores de funcionários e registros.
- **Estruturas de Dados (`struct`)**:
  - `Funcionario`: Armazena dados cadastrais e total de horas.
  - `Data`: Armazena dia, mês e ano.
  - `RegistroPonto`: Associa funcionário, data e horários de entrada/intervalo/saída.
- **Algoritmo de Ordenação**: Implementação manual do **QuickSort** para ordenação eficiente dos funcionários por horas trabalhadas.

---

## 💻 Como Compilar e Executar

### Pré-requisitos
* Compilador C instalado (como **GCC** via MinGW no Windows ou nativo no Linux/macOS).

### 1. Clonar o repositório
```bash
git clone https://github.com/Luiz-FMP/sistema-ponto-eletronico-c.git
cd sistema-ponto-eletronico-c
```

### 2. Compilar via terminal
```bash
gcc ponto.c -o ponto.exe
```

### 3. Executar
* **Windows**:
  ```powershell
  .\ponto.exe
  ```
* **Linux/macOS**:
  ```bash
  ./ponto
  ```

> 💡 **Dica (VS Code / Antigravity IDE):** Se você usa a extensão **Code Runner**, basta abrir o arquivo `ponto.c` e pressionar `Ctrl + Alt + N`.

---

## 📋 Menu da Aplicação

Ao iniciar o programa, o menu principal interativo é exibido no terminal:

```text
=========== MENU INICIO ===========
1 - Marcar ponto
2 - Cadastrar funcionario
3 - Horas trabalhadas
4 - Buscar ponto
0 - Sair
Escolha uma opcao:
```

---

## 🗺️ Próximos Passos (Roadmap para versões futuras)

- [ ] **Persistência de Dados**: Gravação e leitura dos cadastros e pontos em arquivos (`.txt`, `.csv` ou binário) para manter os dados após fechar o programa.
- [ ] **Cálculo Automático de Horas**: Parser para calcular automaticamente as horas trabalhadas subtraindo os horários de entrada, intervalo e saída.
- [ ] **Validação de Entradas**: Verificação rigorosa do formato de horários (`HH:MM`) e datas válidas no calendário.
- [ ] **Interface Gráfica / CLI Aprimorada**: Melhorias na experiência do usuário e na navegação de menus.

---

## 👥 Autores

* **Luiz Felipe** - [@Luiz-FMP](https://github.com/Luiz-FMP)
* **Luis Arthur**
