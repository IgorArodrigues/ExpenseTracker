# 💰 Gastos Mensais - Sistema de Controle Financeiro

> **Um sistema completo para controle de gastos mensais com interface web intuitiva**

[![GitHub](https://img.shields.io/badge/GitHub-Repository-blue?style=flat-square&logo=github)](https://github.com/IgorArodrigues/ExpenseTracker)

## 📋 Índice

- [Navegação](#navegação)
- [Estrutura da Aplicação](#estrutura-da-aplicação)
- [Telas e Funcionalidades](#telas-e-funcionalidades)
- [Como Usar](#como-usar)
- [Executável Local](#executável-local)

---

## 🧭 Navegação

### Dashboard - Ponto Central

Na página inicial do Dashboard, os **cartões de resumo** oferecem navegação rápida para todas as seções da aplicação:

| Seção | Destino | Descrição |
|-------|---------|-----------|
| 💰 **Receitas** | `/dashboard` | Acesso direto ao Dashboard |
| 💸 **Despesas** | `/expense` | Tela de Despesas Fixas |
| 💳 **Saldo** | `/balance` | Saldo com histórico e previsão |
| 📊 **Transações** | `/historico` | Histórico detalhado |

---

## 🏗️ Estrutura da Aplicação

```
GastosMensais
├── 🔐 Login (tela inicial)
│   ├── 📝 Registro
│   ├── 🔑 Esqueci minha senha
│   └── 🏠 Dashboard
│       ├── 💸 Despesas (Recorrências)
│       ├── 💳 Saldo (Histórico e Previsão)
│       └── 📊 Histórico (Filtros de transações)
```

---

## 🖥️ Telas e Funcionalidades

### 1. 🔐 **Login** (`/`, `/login`)
> **Tela de entrada da aplicação**

- **Funcionalidades:**
  - Autenticação com usuário e senha
  - Link para registro de nova conta
  - Recuperação de senha
  - Redirecionamento automático para o Dashboard

### 2. 📝 **Registro** (`/register`)
> **Criação de novas contas**

- **Campos obrigatórios:**
  - Nome completo
  - Sobrenome
  - Nome de usuário
  - E-mail
  - Senha
- **Fluxo:** Cadastro → Redirecionamento para Login

### 3. 🔑 **Esqueci minha senha** (`/forgot-password`)
> **Recuperação segura de conta**

- **Processo:**
    - Busca por nome de usuário ou e-mail
    - Envio de código de verificação
    - Definição de nova senha
- **Segurança:** Verificação por e-mail

### 4. 🏠 **Dashboard** (`/dashboard`)
> **Painel principal e centro de controle**

#### 📊 **Resumo Financeiro**
- Total de receitas do mês
- Total de despesas do mês
- Saldo atual
- Contagem de transações

#### ⚡ **Funcionalidades Principais**
- ✅ Adição de novas transações
- 📈 Gráficos de distribuição (receitas vs despesas)
- 📋 Lista das 10 transações mais recentes
- 🧭 Navegação para todas as seções

### 5. 💸 **Despesas Fixas** (`/expense`)
> **Gestão de transações recorrentes**

#### 🎯 **Foco em Recorrências**
- Assinaturas mensais
- Pagamentos fixos
- Contas recorrentes

#### 📊 **Visualização**
- Gráfico de pizza por categoria
- CRUD completo (Criar, Ler, Atualizar, Deletar)
- Organização por prioridade

### 6. 💳 **Saldo** (`/balance`)
> **Histórico e previsão financeira**

#### 📈 **Análise Temporal**
- Histórico de saldo mensal
- Previsão futura (regressão linear)
- Variação mensal

#### 📊 **Relatórios**
- Tabela detalhada (receitas, despesas, saldo, variação)
- Gráficos de linha (histórico e previsão)
- Análise de tendências

### 7. 📊 **Histórico** (`/historico`)
> **Filtros avançados e análise detalhada**

#### 🔍 **Filtros Disponíveis**
- **Por data específica:**
  - Mês específico
  - Ano específico
  - Dia específico
- **Por intervalo:** Período personalizado

#### 📈 **Visualizações Dinâmicas**
- Distribuição por forma de pagamento
- Resumo mensal (receitas vs despesas)
- Gráficos interativos
- Exportação de dados

---

## 🚀 Como Usar

### **Primeiro Acesso**
1. Acesse a tela de **Login**
2. Clique em **"Registrar"** para criar sua conta
3. Preencha seus dados pessoais
4. Faça login com suas credenciais

### **Uso Diário**
1. **Dashboard:** Visualize seu resumo financeiro
2. **Adicione transações** através do formulário disponivel na tela inicial
3. **Navegue pelas seções** conforme sua necessidade:
   - 💸 **Despesas:** Para gerenciar gastos fixos
   - 💳 **Saldo:** Para análise de tendências
   - 📊 **Histórico:** Para consultas detalhadas

### **Dicas de Uso**
- ⭐ **Mantenha suas despesas fixas atualizadas**
- 📊 **Monitore regularmente o histórico**
- 💡 **Use os gráficos para identificar padrões**
- 🔄 **Faça backup regular dos seus dados**

---

## 🛠️ Tecnologias Utilizadas

- **Backend:** Python Flask
- **Frontend:** HTML, CSS, JavaScript
- **Banco de Dados:** SQLite
- **Gráficos:** Chart.js
- **Análise:** Scikit-learn para regressão linear
- **Interface:** Design responsivo

---

## 💻 **Executável Local**

### 🚀 **Sobre a Versão Executável**

Esta versão do sistema foi desenvolvida para funcionar como **aplicação local** através de um executável (.exe), permitindo que o usuário execute o servidor web diretamente em sua máquina e acesse a aplicação através do navegador.

### ⚙️ **Características do Servidor Local**

- **🌐 Acesso via Rede:** O servidor fica disponível na rede local para acesso de outros dispositivos
- **⏰ Finalização Automática:** O processo é encerrado automaticamente a cada **1 hora** para evitar consumo desnecessário de memória
- **💾 Economia de Recursos:** Sistema otimizado para uso doméstico sem impacto no desempenho da máquina
- **🔒 Segurança:** Dados armazenados localmente utilizando sqllite, sem dependência de servidores externos

### 📱 **Como Funciona**

1. **Download:** Baixe o repositorio ou arquivo `.exe` na sua máquina
2. **Execução:** Execute o arquivo `.exe` na sua máquina
3. **Servidor:** O sistema inicia um servidor web local
4. **Acesso Local:** Acesse via navegador usando `http://127.0.0.1:5000`
5. **Acesso na Rede:** Outros dispositivos na mesma rede podem acessar: `http://IP_DA_MAQUINA_HOST:5000`
6. **Finalização:** Após 1 hora, o servidor é encerrado automaticamente

### 🌐 **Acesso na Rede Local**

Para acessar o sistema de outros dispositivos na mesma rede:

#### **📱 A partir de outros dispositivos:**
- **Formato:** `http://IP_DA_MAQUINA_HOST:5000`
- **Exemplo:** `http://192.168.1.100:5000`

#### **🔍 Como descobrir o IP da máquina host:**

1. **Abra o CMD** (Prompt de Comando) na máquina onde o executável está rodando
2. **Digite:** `ipconfig`
3. **Procure por:** "IPv4 Address" ou "Endereço IPv4"
4. **Use esse IP** para acessar de outros dispositivos

#### **💡 Exemplo prático:**
```
C:\> ipconfig
...
Adaptador Ethernet:
   Endereço IPv4. . . . . . . . . . . . . . : 192.168.1.100
...
```
**Acesso:** `http://192.168.1.100:5000`

### 🎯 **Vantagens**

- ✅ **Sem instalação:** Apenas execute o arquivo
- ✅ **Portabilidade:** Funciona em qualquer Windows
- ✅ **Economia:** Não consome recursos desnecessários
- ✅ **Privacidade:** Dados ficam na sua máquina
- ✅ **Rede Local:** Compartilhamento com outros dispositivos

---

## 🔗 **Links Úteis**

- **📂 Repositório:** [GitHub - ExpenseTracker](https://github.com/IgorArodrigues/ExpenseTracker)
- **📄 Licença:** MIT License
- **🐛 Issues:** Reporte bugs e sugestões no GitHub

---


*Desenvolvido com ❤️ para facilitar o controle financeiro pessoal*
