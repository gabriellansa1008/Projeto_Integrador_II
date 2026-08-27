# Arte na Escola

## Arquitetura e Modelagem do Sistema

## 1. Visão geral

O **Arte na Escola** será uma plataforma destinada à divulgação e valorização dos desenhos produzidos pelos alunos da instituição.

O sistema permitirá que alunos criem uma conta, publiquem seus desenhos e gerenciem suas próprias publicações. Visitantes poderão visualizar os desenhos e consultar informações sobre os artistas sem a necessidade de realizar login.

A plataforma terá uma interface simples, organizada e intuitiva, facilitando o acesso às publicações.

---

## 2. Usuários do sistema

O sistema possuirá dois tipos principais de usuários:

### Aluno/Artista

O aluno poderá:

* Criar uma conta;
* Realizar login;
* Publicar desenhos;
* Editar suas próprias publicações;
* Remover suas próprias publicações;
* Pesquisar perfis de artistas.

### Visitante

O visitante poderá:

* Visualizar desenhos publicados;
* Pesquisar perfis de artistas;
* Visualizar informações dos artistas;
* Visualizar os trabalhos publicados.

---

## 3. Funcionamento do sistema

O funcionamento será dividido entre as ações que podem ser realizadas por visitantes e alunos.

O visitante poderá acessar a plataforma sem realizar login para visualizar os desenhos e os perfis dos artistas.

Para publicar, editar ou remover um desenho, o aluno deverá possuir uma conta e estar autenticado.

### Fluxo geral

1. O usuário acessa o sistema.
2. O usuário pode visualizar os desenhos publicados.
3. Caso seja um aluno, poderá criar uma conta ou realizar login.
4. Após realizar login, poderá publicar um desenho.
5. O aluno poderá editar ou remover suas próprias publicações.
6. Os visitantes poderão visualizar os trabalhos publicados e as informações dos artistas.

---

## 4. Fluxograma

```text
                         INÍCIO
                            |
                            v
                    Acessar plataforma
                            |
                            v
                  Visualizar publicações
                            |
                            v
                    É aluno cadastrado?
                       /           \
                     NÃO            SIM
                      |              |
                      v              v
                 Continuar       Realizar login
                 como visitante       |
                      |               v
                      |        Acessar área do aluno
                      |               |
                      |        ┌──────┼───────┐
                      |        |      |       |
                      |        v      v       v
                      |    Publicar  Editar  Remover
                      |    desenho  desenho  desenho
                      |        |      |       |
                      |        └──────┼───────┘
                      |               |
                      └───────┬───────┘
                              |
                              v
                     Visualizar trabalhos
                              |
                              v
                             FIM
```

---

## 5. Publicação de desenhos

Para publicar um desenho, o aluno deverá estar autenticado.

Cada publicação deverá possuir:

* Título;
* Imagem;
* Categoria;
* Descrição.

Após publicada, a obra poderá ser visualizada pelos visitantes.

O aluno poderá editar ou remover somente as suas próprias publicações.

---

## 6. Pesquisa

O sistema permitirá que os usuários pesquisem desenhos por:

* Título;
* Nome do artista.

Também será possível pesquisar perfis de artistas.

A pesquisa terá como objetivo facilitar a localização de determinados trabalhos e artistas dentro da plataforma.

---

## 7. Perfil do artista

Cada aluno/artista possuirá um perfil contendo informações básicas e seus trabalhos publicados.

Os visitantes poderão acessar o perfil sem realizar login.

O perfil servirá como espaço para apresentação das produções artísticas do aluno.

---

## 8. Controle de acesso

O sistema terá diferentes permissões de acordo com o tipo de usuário.

```text
VISITANTE
│
├── Visualizar desenhos
├── Pesquisar desenhos
├── Pesquisar artistas
└── Visualizar perfis


ALUNO/ARTISTA
│
├── Todas as funções do visitante
├── Criar conta
├── Realizar login
├── Publicar desenhos
├── Editar suas publicações
└── Remover suas publicações
```

As funções de publicação, edição e remoção estarão disponíveis somente para alunos autenticados.

---

## 9. Modelo básico das informações

A estrutura inicial das principais informações do sistema será:

```text
ALUNO/ARTISTA
│
├── Nome
├── E-mail
├── Senha
└── Publicações
       │
       ├── Título
       ├── Imagem
       ├── Categoria
       └── Descrição
```

Um aluno poderá possuir várias publicações, enquanto cada publicação estará associada ao seu respectivo artista.

---

## 10. Estrutura das telas

O sistema poderá possuir as seguintes telas principais:

### Tela inicial

Apresentará os desenhos publicados e permitirá que o usuário realize pesquisas.

### Tela de login

Permitirá que alunos cadastrados acessem suas contas utilizando e-mail e senha.

### Tela de cadastro

Permitirá que novos alunos criem suas contas.

### Perfil do artista

Apresentará informações básicas do aluno e seus trabalhos publicados.

### Tela de publicação

Permitirá que o aluno autenticado informe:

* Título;
* Imagem;
* Categoria;
* Descrição.

### Tela de edição

Permitirá que o aluno altere as informações de uma publicação própria.

---

## 11. Requisitos não funcionais

A modelagem considera os requisitos não funcionais definidos para o projeto:

### Usabilidade

A interface deverá ser simples e organizada, facilitando sua utilização.

### Segurança

Publicações, edições e remoções deverão ser realizadas somente por alunos autenticados.

### Desempenho

Os desenhos e as informações solicitadas deverão ser apresentados de forma adequada durante a utilização do sistema.

---

## 12. Funcionalidades fora do escopo

Não fazem parte da proposta inicial do sistema:

* Comentários;
* Curtidas;
* Mensagens privadas;
* Seguidores;
* Pagamentos;
* Loja de desenhos;
* Integração com redes sociais;
* Aplicativo mobile.

Essas funcionalidades não serão consideradas na primeira versão do projeto.

---

## 13. Conclusão

A modelagem apresentada representa a estrutura inicial do projeto **Arte na Escola**, definindo os principais usuários, funcionalidades, permissões e fluxos do sistema.

A proposta busca criar um espaço digital simples para divulgar e valorizar os trabalhos artísticos produzidos pelos alunos da instituição.

Link do Trello:  https://trello.com/b/MbutCJNj/arte-na-escola
