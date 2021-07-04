# Projeto da Solução

#### Apresentado nessa sessão estão os detalhes técnicos da solução criada pela equipe.

## Tecnologias Utilizadas

> Descreva aqui qual(is) tecnologias você vai usar para resolver o seu
> problema, ou seja, implementar a sua solução. Liste todas as
> tecnologias envolvidas, linguagens a serem utilizadas, serviços web,
> frameworks, bibliotecas, IDEs de desenvolvimento, e ferramentas.
> Apresente também uma figura explicando como as tecnologias estão
> relacionadas ou como uma interação do usuário com o sistema vai ser
> conduzida, por onde ela passa até retornar uma resposta ao usuário.
> 
> Inclua os diagramas de User Flow, esboços criados pelo grupo
> (stoyboards), além dos protótipos de telas (wireframes). Descreva cada
> item textualmente comentando e complementando o que está apresentado
> nas imagens.

## Arquitetura da solução

> Inclua um diagrama da solução e descreva os módulos e as tecnologias
> que fazem parte da solução. Discorra sobre o diagrama.

A imagem a seguir ilustra o fluxo do usuário em nossa solução. Assim
que o usuário entra na plataforma, ele é apresentado à tela inicial
(Main Page) onde ele possui as seguintes opções: 
 1. Clicar em um dos sites em destaque e ser direcionado a ele.
 2. Clicar em alguma das opções no _Header_.
 3. Clicar no círculo inferior direito para ativar o _Dark mode_.

Caso ele opte pela opção 1 e escolha um dos sites em destaque, ele será 
redirecionado para uma o site, assim como possuirá uma opção de avaliação.

Caso ele opte pela opção 2, o usuário poderia escolher entre: 
 - `Home`: página principal.
 - `Busca`: página para buscar um site em específico.
 - `Favoritos`: apresenta os favoritos do usuário.
 - `Login`: entrar com usuário ou cadastrar-se.
 - `Sobre`: possui informações sobre o grupo.

Caso o usuário opte por `Home` ele será enviado para mesma página em que está. 

Caso o usuário opte por `Busca` ele será enviado para uma página que possui 
uma barra para pesquisar. Escrever o nome do site fará com que ele potencialmente 
apareça e assim seja possível acessa-lo, favorita-lo ou avalia-lo.

Caso o usuário opte por `Favoritos` ele será enviado para uma página contendo 
os sites marcados como "favoritos", representados pela estrela. Assim, há 
também uma opção de retira-los dos favoritos, avalia-los e acessa-los.

Caso o usuário opte por `Login` ele será enviado a uma página que o permitirá 
entrar com sua conta ou se cadastrar. Se o usuário deseja cadastrar-se então 
ele será enviado para outra página com essa função. Após terminado o processo
de login/cadastro, o usuário é redirecionado para a Main Page.

Caso o usuário opte por `Sobre` ele será enviado para uma página contendo 
informação sobre os integrantes do grupo.

![tela principal](/docs/images/mainpage.png)
![Exemplo de UserFlow](/docs/images/flowmap.png)
