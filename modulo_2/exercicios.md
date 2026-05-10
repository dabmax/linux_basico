### 2. `modulo 2/exercicio.md`
Desafios práticos para fixar o conhecimento.

```markdown
# 📑 Exercícios de Fixação - Módulo 2

### Desafio 1: Gestão de Usuários
1. Crie um novo usuário chamado `dev_user`.
2. Adicione esse usuário ao grupo `sudo`.
3. Mude para esse usuário usando `su - dev_user` e tente criar um arquivo dentro de `/root`.

### Desafio 2: Permissões Octais
1. Crie um arquivo chamado `confidencial.txt`.
2. Configure as permissões para que:
   - Você (Dono) possa ler e escrever.
   - O Grupo possa apenas ler.
   - Outros não tenham **nenhum** acesso.
3. Use `ls -l` para validar se ficou `-rw-r-----`.

### Desafio 3: Caça ao Processo
1. Abra o editor `nano` em um terminal e deixe-o aberto.
2. Em outro terminal, use `ps aux | grep nano` para achar o número do processo (PID).
3. Use o comando `kill` para fechar o nano remotamente.

### Desafio 4: Meu Primeiro Script
1. Crie um arquivo chamado `backup_logs.sh`.
2. O script deve:
   - Criar uma pasta chamada `backup` na sua home.
   - Copiar todos os arquivos `.log` de `/var/log` para essa nova pasta.
   - Exibir a mensagem "Backup concluído!".
3. Torne-o executável e execute-o.