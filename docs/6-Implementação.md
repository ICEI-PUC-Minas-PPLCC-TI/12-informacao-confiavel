# Implementação da solução
Nesta seção são apresentados os detalhes técnicos da solução criada pela equipe,
tratando da Arquitetura da Solução, as estruturas de dados e as telas já implementadas.
## Arquitetura da solução
### Diagrama de componentes
Os componentes que fazem parte da solução são apresentados na Figura que se
segue.
![diagram](/docs/images/diagrama_componente.PNG)

A solução implementada conta com os seguintes módulos:
* **Navegador** - Interface básica do sistema
  * **Páginas Web** - Conjunto de arquivos HTML, CSS, JavaScript e imagens que
implementam as funcionalidades do sistema.  
  * **Local Storage** - armazenamento mantido no Navegador, onde são
implementados bancos de dados baseados em JSON. São eles:
    * **Canais** - tags de notícias apresentadas
    * **Avaliações** - registro de opiniões dos usuários sobre os sites
    * **Favoritos** - lista de notícias que foram favoritadas pelo usuário 
* **API** - plataforma que permite o acesso às notícias exibidas no site.
* **Hospedagem** - local na Internet onde as páginas são mantidas e acessadas pelo
navegador.

### Hospedagem
O site utiliza a plataforma do Github como ambiente de hospedagem do site do projeto.
O site é mantido no ambiente da URL:
https://github.com/ICEI-PUC-Minas-PPLCC-TI/12-informacao-confiavel

