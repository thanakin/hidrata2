# Hidrata
"Lembrete" para beber água regularmente.

## Motivo
Beber agua é uma necessidade, porem a correria do dia a dia acaba por atropelar esta carência em alguns casos.

Como o home office se tornou algo frequente, o uso do computador para tal ainda mais... então ele bem que poderia "me lembrar" quando eu esquecer, não é mesmo? Para isso pensei no Hidrata!
O nome pode não ser muito bom, mas representa bem a ideia.

## Opções
Aplicativos moveis existem aos punhados com este mesmo proposito, acredito que até mesmo para computadores, em lojas de app ou originários de terceiros.

Confesso que não cheguei a procurar, pois queria algo mais simples e que funcionasse basicamente com o que tenho no computador.

## Testes
Realizei testes e esta em funcionamento atualmente com:   
Windows 10 Home Single Language versão 21H1, desde 24/04/2020;   
Ubuntu 20.10 com Gnome 3.38.3, desde 21/07/2021.   

## Requerimentos
Nos sistemas testados, tenho usuário com permissões elevadas (admin e sudo, respectivamente).
No momento atual (agosto/2021) é necessário ao menos 1 arquivo em cada sistema para o funcionamento, mais detalhes a seguir em cada um.

**Observação**: acredito que possam existir maneiras ainda mais simples ou mais requintadas de atingir este mesmo objetivo, porem no momento, me atende satisfatoriamente. Não descarto atualizar este repo num futuro, pois ja é uma segunda versão...

## Windows
Utilizarei o Agendador de Tarefas, que de acordo com o(s) horário(s) estabelecido(s), executara um arquivo Html simples com a frase "Beber água!". Não testei de outras formas ou arquivos.   

* Tecle iniciar e depois digite "tarefas" ou "agendador de tarefas".
* Na tela que sera aberta, clique em "Biblioteca do Agendador" e depois em "Criar Tarefa...".
* Na tela seguinte estará na aba "Geral", preencha o campo nome com valor pertinente.
* Clique na aba "Disparadores" e em "Novo".
* Sera aberta uma terceira janela onde pode definir a frequência das notificações.   
* No meu caso, tenho dois agendamentos: um iniciando as 07:30 e outro as 08:00, ambos configurados para o modo Semanal a cada 1 semana, sendo segunda, terça, quarta, quinta e sexta, repetindo a tarefa a cada 1 hora. Desta forma, enquanto meu computador de trabalho estiver ligado, chamara o arquivo especificado a seguir.
* Ao termino da configuração do disparador, clique em ok e então na aba Ações e depois em Novo.
* Utilizei a opção Iniciar um programa e em Programa/script, indiquei o arquivo html que uso.
* Feito isso, clique em Ok. Poderá ver opções adicionais nas demais abas, porem os ajustes citados aqui já são suficientes, podendo clicar em Ok uma ultima vez.
* Feche o agendador e aguarde a execução nos horários definidos.


## Linux
Utilizarei o Cron, que executara um script Python responsável por emitir uma notificação do sistema.


