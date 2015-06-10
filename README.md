# Estudos de Git e GitHub
##Comandos Iniciais

###Se identificando
1. ```git config --global user.name "Danilo Marinho"```
2. ```git config --global user.email dannilodms@gmail.com```

###Comandos Iniciais 
1. ```git init``` > Incializa repositório
2. ```git status``` > Ver a situação do repositório
3. ```git add 'nome_do_arquivo ou * para todos os arquivos'``` > coloca o arquivo na área de stage para que possa ser comitado
4. ```git commit -m "Mensagem sobre o commit"``` > grava os arquivos que estão na área de stage no repositório
3. ```git log``` > verfica o histórico das alterações gravadas

###Iniciando com GitHub
1. ```git remote add origin 'endereço do repositório'``` > referecia o repositório do GitHub como o de origem
2. ```git push origin master``` > envia as alerações para o repositório do GitHub
3. ```git clone 'endereço do repositório'``` > clona um repositório do GitHub

###Trabalhando com repositórios locais
1. ```git add 'subDiretorio .' ``` > coloca somentes os arquivos do subdiretorio informado na área de stage
2. criar arquivo .gitignore, cada linha é o nome de um arquivo a ser ignorado, ex: todo.txt ou *log (ignora tudo com termina com log) > indica os arquivos a serem ignorados pelo Git
3. ```git commit -am "Mensagem do commit"``` > adiciona à área de stage e comita ao mesmo tempo, obs: não funciona com arquivos novos
3. ```git log -n 'n'``` > mostra apenas o 'n' ultimos commits
4. ```git log --oneline``` > melhor visualização do historico de commits
5. ```git log --stat``` > mostra resumo dos arquivos alterados
6. pode ser usar os três ultimos comandos combinados, ex: ```git log -n 2 --oneline --stat
7. ```git diff 'opcianal: nome do arquivo'``` > mostra as mudanças ainda não adicionadas à área de stage nos arquivos já existentes alterados
8. ```git diff --staged``` > mostra diferenças entres arquivos na área de stage e a última versão comitada
9. ```git diff 'codigo do commit'``` > mostra alterações dentro e fora do stage
10. ```git diff 'codigo do commit inicial..final'``` > mostra as alterações realizadas entre o commit inicial e final passados
11. ```git diff 'codigo do commit~n``` > mostra mudanças em relação aos 'n' commits anteriores.
12. ```git rm 'arquivo'``` > mesmo funcionamento do add porém para remoção de arquivos
13. ```git mv 'nome atual' 'nome desejado'``` > renomeia um arquivo obs: mesmo comando do linux
14. ```git mv 'arquivo' 'subDir/arquivo'``` > move o arquivo obs: mesmo comando do linux
15. ```git checkout -- 'arquivo' > desfaz as alterações que não estão na área de stage no arquivo
16. ```git reset -- 'arquivo' ou sem paremetros``` > remove os arquivo passados como parametro da área de stage, ou de todos os arquivos casa não tenha paramentros
17. ```git reset --hard``` > remove os arquivos da área de stage e desfaz as mudanças feitas nesses arquivos
18. ```git revert --no-edit 'codigo do commit'``` > volta o repositorio para o commit correspondente ao codigo. obs: se omitir --no-edit sera solicitado nova mesagem do commit
19. ```git reset --hard 'codigo do commit'``` > semelhante ao revert porém apaga todos os commit posteriores ao commit passado. Não recomendado se quiser manter o historico do codigo

