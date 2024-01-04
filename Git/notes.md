# Como retornar para um commit antigo?
É simples! É só usar o comando "git reset"!
Mas cuidado! Existem algumas maneiras de fazer esse reset,
dependendo do nível de confusão do código! Estas são elas:

1. soft: Reseta tudo, mas deixa os arquivos futuros em **STAGED**;
2. mixed: Reseta tudo, mas deixa os arquivos futuros em **UNTRACKED**;
3. hard: Reseta TUDO, deleta TUDO! Quando o nível de caos do código chegou ao máximo;

Tô testando os três modos.

# Comandos úteis importantes
Alguns comandos que podem me salvar no trabalho!

1. git fetch: Pega as alterações feitas no branch remoto! É diferente do git pull que pega e faz um merge
com o nosso branch;
2. git stash: Tá ocupado resolvendo um problema numa branch e um bug apareceu em outro? O git stash salva todas as alterações
feitas na branch atual **SEM COMMITTAR**. Isso te deixa livre para ir para outra branch!

## Sobre o git stash
Existem dois modos de usar o **stash**. O **APPLY** e o **POP**. O primeiro
aplica as alterações no branch atual e ainda as deixa guardadas. No segundo,
as alterações saem do stash e são aplicadas. Podemos criar um stash em uma
determinada branch **X** e usar em outra branch **Y**!
