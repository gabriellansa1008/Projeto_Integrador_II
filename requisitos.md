# Sistema de Controle de Achados e Perdidos
O funcionamento desse sistema consiste numa solução bastante simples, como o foco principal na acessibilidade e agilidade do processo de localização e devolução 
do objeto. 
## Escopo Geral do Projeto
As funcionalidades gerais fornecidas pelo sistema permitem uma busca simples e objetiva. 
### Dentro do escopo
- Cadastro de objetos;
- Consulta e pesquisa;
- Visualização de detalhes;
- Edição de registros;
- Controle de situação;
- Registro de devoluções;
- Remoção de registros.
### Fora do escopo
- Aplicativo para celular;
- Inteligência artificial;
- Envio de SMS;
- Integrações externas;
- Sistema de pagamentos.

## Tipos de usuário
As funcionalidades são diferentes para os tipos de usuário "responsável" e "usuário", definidos no momento do login no sistema,
como mostra a tabela abaixo: 

|Funcionalidade                    |  Tipo de usuário       |
|----------------------------------|------------------------|
|Cadastro de objetos encontrados   |  Responsável           |
|Consulta de objetos               |  Responsável e Usuário |
|Pesquisa de objetos               |  Responsável e Usuário |
|Visualização de detalhes          |  Responsável e Usuário |
|Edição de informações             |  Responsável           |
|Controle da situação dos objetos  |  Responsável           |
|Registro de devoluções            |  Responsável           | 
|Remoção de registros              |  Responsável           | 

## Requisitos funcionais 
### 01. Cadastrar usuário
O sistema permite cadastrar dois tipos diferentes, "usuário" e "responsável" . 
Exemplo de aplicação em um ambiente escolar:
|Usuários reais                    |  Tipo de usuário       |
|----------------------------------|------------------------|
|Funcionário da instituição responsável pelos achados e perdidos   |  Responsável           |
|Alunos               |  Responsável e Usuário |

### 02. Cadastrar objeto
O sistema deverá permitir que o responsável cadastre um objeto encontrado. Esse registro só será feito com todos esses requisitos preenchidos:
- Descrição
- Local onde foi encontrado
- Data em que foi encontrado.
- Código de identificação do objeto

### 03. Consultar e Pesquisar objetos
A consulta e a pesquisa dos objetos pode ser feita através das informações disponíveis no cadastro dele. Exemplo: o usuário perdeu uma garrafa branca na escola
e pretende consultar o sistema.  Ele verifica que há uma garrafa branca esquecida no bloco dos professores . A segurança se amplia com a visualização dos detalhes
do objeto.

### 04. Editar objeto
O responsável consegue editar as informações do objeto preenchidas no momento do cadastro.

### 05. Editar situação do objeto
O responsável poderá modificar as situações em que o objeto se encaixa. São elas:
- encontrado,
- aguardando retirada,
- devolvido.

### 06. Remover objeto
A remoção de um registro poderá ser feita pelo responsável. 


## Requisitos não funcionais

### 01. Acessibilidade
A interface do projeto é objetiva e não complexa, permitindo que o usuário usufrua do sistema de forma intuitiva.

### 02. Segurança
As funcionalidades de cadastro, edição e remoção de objetos deverão estar disponíveis somente para o responsável autorizado.

### 03. Agilidade
O sistema deve responder às pesquisas dos usuários sem um atraso significativo , de modo que a experiência desses indivíduos seja satisfatória.

### 04. Manutenções
O sistema permite mudanças, atualizações e futuras melhorias .

### Observações: 
Esses requisitos estão definidos nessa etapa inicial do projeto e podem ser aperfeiçoados ou modificados.

## Regras obrigatórias 

- Um objeto que estiver com a situação "devolvido" não deverá ser considerado como disponível para retirada;
- O cadastro como responsável ou como usuário deverá ser regulado pela instituição. Por exemplo, funcionário da escola como responsável e alunos como usuários;
- Por se tratar de um sistema simples, aplicativos para celular e envio de mensagens através do sistema ainda não estão integrados ao sistema;
- Quando devolvido o objeto deve conter a data de devolução.
  
## Cadastro de objetos
Ao cadastrar o objeto perdido o responsável deve obrigatoriamente preencher estas informações:
- Código único do registro	
- Descrição do objeto		
- Características	ou informações que ajudam na identificação
- Local onde foi encontrado	
- Data em que foi encontrado	
- Situação atual do objeto	

## Conclusão 
O sistema consiste numa solução simples e objetiva para controlar objetos que foram perdidos , ela foi pensada para ser utilizada principalmente em espaços educacionais. O Sistema de Achados e Perdidos apresenta uma solução e uma estrutura para organizar uma atividade comum, permitindo sua evolução em etapas posteriores.
