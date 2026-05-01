# 📝 Exercícios Práticos - Módulo 1

### Parte 1: Navegação e Organização
1. Entre na sua pasta pessoal (`/home/usuario`).
2. Crie uma estrutura de pastas: `Projeto/Documentos` e `Projeto/Scripts`.
3. Crie um arquivo vazio chamado `notas.txt` dentro de `Documentos`.

### Parte 2: Edição e Instalação
1. Instale o monitor de sistema `htop` usando o comando: `sudo apt update && sudo apt install htop`.
2. Abra o arquivo `notas.txt` com o editor **Nano**.
3. Escreva seu nome completo e o nome da sua distribuição Linux dentro do arquivo.
4. Salve e saia (`Ctrl+O`, `Enter`, `Ctrl+X`).

### Parte 3: Filtros e Encadeamento
1. Liste todos os arquivos da pasta `/etc`.
2. Agora, use o **pipe** e o **grep** para listar apenas os arquivos dentro de `/etc` que contenham a palavra "conf".
   * *Dica: `ls /etc | grep conf`*
3. Tente rodar o comando `htop` e identifique qual processo está consumindo mais memória.

### Parte 4: Desafio Final
1. Crie um arquivo chamado `lista_servicos.txt`.
2. Use o comando `ls /bin` e redirecione a saída para este arquivo usando o operador `>`.
3. Verifique se o arquivo foi criado corretamente usando o comando `cat`.
