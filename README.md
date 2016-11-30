# meuconky

Configuração do Conky para o Linux Mint em português.
Um tema para o Conky com uma barra informativa com uma variedade de funções, todas elas traduzidas para português: data e hora, info de sistema, discos, memória, processos, etc. Contém ainda um calendário e suporte meteorológico do Yahoo! (em inglês). 

# INSTALAÇÃO:

- Copie ou extraia a pasta “conky-mint-pt-meuconky” (“conky-google-now”, “fontes”, “logos” e os ficheiros “infobar” "cal13meses"  "yahoometeo" e “conky-startup.sh”)  para a pasta “~/.conky”. Se esta não existir, crie-a "~/.conky/meuconky/".

- Crie uma pasta em “~/.cache/” com o nome conky, nesta pasta ficarão os ficheiros temporários relacionados com a meteorologia (~/.cache/conky).

- Personalize a sua localização no ficheiro yahoometeo, substitua a palavra "localização" na linha 88 pelo nome da sua cidade em inglês. (exemplos que funcionam: “Setubal” ou “Lisbon”.)

- Instale as fontes Play da pasta “fontes”, por exemplo a partir de um visualizador de fontes tal como o gnome-font-viewer( instale este pelo terminal $ sudo apt-get install gnome-font-viewer).

- Faça o script “conky-startup.sh” arrancar no inicio do sistema.
Aceda a Definições>Sessão e arranque>Aplicações automáticas>Adicionar>Nome = Conky e Comando = sh ~/.conky/meuconky/conky-startup.sh . O calendário e a previsão do tempo estão desactivados, para activar basta descomentar as respectivas linhas no ficheiro conky-startup.sh .
E pronto, espero que gostem!

Nota: Esta configuração foi optimizada para uma resolução de ecrã de 1280x800 e definições personalizadas das fontes em 96 PPP, para outras resoluções terão que ser feitas alterações nos ficheiros infobar, cal13meses e yahoometeo.
Relativamente as partições do disco, este ficheiro está configurado para a existência de uma partição /HOME separada da /ROOT, se o seu sistema não tiver essa separação, pode comentar ou eliminar essa linha referente à partição /HOME.
A configuração está igualmente optimizada para processadores de 4 núcleos, se o seu não tiver 4 núcleos terá OBRIGATÓRIAMENTE que apagar, ou acrescentar as respectivas linhas de configuração dos CPU no ficheiro infobar, de acordo com o seu modelo.
Quando à placa gráfica, o ficheiro infobar contém linhas de código exclusivas para serem usadas em placas Nvidia.