O site utiliza a plataforma do Github como ambiente de hospedagem do site do projeto.
O site é mantido no ambiente da URL:
https://github.com/ICEI-PUC-Minas-PPLCC-TI/12-informacao-confiavel
## Template do site
### Tela principal
Tela que abrange todas as visualizações iniciais do site e a listagem dos mesmos.
![home](/docs/images/home.PNG)
### Buscas
Exibição de sites para avaliação e marcar como favorito.
![busca](/docs/images/buscas.PNG)
### Favoritos
Tela que mostra os sites arcados como favorito
![favoritos](/docs/images/favoritos.PNG)
### Tela de Login
Local onde o usuário irá cadastrar e logar com sua conta.
![login](/docs/images/login.PNG)
## Funcionalidades do Sistema (Telas)
Nesta seção são apresentadas as telas desenvolvidas para cada uma das
funcionalidades do sistema. O respectivo endereço (URL) e outras orientações de acesso são
apresentadas na sequência.
### Categorização do site de acordo com reputação ( RF-02)
A partir das avaliações fornecidas pelos usuários criamos uma pontuação de 0 a 10
para determinar a reputação de determinado domínio ou URL. Isso se torna visível ao usuário
ao lado do nome de cada página. No código definimos 3 estados de reputação (boa, neutra
e ruim) definidas respectivamente pelos _ranges_ 0 a 4; 4 a 6 e 6 a 10.
![rf-02](/docs/images/rf_02.PNG)
* Indicador: Ícones: rosto com coloração verde, amarelo e vermelho.
* O algoritmo analisa a nota do site, sendo de 0 à 10. Assim, caso a nota seja menor
que 4, o indicador terá coloração vermelha. Caso esteja entre 4 e 6, inclusive,
coloração amarela. E, caso esteja maior que 6, coloração verde.
* A nota do site é analisada a partir de um JSON que contém as informações dele.
#### **Requisitos atendidos**
* RF-01: Sistema de avaliação por site para demonstrar sua credibilidade.
* RF-02: Coloração própria que correspondente a confiabilidade da informação 
#### **Artefatos de funcionalidade**
* Função para o indicador de confiabilidade do site mudar de cor de acordo com sua
nota.
#### **Estrutura de Dados**
![](/docs/images/rf_02_estrutura1.PNG)
![](/docs/images/rf_02_estrutura2.PNG)
#### Instruções de acesso 
1. Abra um navegador de Internet e informe a seguinte URL: https://12-informacaoconfiavel-omega.vercel.app/
2. A tela de sites é a primeira funcionalidade exibida pelo aplicativo.
### Filtro de sites com nota boa (RF-03)
A partir da análise do contexto e da aplicabilidade do desenvolvimento desta
aplicação, foi observado que necessita-se de uma forma de “filtro de qualidade” das notícias
exibidas como exibir apenas notícias com boa avaliação (maior que pontuação 0).
![](/docs/images/rf_03.PNG)
* Imagem 1: Filtro não selecionado.
* Imagem 2: Filtro selecionado.
* Seleciona as manchetes com notícias de sites com boas avaliações.
* O algoritmo entende um site com uma boa avaliação um site que tem o valor da
mesma maior que 0.
* O valor da avaliação é analisado por meio dos valores armazenados no localStorage,
que por sua vez são adquiridos por meio de arquivo JSON.
#### **Requisitos atendidos**
RF-03: O site deve oferecer uma funcionalidade de filtro/pesquisa para permitir ao usuário
bloquear conteúdos de baixa avaliação.
#### **Artefatos da funcionalidade**
* Função para filtrar apenas sites com pontuação “Boa”.
#### **Estrutura de Dados**
![](/docs/images/rf_03_estrutura.PNG)
#### **Instruções de acesso**
1. Abra um navegador de Internet e informe a seguinte URL: https://informacaoconfiavel.lucaribeiro1.repl.co/buscas.html
2. Entre na aba “Buscas”.
3. Clique no botão representado por um filtro.
4. Agora, seleciona o botão: Boas avaliações.
#### **Instruções de acesso ao código fonte**
1. Abra um navegador de Internet e entre no link: https://github.com/ICEI-PUC-MinasPPLCC-TI/12-informacao-confiavel/blob/master/src/scripts/app.js
2. Logo após, navegue até a linha 155.
### Compartilhamento em redes sociais (RF-04)
A partir das APIs das principais redes sociais é possível fazer um link para
compartilhar o site e o seu conteúdo.
![](/docs/images/rf_04.PNG)
#### **Requisitos atendidos**
RF-04: O site deve permitir o compartilhamento de avaliações de sites em plataformas de
redes sociais
#### **Artefatos da funcionalidade**
* Função para compartilhar o site nas mídia sociais.
#### **Instruções de acesso**
1. Abra um navegador de Internet e informe a seguinte URL: https://informacaoconfiavel.lucaribeiro1.repl.co/buscas.html
2. Entre na aba “Buscas”.
3. Adicione algum dos dominios ao seus favoritos.
4. Entre na aba “Favoritos”.
5. Compartilhe na sua rede social preferida.
#### **Instruções de acesso ao código fonte**
1. Abra um navegador de Internet e entre no link: https://github.com/ICEI-PUC-MinasPPLCC-TI/12-informacao-confiavel/blob/master/src/scripts/app.js
2. Logo após, navegue até a linha 247.
### Filtro de sites (RF-05)
A tela de pesquisa permite ao usuário informar um texto que será pesquisado na base de
sites e retornar todas que tiverem uma ocorrência do texto digitado no campo nome, url ou
descrição.
![](/docs/images/rf_05.PNG)
#### **Artefatos da funcionalidade**
* index.html
* app.js:search()
#### **Instruções de acesso**
1. Faça o download do arquivo do projeto (ZIP) ou clone do projeto no GitHub;
2. Descompacte o arquivo em uma pasta específica;
3. Abra o Visual Studio Code e execute o Live Server;
4. Abra um navegador de Internet e informe a seguinte URL:
http://localhost:5500/index.html
### Favoritos (RF-06)
![](/docs/images/rf_06.PNG)
* Ferramenta para adicionar ou remover webpages da lista de favoritos
#### **Artefatos da funcionalidade**
* Botão de like(estrelinha)quando clicado é capaz de definir sites favoritos e separá-los
na sessão de “Favoritos” do site.
* function:setFav() e function:showFavorites() 
#### **Instruções de acesso**
1. Abra um navegador de Internet e informe a seguinte URL:
https://Informacao-Confiavel.lucaribeiro1.repl.co
2. Clique em “Busca” marque uma opção como favorito
3. Clique na aba “Busca”
4. Adicione sites aos favoritos selecionando a estrela
5. Acesse a aba “Favoritos” e veja os sites marcados como favoritos
6. Remova as páginas do favoritos clicando novamente na estrela
### Sistema de “rating” funcional (RF-07)
![](/docs/images/rf_07.PNG)
* A programação em Java Script agora permite que os botões de “gostei” e “não gostei”
mudem os status da avalição dos sites no localStorage.
* Cada botão gera um incremento ou decremento na categoria em específico, o
cálculo final é feito através da soma de todos os valores das categorias (design,
information, user interface, partiality).
#### **Artefatos da funcionalidade**
* Função que calcula avalição do site e com base nela muda a avalição do site
no localStorage também alterando o ícone na esquerda com base na somatória
dos votos.
* function changeReputation()
#### **Instruções de acesso**
1. Abra um navegador de Internet e informe a seguinte URL: https://informacaoconfiavel.lucaribeiro1.repl.co/buscas.html
2. Clique em algum site e avalie negativamente
3. Abra o local o Storage nas ferramentas de desenvolvedor do navegador(F12 ou
CRTL+SHIFT+C), perceba os valores alterados
4. Avalie negativamente até que o ícone demonstre uma reputação ruim
5. Avalie positivamente até que o ícone demonstre uma reputação boa
6. Faça com que as somas das categorias dê 0, perceba o ícone de avaliação neutra
#### **Estrutura de dados**
![](/docs/images/rf_07_estrutura1.PNG)
![](/docs/images/rf_07_estrutura2.PNG)
### Sistema de Cadastro (RF-08)
A opção de “Cadastro” no menu levará a uma página que permite ao usuário digitar seu
“nome”, “sobrenome”, “email”, “senha” e “confirmação de senha” para que o usuário seja
cadastrado no sistema.

