# conky-mint-pt

Configuração do Conky para o Linux Mint em português.
Um tema para o Conky com suporte meteorológico do Yahoo! (em inglês), mais uma variedade de funções, todas elas traduzidas para português: data e hora, info de sistema, discos, memória, processos, etc.

# INSTALAÇÂO:

- Copie ou extraia a pasta “conky_mint_pt” (“conky-google-now”, “fontes”, “logos” e os ficheiros “conkyrc” e “conky-startup.sh”)  para a pasta “~/.conky”. Se esta não existir, crie-a (~/.conky/conky_mint_pt/).

- Crie uma pasta em “~/.cache/” com o nome conky, nesta pasta ficarão os ficheiros temporários relacionados com a meteorologia (~/.cache/conky).

- Instale as fontes Play da pasta “fontes”, por exemplo a partir de um visualizador de fontes tal como o gnome-font-viewer( instale este pelo terminal $ sudo apt-get install gnome-font-viewer).

- Faça o script “conky-startup,sh” arrancar no inicio do sistema.
Aceda a Definições>Sessão e arranque>Aplicações automáticas>Adicionar>Nome = Conky e Comando = sh ~/.conky/conky_mint_pt/conky-startup.sh .

E pronto, espero que gostem!

Nota: Esta configuração foi optimizada para uma resolução de ecrã de 1280x800, para outras resoluções terão que ser feitas alterações no ficheiro conkyrc.
Relativamente as partições do disco, este ficheiro está configurado para a existência de uma partição /HOME separada da /ROOT, se o seu sistema não tiver essa separação, pode comentar ou eliminar essa linha referente a partição /HOME.

