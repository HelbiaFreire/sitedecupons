# sitedecupons
site de cupons
#language: pt
Funcionalidade Login
	Deve apresentar a tela do login com email e senha
cenário: Como um usuário válido, posso logar no sitema
	Dado que estou na tela de Login
	Quando digitar meu email e senha válido
	e clicar no botão de Login
	Então devo acessar a Home do Sistema
cenário: Como um usuário inválido, devo visualizar uma mensagem de Dados inválidos e continuar na pagina de login
	Dado que estou na tela de Login
	Quando digitar email e senha inválidas
	E clicar no botão de Login
	Então devo ver uma mensagem de dados inválidose devo estar na tela de Login
cenário: Como um usuário do facebook, posso logar no sistema usando meu perfil do facebook
	Dado que estou na tela de Login
	E escolho a opção facebook
	Quando clicar no botão facebook
	e logar no facebook
	Então devo ter acesso a home do Sistema
Funcionalidade Cadrastar
	Deve apresentar a tela de criar conta com campos nome, email e senha
cenário: Como um usuário válido, posso realizar o cadrastro
	Dado que estou da tela de cadrastro
	Quando digitar dados válidos não cadrastrados
	e clicar no botão Cadrastrar
	Então devo ter acesso ao sistema
cenário: Como usuário cadrastrado, sistema deve informar que estou cadrastrado
	Dado que estou na tela de cadrastrado
	Quando digitar dados válidos cadrastrados
	e clicar no botão Cadrastrar
	Então devo ver uma mensagem de Email já cadrastrado devo estar na tela de criar conta
Funcionalidade Comprar
	Deve apresentar um cupom escolhido com os valor visivel e descrição
cenário: Como um comprador, posso efetuar o pagamento de um cupom válido
	Dado que escolho o cupom válido
	e ao clicar visualizo a descrição
	Quando clicar no botão comprar
	Então deve exibir opções de pagamentos
cenário: Como um comprador, devo visualizar quando o cupom está inativo
	Dado que escolhi um cupom
	e ao clicar visualizo a descrição exibindo cupom inválido
	Então o botão Comprar deve está desabilitado
Funcionalidade Meus Cupons
	Quando clicar no nome do usuário e escolher a opção Meus Cupons deve apresentar a tela de cupons com cupons grátis e cupons pagos
cenário: Como usuário quero visualizar meus cupons gratis
	Dado que ganhei um cupom grátis válido
	e tenha apenas 5 dias válido
	Quando escolher Cupons grátis
	Então o sistema deve listar meu cupom com a validade
cenário: Como Comprador quero visualizar as compras dos meus cupons
	Dado que realizei uma compra no sistema
	Quando clicar no botão Meus cupons
	Então o sistema deve ser listados todos os cupons Disponíveis e Expirados
Funcionalidade busca
	Ao realizar uma busca no sistema deve apresentar um campo para Buscar cupons e outro campo para selecionar a cidade e um butão com o icone de uma lupa
cenário: Como usuário quero realizar busca apenas de cupom na minha cidade
	Dado que estou no campo cidade 
	e escolho uma cidade válida
	Quando clicar na cidade válida
	Então o sistema deve exibir apenas cupons da cidade escolhida
cenário: Como usuário esclho uma cidade que não possui no cadrastrado
	Dado que estou no campo cidade
	e digito uma cidade inválida
	Quando clicar em buscar 
	Então o sistema deve permanecer na home com o icone de busca desabilitado
Funcionalidade Meus Favoritos
	Os cupons deve ter uma marcação de favoritos, e um acesso a lista de favoritos
cenário: Como usuário quero visualizar os cupons marcados como favoritos, para comprar.
	Dado que estou em meu perfil na opção meus favoritos e selecionei uns cupons como favoritos
	e visualizo todos os cupons marcados com o valores coretos
	Quando clicar no cupom válido
	Então sistema deve ser direcionado para o cupom com suas informaçoes
cenário: Como usuário quero excluir cupons na lista de favoritos
	Dado que estou em meu perfil na opção meus favoritos e selecionei uns cupons como favoritos
	e visualizo todos os cupons
	Quando Clicar na lixeira
	Então o sistema deve apagar o cupom do meu perfil



