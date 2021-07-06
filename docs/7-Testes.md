# Avaliação da Aplicação

O processo de realização dos testes da solução desenvolvida está documentado 
na seção que se segue e traz os planos de testes de software e de usabilidade e,
na sequência, o registro dos testes realizados. 

## Plano de Testes de Software

#### `Objetivos`
Este segmento tem como objetivo listar os requisitos que serão testados no 
protótipo Rotten Info, recomendando e descrevendo as estratégias a serem
empregadas nesses testes.  

#### `Casos`

Caso de Teste | CT-01 – Visualizar avaliação dos sites  
------------- | -------------------------------------- 
Requisitos Associados | RF- 01- O site deve apresentar a avaliação de cada site, a fim de demonstrar a sua “credibilidade”.
... | RF-02- O site deve apresentar, para cada site, uma coloração própria que correspondente a segurança da informação.  
Objetivo do Teste | Verificar se os sites estão tendo suas avaliações mostradas de maneira eficaz. 
Passos | 1) Acessar o Navegador / 2) Informar o endereço do Site / 3) Visualizar a página principal / 4) Clicar em um site que deseja saber mais sobre / 5) Observar thumnails pela página que indicam avaliação e/ou coloração dessa.  
Critérios de Êxito | A página deve apresentar um índice de crebilidade e/ou um thumbnail na cor verde se confiável e vermelha se não confiável. 

Caso de Teste | CT-02 – Visualizar avaliação por Rating 
------------- | -------------------------------------- 
Requisitos Associados | RF-07- O site deve exibir as avaliações registradas juntamente com "rating” do site e, também, apresentar uma ferramenta de avaliação. 
Objetivo do Teste | Verificar se sites específicos estão tendo suas avaliações mostradas por rating e/ou categoria. 
Passos | 1) Acessar o Navegador / 2) Informar o endereço do Site / 3) Visualizar a página principal / 4) Buscar por Raking na página principal / 5) Observar topdown pela página que indicam avaliação  
Critérios de Êxito | A página deve apresentar um raking mostrando os sites mais confiáveis e a opção de percorrer através de categorias de avaliações. 

Caso de Teste | CT-03 – Visualizar por sites salvos 
------------- | -------------------------------------- 
Requisitos Associados | RF-6 -- O site deve permitir verificar sites salvos como preferidos 
Objetivo do Teste | Verificar se os sites marcados como “salvos” estão sendo exibidos separadamente 
Passos | 1) Acessar o Navegador / 2) Informar o endereço do Site / 3) Visualizar a página principal / 4) Acessar a aba “Buscas” e marcar algum site como favorito. / 5) Acessar a aba “Favoritos” e verificar se os sites marcados como “salvos” estão lá.
Critérios de Êxito | A página “Favoritos” deve apresentar apenas os sites salvos. 


Caso de Teste | CT-04 – Bloqueio de sites não confiáveis 
------------- | -------------------------------------- 
Requisitos Associados | RF-05- O site deve oferecer uma funcionalidade de filtro/pesquisa para permitir ao usuário bloquear conteúdos de baixa avaliação. 
Objetivo do Teste | Verificar se os filtros que detectam baixas avaliações estão funcionais.  
Passos | 1) Acessar o Navegador / 2) Informar o endereço do Site / 3) Visualizar a página principal / 4) Procurar por button que permite a opção de bloqueio de conteúdo não confiável. 
Critérios de Êxito | A página deve apresentar a opção de filtro e bloqueio de páginas indesejadas. 


Caso de Teste | CT-05 – Compartilhamento de avaliações em redes sociais 
------------- | -------------------------------------- 
Requisitos Associados | RF-04- O site deve permitir o compartilhamento de avaliações de sites em plataformas de redes sociais 
Objetivo do Teste | Verificar se a página permite o compartilhamento de avaliações em redes sociais através de geração de links.  
Passos | 1) Acessar o Navegador / 2) Informar o endereço do Site / 3) Visualizar a página principal / 4) Procurar por categoria de avaliados e através disso, verificar se está funcional a opção de compartilhamento.  
Critérios de Êxito | A página deve apresentar formas de compartilhar as avaliações em meios fora do próprio site. 