![](/docs/images/rf_08.PNG)

#### **Artefatos da funcionalidade**
* cadastro.html;
* App.js:cadastro();
#### **Estrutura de dados**
![](/docs/images/rf_08_estrutura.PNG)
#### **Instruções de acesso ao site**
1. Abra um navegador de Internet e informe a seguinte URL:
https://informacao-confiavel.lucaribeiro1.repl.co/buscas.html
2. Clique na opção “Login” no menu.
3. Clique na opção “Cadastre aqui”.
4. Insira “Email”, “Nome”, “Sobrenome”, “Senha” que deseja cadastrar e “Confirmar
Senha” inserindo a mesma senha anteriormente digitada para, então, efetuar
corretamente o Cadastro no sistema.
#### **Instruções de acesso ao código fonte**
1. Abra um navegador de Internet e entre no link: https://github.com/ICEI-PUC-MinasPPLCC-TI/12-informacao-confiavel/blob/master/src/scripts/app.js
2. Logo após, navegue até a linha 301.
### Sistema de Login (RF-09)
A opção de “Login”, no menu, agora levará a uma página que permite ao usuário digitar seu
“email” ou “usuário” cadastrado previamente.

![](/docs/images/rf_09.PNG)

#### **Artefatos da funcionalidade**
* Login.html;
* App.js:login();
#### **Estrutura de dados**
![](/docs/images/rf_09_estrutura.PNG)
#### **Instruções de acesso ao site**
* Abra um navegador de Internet e informe a seguinte URL:
https://informacao-confiavel.lucaribeiro1.repl.co/buscas.html
* Clique na opção “Login” no menu.
* Insira “teste@admin.com” como usuário e “teste” como senha (ou alguma outra
conta cadastrada previamente)
#### **Instruções de acesso ao código fonte**
1. Abra um navegador de Internet e entre no link: https://github.com/ICEI-PUC-MinasPPLCC-TI/12-informacao-confiavel/blob/master/src/scripts/app.js
2. Logo após, navegue até a linha 318.
### Hospedagem do projeto (RNF-01)
![](/docs/images/rnf_01.PNG)
* Interface da aplicação do site de hospedagem.
#### **Artefatos da funcionalidade**
* Site de hospedagem do projeto(replit).
#### **Instruções de acesso**
1. Abra um navegador de Internet e informe a seguinte URL:
https://Informacao-Confiavel.lucaribeiro1.repl.co



