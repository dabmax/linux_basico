# Módulo 2: O Poder do Superusuário e a Orquestração de Dados 🔑

Neste módulo, mergulhamos na segurança do sistema, controle de processos e automação básica.

## 1. Usuários e Grupos
No Linux, a segurança é baseada em quem você é.
* **Root (UID 0):** O superusuário com poderes totais.
* **Usuários Comuns:** Têm acesso limitado à sua própria `/home`.
* **Sudo (SuperUser Do):** Comando que permite usuários autorizados executarem tarefas de admin.

## 2. Permissões de Arquivos (rwx)
Cada arquivo ou diretório tem três tipos de permissões para três tipos de pessoas:

| Permissão | Letra | Valor | O que faz? |
| :--- | :---: | :---: | :--- |
| **Read** | `r` | 4 | Lê o conteúdo |
| **Write** | `w` | 2 | Altera o conteúdo |
| **Execute** | `x` | 1 | Roda o arquivo como programa |



**Exemplo de cálculo:** `chmod 755 script.sh`
* **7 (4+2+1):** Dono faz tudo.
* **5 (4+0+1):** Grupo lê e executa.
* **5 (4+0+1):** Outros lêem e executam.

## 3. Comandos de Sistema e Processos
* `ps aux`: Lista todos os processos rodando no sistema.
* `kill -9 <PID>`: Encerra um processo à força.
* `top` ou `htop`: Monitoramento em tempo real (vimos o htop no módulo 1).
* `chown`: Altera o dono do arquivo (`sudo chown usuario:grupo arquivo`).

## 4. Manipulação Avançada de Texto
* `cat`: Exibe o arquivo inteiro.
* `head` / `tail`: Mostra o início ou o fim de um arquivo.
* `tail -f`: Monitora um arquivo de log conforme ele cresce (essencial para troubleshoot).

## 5. Introdução ao Shell Scripting
Um script é uma sequência de comandos salva em um arquivo. Deve começar com o **Shebang**:
```bash
#!/bin/bash
echo "Iniciando verificação..."
df -h # Mostra espaço em disco