Caso de Teste | CT-06- Compatibilidade de Navegador 
------------- | -------------------------------------- 
Requisitos Associados | RNF-03- O site deve ser compatível com os principais navegadores do mercado (Google Chrome, Firefox, Microsoft Edge, Opera GX) 
Objetivo do Teste | Testar se o sistema desenvolvido é compatível com os navegadores solicitados. 
Passos | 1) Acessar os navegadores desejados / 2) Verificar se há compatibilidade, podendo ser usado a ferramenta MochaJS como auxílio. 
Critérios de Êxito |A página deve apresentar compatibilidade com os navegadores anteriormente citados. 

Caso de Teste | CT-07- Disponibilidade do site na Internet 
------------- | -------------------------------------- 
Requisitos Associados | RNF-01- O site deve ser publicado em um ambiente acessível publicamente na Internet (Repl.it, GitHub Pages, Heroku); 
Objetivo do Teste | Verificar se o site foi publicado em algum ambiente de hospedagem.  
Passos | 1) Acessar ambientes de hospedagem anteriormente citados 2) Verificar a disponibilidade da página.  
Critérios de Êxito | A página deve apresentar hospedagem na Internet. 

Caso de Teste | CT-08- Contraste entre os elementos 
------------------- | ---------------------------------
Requisitos Associados | RNF-02- O site deve ter bom nível de contraste entre os elementos da tela em conformidade 
Objetivo do Teste | Verificar se o site tem um bom contraste entre os elementos que o compõe, fazendo com que seja facilmente identificado certas coisas. 
Passos | 1) Abrir a tela inicial do site e analizar o contraste dos elementos. / 2) Abrir a tela de buscas e analizar o contraste dos elementos. 
Critérios de Êxito | Cores significativas para certas características de elementos da página. Ex: Site não confiável sinalizado com a cor vermelha, site confiável com a cor verde. 

### `Avaliação`

Registro de teste 1 | (Visualizar avaliação dos sites) 
------------------- | ---------------------------------
RF-1 / RF-2 | Itens a serem observados de acordo com os critérios de êxito. 
Resultado | Exito
Observação | Nada a relatar
 
Registro de teste 2 | (Visualizar avaliação por Rating ou Categoria) 
------------------- | ---------------------------------
RF-7 | Apenas sites com boas avaliações são mostrados e possibilidade de avaliar o site.
Resultado | Exito
Observação | Nada a relatar

Registro de teste 3 | (Visualizar por sites salvos) 
------------------- | ---------------------------------
RF-6 | Função de filtro de sites salvos, prints ilustrativos dos resultados: 
Resultado | Exito
Observação | Nada a relatar

Registro de teste 4 | (Bloqueio de site não confiáveis) 
------------------- | ---------------------------------
RF-5 | Bloqueia conteúdos de baixa avaliação, mostra apenas os com avaliação “Boa” 
Resultado | Exito
Observação | Nada a relatar
 
Registro de teste 5 | (Compartilhamento de av. em redes socais) 
 ------------------- | ---------------------------------
RF-4 | Função de compartilhamento em redes sociais. 
Resultado | Falha
Observação | Implementar um botão facilmente visível para o compartilhamento das notícias em redes sociais 

Registro de teste 6 | (Compatibilidade com navegador) 
 ------------------- | ---------------------------------
RNF-3 | Compatibilidade com os principais navegadores disponíveis no mercado: 
Resultado | Exito
Observação | Testado em Firefox, Chrome, Edge e Opera GX. 

Registro de teste 7 | (Disponibilidade do site na Internet) 
 ------------------- | ---------------------------------
RNF-1 | Site publicado em ambiente disponível para o público na Internet. 
Resultado | Exito
Observação | Nada a relatar

Registro de teste 8 | (Contrasto entre os elementos) 
 ------------------- | ---------------------------------
RNF-2 | Bom nível de contraste entre os elementos presentes no site. 
Resultado | Exito
Observação | Botão de “gostei” e sites bem avaliados de coloração verde, botão “não gostei” e sites mal avaliados com coloração vermelha. Sites neutros com coloração amarela. 

