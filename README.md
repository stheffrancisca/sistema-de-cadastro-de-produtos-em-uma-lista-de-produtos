# sistema-de-cadastro-de-produtos-em-uma-lista-de-produtos
Este repositório contém um sistema simples de cadastro de produtos em uma lista de produtos. O objetivo é garantir um cadastro eficiente e evitar duplicações de produtos na lista.



### Criando um sistema de cadastro de produtos em uma lista de produtos
Seu sistema deve:
- Pegar o usuário qual produto vai ser cadastrado por meio de um input
- Garantir que se o usuário escrever com letra maiúscula ou minúscula, o produto continua sendo o mesmo produto
- Se o usuário inserir um produto que já existe na lista, o programa deve printar a mensagem "Produto já existente, tente novamente"
- Se o usuário inserir um produto que não existe na lista, o programa deve inserir na lista, printar a mensagem Produto X cadastrado com sucesso e em seguida printar a lista completa.

produtos = ["celular", "camera", "fone de ouvido", "monitor"]

novo_produto = input("Digite o produto para cadastrar:")
novo_produto = novo_produto.lower()

if novo_produto in produtos:
    print("Produto já existente, tente novamente")
else:
    produtos.append(novo_produto)
    print(f"Produto {novo_produto} cadastrado com sucesso")
    print(produtos)
