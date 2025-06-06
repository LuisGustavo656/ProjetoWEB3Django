DjangoProjeto

Esse projeto foi desenvolvido durante as aulas de Desenvolvimento Web 3
ele se baseia em um sistema de compras, onde qualquer pessoa consegue cadastrar seu produto para venda,
mas somente o admin pode ver os usuarios,edita-los ou exclui-los
Foi desenvolvido em python por meio da frameqork Django
As Funções disponiveis no dashboard somento são exibidas quando o usuario está logada

COMANDOS PARA EXECUTAR AO BAIXAR(EXECUTE NO CMD)
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver

AS EXECUÇÕES
HOME
Apenas um botão de cadastre-se e um Header com as opções de Home,Quem somos,Produtos,Login
CADASTRO
Cadastro de Usuario pedindo o nome, email, senha, confirmação,
CEP,Logradouro, Bairro,Localidade, Uf, Numero da residencia
LOGIN
Acesso usando o email e senha cadastrado, assim q confirmado vai direto pro Dashboard
DASHBOARD
O usuario consegue acesso das paginas Produtos e Dashboard após realizar o cadastro e se logar no site, 
dentro da Pagina dashboard ele consegue ver o grafico dos produtos cadastrados no banco de dados, 
o grafico de vendas registradas no banco de dados(ordenado por dia e total gasto),
Listar os produtos,ou seja, exibir eles
Cadastrar os produtos
Caso seja admin vc consegue entrar na listas de usuarios

PRODUTOS
O usuario consegue ver a lista de produtos, excluir o produto, editar o produto,cadastrar o produto(tendo a categoria Produto e categoria Jogos)
consegue efetuar compra tbm indo ditero para pagina de checkout

CADASTRAR PRODUTO
Nessa pagina o usuario vai cadastrar o produto colocando o nome,uma descrição
a quantidade em estoque e o preço(O estoque,nome vão ser exibidos no grafico de estoque)
EDITAR PRODUTO
Basicamente a mesma pagina do cadastro de produtos
CHECKOUT
Vai aparecer a area de pagamento
Onde vai poder ser inserido o numero do cartão,com verificação se é valido ou não,
a data de validade, também com verificação de validade,
e o CVV, também com verificação,
Assim q confirmado tudo o botão de finalizar compra redicionara para a pagina checkout_sucesso
também será registrado o id e valor do produto no banco de dados para ser incorporado no grafico de vendas e estoque

CHECKOUT_SUCESSO
Aparecerá a foto do produto junto com a mensagem de compra confirmada