## Plano de Testes de Usabilidade

#### `Objetivos`
Esses testes têm como objetivo principal garantir que o protótipo esteja
de fácil acesso, visualização e navegação pelo usuário. Além disso, é 
necessário que as informações estejam facilmente legíveis e compreensíveis, 
garantindo, portanto, uma interface intuitiva. Ao realizar os testes nessa 
etapa, a equipe obterá informações de extrema utilidade acerca do projeto 
de forma crítica, considerando os testes a serem feitos. Ou seja, os 
objetivos podem ser descritos como: 
 - Garantir que o protótipo esteja intuitivo; 
 - Compreender a decisão dos usuários e suas determinadas ações; 
 - Avaliar a satisfação dos usuários em relação ao protótipo; 
 - Utilizar o feedback para melhorar os aspectos necessários; 

#### `Casos`


Tarefa de usuário | TU-01 - Entrar no site 
 ---------------- | -----------------------
Objetivo do Teste | Observar se o usuário consegue acessar corretamente o protótipo. 
Passos | 0) Computador ligado e visualizando a área de trabalho, arquivo txt aberto com o link para o site; / 1) Abrir o browser escolhido (Chrome, GX, Edge, Firefox, etc.); / 2) Copiar e colar o link no browser; / 3) Esperar o site carregar. 
Critérios de Êxito | O usuário deve acessar o site com facilidade; / O site deve carregar em torno de 5 segundos; 


Tarefa de usuário | TU-02 – Explorar o site 
 ---------------- | -----------------------
 Objetivo do Teste | Familiarizar o usuário em relação ao site para as próximas tarefas, assim como identificar se os elementos principais são facilmente encontrados. 
Passos | 0) Site devidamente aberto na página principal, pronto para navegação. / 1) Observar a página principal (também chamada de “Home”) completa; /2) Identificar pontos chaves do site, tal como: Logo , Menu de opções , Sites destacados; /3) Sinalizar o avaliador quando se sentir familiarizado com a página principal. 
Critérios de Êxito | O protótipo deve estar funcionando como esperado; / O participante deve sinalizar em menos de 2 minutos, aproximadamente. 


Tarefa de usuário | TU-03 – Sites em Destaque 
 ---------------- | -----------------------
Objetivo do Teste | Observar se o design permite aos usuários fácil identificação dos destaques, avaliando se a escolha é intuitiva. 
Passos | 0) Site devidamente aberto na página principal, pronto para navegação (TU-02). / 1) Clique no site em 1º lugar nos destaques; / 2) Retornar a página principal do protótipo; / 3) Clicar no site em 2º lugar nos destaques; / 4) Retornar a página principal do protótipo; / 5) Clicar no site em 3º lugar nos destaques; 
Critérios de Êxito | O participante deve ser capaz de discernir qual a posição do site; / O participante dever suceder no acesso aos 3 sites; 


Tarefa de usuário | TU-04 – Alterar para categoria Acadêmico 
 ---------------- | -----------------------
Objetivo do Teste | Observar se a alteração de categoria é intuitiva e user friendly para a categoria acadêmica. 
Passos | 0) Site devidamente aberto na página principal, pronto para navegação (TU-02). / 1) Encontrar a alteração de categorias; / 2) Alterar para a categoria "Acadêmico”; / 3) Escolher o primeiro site da categoria e clicar; / 4) Retornar à página principal do protótipo; 
Critérios de Êxito | O participante deve ser capaz de encontrar onde alterar a categoria de forma rápida; /A categoria deve ser corretamente selecionada; / A mudança dos sites de determinada categoria deve ser feita em menos de 2 segundos; / O participante deve sinalizar ao avaliador em menos de 3 minutos, aproximadamente. 


Tarefa de usuário | TU-05 – Alterar para categoria Política
 ---------------- | -----------------------
