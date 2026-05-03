# 🔐 Brute Force Lab com Kali Linux e Medusa

## 📌 Visão Geral

Este projeto foi desenvolvido como parte dos meus estudos em cibersegurança, com foco na prática de ataques de força bruta em um ambiente controlado.

Utilizando Kali Linux como máquina atacante e Metasploitable 2 como alvo vulnerável, o laboratório simula cenários reais de falhas de autenticação em serviços comuns.

---

## 🎯 Objetivos

* Compreender como ataques de força bruta funcionam na prática
* Identificar vulnerabilidades em serviços de autenticação
* Simular ataques em diferentes protocolos (FTP, Web e SMB)
* Aplicar conceitos de segurança ofensiva e defensiva
* Documentar o processo de forma clara

---

## 🖥️ Ambiente de Laboratório

* **Atacante:** Kali Linux
* **Alvo:** Metasploitable 2
* **Virtualização:** VirtualBox
* **Rede:** Host-only (isolada)

### 🌐 Comunicação

* Kali Linux: 192.168.56.101
* Metasploitable 2: 192.168.56.102

A comunicação entre as máquinas foi validada com sucesso, permitindo a execução dos testes em ambiente controlado.

---

## 🔎 Reconhecimento

Foi realizada uma etapa inicial de enumeração para identificar serviços ativos no alvo.

### Serviços identificados:

* FTP (porta 21)
* HTTP (porta 80)
* SMB (porta 445)

Esses serviços são conhecidos por serem alvos comuns de ataques de autenticação.

---

## 🔐 Conceitos Aplicados

### ✔️ Força Bruta

Tentativa de múltiplas combinações de usuário e senha até encontrar uma válida.

### ✔️ Password Spraying

Aplicação de uma senha comum em vários usuários para evitar bloqueios rápidos.

### ✔️ Ataques em aplicações web

Exploração de formulários de login sem proteção contra múltiplas tentativas.

---

## ⚔️ Simulações Realizadas

### 📁 FTP

Foram realizados testes de autenticação utilizando combinações simples de credenciais.

**Resultado:**
Foi possível observar que o serviço não possui limitação de tentativas, tornando-o vulnerável a ataques de força bruta.

---

### 🌐 Aplicação Web (DVWA)

Simulação de múltiplas tentativas de login em um formulário web vulnerável.

**Resultado:**
A aplicação não apresentou mecanismos de proteção como bloqueio por tentativa ou CAPTCHA.

---

### 🖥️ SMB

Teste utilizando técnica de password spraying em múltiplos usuários.

**Resultado:**
Foi possível observar o risco associado ao uso de senhas fracas e reutilizadas.

---

## 📂 Wordlists Utilizadas

### Usuários

```id="u1a9sx"
admin
user
test
root
msfadmin
```

### Senhas

```id="p8k3zm"
123456
password
admin
123123
msfadmin
```

Essas listas foram utilizadas para demonstrar como credenciais simples ainda representam uma falha crítica de segurança.

---

## 🚨 Vulnerabilidades Identificadas

* Uso de senhas fracas
* Ausência de bloqueio após múltiplas tentativas
* Falta de monitoramento de autenticação
* Serviços expostos sem proteção adicional

---

## 🛡️ Medidas de Mitigação

### 🔒 Autenticação

* Implementação de MFA
* Uso de senhas fortes

### ⛔ Proteção

* Limitação de tentativas de login
* Bloqueio temporário após falhas consecutivas

### 👁️ Monitoramento

* Registro de logs
* Alertas de atividades suspeitas

### ⚙️ Configuração

* Desativação de serviços desnecessários
* Restrição de acesso por rede

---

## 📚 Aprendizados

Este laboratório reforça como vulnerabilidades simples ainda são amplamente exploráveis em ambientes mal configurados.

A prática demonstrou que ataques básicos podem ser eficazes quando não há medidas de proteção adequadas.

---

## ⚠️ Considerações Éticas

Todos os testes foram realizados exclusivamente em ambiente controlado, com finalidade educacional.

---

## 🚀 Conclusão

O projeto demonstrou, na prática, como falhas de autenticação podem comprometer sistemas.

A aplicação de boas práticas de segurança é essencial para reduzir significativamente esses riscos.

---

## 🔗 Autor

Projeto desenvolvido por Emanuel Victor Lima dos Santos como parte dos estudos em Cibersegurança.
