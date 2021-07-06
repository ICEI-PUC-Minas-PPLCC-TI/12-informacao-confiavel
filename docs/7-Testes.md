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

> Enumere quais cenários de testes foram selecionados para teste. Neste
> tópico o grupo deve detalhar quais funcionalidades avaliadas, o grupo
> de usuários que foi escolhido para participar do teste e as
> ferramentas utilizadas.

### Ferramentas de Testes (Opcional)

> Comente sobre as ferramentas de testes utilizadas.


### Avaliação

> Discorra sobre os resultados do teste. Ressaltando pontos fortes e
> fracos identificados na solução. Comente como o grupo pretende atacar
> esses pontos nas próximas iterações. Apresente as falhas detectadas e
> as melhorias geradas a partir dos resultados obtidos nos testes.