Objetivo do Teste |Observar se a alteração de categoria é intuitiva e user friendly para a categoria política. 
Passos | 0) Site devidamente aberto na página principal, pronto para navegação (TU-02). / 1) Encontrar a alteração de categorias; / 2) Alterar para a categoria "Política”; / 3) Escolher o primeiro site da categoria e clicar; / 4) Retornar à página principal do protótipo; 
Critérios de Êxito | O participante deve ser capaz de encontrar onde alterar a categoria de forma rápida; / A categoria deve ser corretamente selecionada; / A mudança dos sites de determinada categoria deve ser feita em menos de 2 segundos; / O participante deve sinalizar ao avaliador em menos de 3 minutos, aproximadamente. 


Tarefa de usuário | TU-06 – Alterar para categoria Esportes 
 ---------------- | -----------------------
Objetivo do Teste | Observar se a alteração de categoria é intuitiva e user friendly para a categoria esportiva. 
Passos | 0) Site devidamente aberto na página principal, pronto para navegação (TU-02). / 1) Encontrar a alteração de categorias; / 2) Alterar para a categoria "Esportes”; / 3) Escolher o primeiro site da categoria e clicar; / 4) Retornar à página principal do protótipo; 
Critérios de Êxito | O participante deve ser capaz de encontrar onde alterar a categoria de forma rápida; / A categoria deve ser corretamente selecionada; / A mudança dos sites de determinada categoria deve ser feita em menos de 2 segundos; / O participante deve sinalizar ao avaliador em menos de 3 minutos, aproximadamente. 


Tarefa de usuário | TU-07 – Busca de determinado site 
 ---------------- | -----------------------
Objetivo do Teste | Determinar se o sistema de busca é facilmente acessível e também intuitivo. 
Passos | 0) Site devidamente aberto na página principal, pronto para navegação (TU-02). / 1) Clicar no menu “Busca”; / 2) Digitar o site escolhido pelo avaliador; / 3) Clicar no site desejado; / 4) Retornar a página principal do protótipo. 
Critérios de Êxito | O participante deve ser capaz de encontrar a opção de “busca”, relatando poucas dúvidas durante o processo; / O site desejado deve aparecer como opção principal; / O participante deve sinalizar ao avaliador em menos de 2 minutos, aproximadamente. 


Tarefa de usuário | TU-08 – Avaliação positiva de um site 
 ---------------- | -----------------------
Objetivo do Teste | Observar se o processo de avaliar positivamente um site é intuitivo para os usuários. 
Passos | 0) Site devidamente aberto na página principal, pronto para navegação (TU-02). / 1) Clicar em um dos sites destacados; / 2) Avalia-lo positivamente com qualquer um dos motivos; / 3) Retornar à página principal; / 4) Clicar novamente no site escolhido no passo 1; / 5) Alterar a avaliação positiva para outro motivo; 
Critérios de Êxito | O participante deve ser capaz de encontrar a opção de “avaliar positivamente”, relatando poucas dúvidas durante o processo; / O participante deve adequadamente avaliar e reavaliar o site escolhido; / O participante deve sinalizar ao avaliador em menos de 3 minutos, aproximadamente. 


Tarefa de usuário | TU-09 – Avaliação negativa de um site 
 ---------------- | -----------------------
Objetivo do Teste |Observar se o processo de avaliar negativamente um site é intuitivo para os usuários. 
Passos | 0) Site devidamente aberto na página principal, pronto para navegação (TU-02). / 1) Clicar em um dos sites destacados; / 2) Avalia-lo negativamente com qualquer um dos motivos; / 3) Retornar à página principal; / 4) Clicar novamente no site escolhido no passo 1; / 5) Alterar a avaliação negativa para outro motivo; 
Critérios de Êxito | O participante deve ser capaz de encontrar a opção de “avaliar negativamente”, relatando poucas dúvidas durante o processo; / O participante deve adequadamente avaliar e reavaliar o site escolhido; / O participante deve sinalizar ao avaliador em menos de 3 minutos, aproximadamente. 


Tarefa de usuário | TU-10 – Selecionar um site como favorito 
 ---------------- | -----------------------
