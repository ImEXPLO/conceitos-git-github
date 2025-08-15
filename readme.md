# Conceitos de Git e Github
Este arquivo tem como objetivo armazenar os comandos básicos para utilização de git e GitHub

## Configuração Inicial 
Rode os comandos abaixo no terminal (CMD ou GitBash) do seu computador.
```bash
git config --global user.name <Nome do Utilizador>
```

```bash
git config --global user.email <Email do Utilizador (sem aspas)>
```

## Exemplo ##
```bash
git config --global user.name "Victor Hugo Silva"
```

```bash
git config --global user.email victor.silva312@fatec.sp.gov.br
```

## Comandos do Git
Para iniciar o GIT em uma pasta de computador utilizamos o init.
**IMPORTANTE:** Só é executado uma vez
**IMPORTANTE:** Isso vale pra uma grande maioria dos comandos, se não apareceu nada na hora que você digitou o comando, é por que deu certo!

```bash
git init
```

Para vincular o projeto ao GitHub utilizamos o comando remote, basta o repositório estar criado no GitHub e seguir a segunda opção da lista de comandos que aparece no site.<br>
**IMPORTANTE:** Depois do remote deve ser executados os outros 2 comandos da página.

```bash
git remote add origin < url_repositorio_github >
```

Para verificar a situação do repositório (pasta) usamos o status a qualquer momento

```bash
git status
```

Após isso, você pode utilizar no seu terminal um comando para abrir o Visual Code naquela pasta

```bash
code .
```

Agora ele irá abrir o Visual Code. Você pode criar um readme.md, ou seja, um Leia-me para o seu repositório GIT, igual a esse que estamos criando. Logo após criar esse read-me (ou upar algum arquivo seu pronto, tanto faz), usaremos outro comando do git para poder dizer pro GitHub que queremos que aquele arquivo seja incluso na nuvem, ele é o:

```bash
git add .
```
**Ele serve para salvar o estado do arquivo pra ser salvo na nuvem.**

Antes de commitar, podemos rodar o **git status** novamente pra vermos se tem algum arquivo faltante, caso sim, ele aparecerá em Vermelho, se aparecer algum, use o comando do **git add .**

Vamos agora commitar, ou seja, preparar o nosso arquivo pra ser salvo na nuvem, e usamos outro comando do git que é;

```bash
git commit -m "Teste de Mensagem" 
```
o "-m" no comando do "git commit" é **usado para demonstrarmos uma mensagem nesse commit**, então, ele serviria para a gente lembrar do que foi feito a alteração, para que se **caso você não se lembre do que se trata o seu commit, ele será um lembrete.**

Para baixar as alterações que estão **apenas** no GitHub utilizamos o pull. <br>
**IMPORTANTE**: Sempre deve baixar a última versão da nuvem antes de enviar a atual do computador
```bash
git pull
```

Para enviar as alterações (Os commits) do PC para o GitHub utilizamos o push. <br>
**IMPORTANTE**: Sempre deve baixar a última versão da nuvem antes de enviar a atual do computador
```bash
git push
```