Objetivo do Teste | Compreender se a função “favoritos” é fácil de encontrar, compreender e utilizar. 
Passos | 0) Site devidamente aberto na página principal, pronto para navegação (TU-02). / 1) Clicar em um dos sites destacados; / 2) Marca-lo como favorito; / 3) Retornar à página principal; / 4) Selecionar outro site destacado; / 5) Marca-lo como favorito; / 6) Retornar à página principal; 
Critérios de Êxito | O participante deve ser capaz de encontrar a opção de “favorito”, relatando poucas dúvidas durante o processo; / O participante deve adequadamente marcar os sites escolhidos como favoritos; / O participante deve sinalizar ao avaliador em menos de 3 minutos, aproximadamente. 


Tarefa de usuário | TU-11 – Retirar um site dos favoritos 
 ---------------- | -----------------------
Objetivo do Teste | Observar a intuitividade da ação de retirar um site no menu “Favoritos”. 
Passos | 0) Site devidamente aberto na página principal, pronto para navegação (TU-02). / 1) Clicar no menu “Favoritos”; / 2) Clicar em um dos sites marcados; / 3) Retirar a marcação de favorito; / 4) Retornar à página principal; 
Critérios de Êxito | O participante deve ser capaz de encontrar acessar o menu “Favorito”, relatando poucas dúvidas durante o processo; / O participante deve adequadamente retirar a marca de favoritos dos sites escolhidos; / O participante deve sinalizar ao avaliador em menos de 3 minutos, aproximadamente. 

### `Avaliação`

Usuário 1 | Fernando 
--------- | --------------
Informações do usuário | 18 anos / Estudante / Acessa regularmente a Web 
Relatório | O usuário conseguiu concluir todos os testes, mas durante a exploração do site relatou o problema de que o dropbox de categorias na página de “Busca” levou a página ao “Erro 1” e o “Erro 2” ao tentar desfavoritar . 

Usuário 2 | Luana 
--------- | --------------
Informações do usuário | 16 anos / Estudante / Acessa regularmente a Web para uso de redes social e sites de entretenimento 
Relatório | O usuário completou as tarefas com certa demora devido à dificuldade de discernir o botão de favorito, mesmo não relatando o “Erro 1” teve o mesmo “Erro 2”. 

Usuário 3 | Maria  
--------- | --------------
Informações do usuário | 58 anos / Aposentada / Baixo acesso sites Web 
Relatório | O usuário concluiu todos os testes, com certa demora, exceto o de favoritar (não conseguiu discernir o botão), e relatou o “Erro 3” quando ao explorar a página não consegui fazer uso da barra de pesquisa na página de “Buscas”. 

Usuário 4 | Miguel 
--------- | --------------
Informações do usuário | 64 anos / Aposentado / Acessa regularmente a Web 
Relatório | O usuário conseguiu concluir todos os testes facilmente exceto pelo de favoritar(não conseguiu discernir o botão), o usuário tentava abrir a página do site a ser favoritado. Esse usuário não relatou Erros. 

Usuário 5 | Luiza 
--------- | --------------
Informações do usuário | 22 anos / Estudante / Acessa regularmente a Web 
Relatório | O usuário conseguiu concluir todos os testes, com dificuldade, houve problemas de discernir o botão de favoritar.Não houve relatos de erros além dos já citados. 

Usuário 6 | Gabriel 
--------- | --------------
Informações do usuário | 25 anos / Atualmente desempregado / Acessa regularmente a Web 
Relatório | O usuário conseguiu concluir todos os testes facilmente e relatou todos os Erros anteriores.  

#### `Erros Notáveis`

ERRO 1: 

 > Ao tentar usar o dropbox na página de “Buscas” e clicando em “Boas Avaliações” 
o site desformatava o site pois os botões na sumiam junto dos sites sem boas avaliações. 
 - STATUS DO PROBLEMA: Resolvido 

ERRO 2: 

> Mesmo com desmarcando como favorito o site não saia dos favoritos 
 - STATUS DO PROBLEMA: Resolvido 

ERRO 3: 

 > A aba de buscas não estava funcionando 
 - STATUS DO PROBLEMA: Resolvido 

#### `Considerações Finais`
Durante questionamentos sobre o que acharam do site, todos demonstraram uma
opinião bem positiva e ficaram surpresos com a agilidade das correções feitas 
com o ERROs encontrados, mesmo assim mais do que claro que o botão de favoritar 
gerou certa confusão, mas não foi possível determinar uma solução para o problema. 

 
