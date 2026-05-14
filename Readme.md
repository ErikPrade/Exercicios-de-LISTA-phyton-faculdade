#1
produtos = ["coca","fruki","sprite","agua","fanta"]
produtos[2] = "pepsi"
print(produtos)
print(len(produtos))




#2
produtos = ["tv", "celular", "mouse", "teclado", "tablet"]
estoque = [100, 150, 80, 120, 60]

produto = input("Digite o nome do produto que deseja: ")
if produto in produtos:
    i = produtos.index(produto)

    quantidade = estoque[i]

    print(f"O produto {produto} está na posição {i} da lista.")
    print(f"Temos {quantidade} unidades em estoque.")
else:
    print("Produto não encontrado no sistema.")





#3
vendas = [1000, 1500, 350, 270, 900, 1200, 700]
print(len(vendas))
print(sum(vendas))

if max(vendas) < 1400:
    print(f"a maior venda foi menor que: 1400")
if max(vendas) > 1400:
    print(f"a maior venda foi maior que: 1400")
if min(vendas) < 300:
    print(f"a menor venda foi menor que: 300")
if min(vendas) > 300:
    print(f"a menor venda foi maior que: 300")




#4
produtos = ["apple tv", "mac", "iphone x", "iPad"]
novos_produtos = ["apple watch", "mac book", "airpods"]

produtos.extend(novos_produtos)
print(produtos)
produtos_lista_original = ["apple tv", "mac", "iphone x", "iPad"]
produtos_completos = produtos_lista_original + novos_produtos
print(produtos_completos)

produtos_teste = ["apple tv", "mac", "iphone x"]
novos = ["airpods", "apple watch"]

produtos_teste.append(novos)
print(produtos_teste)






#5
produtos = ["apple tv", "mac", "iphone x", "iPad", "apple watch", "mac book", "airpods"]
vendas = [1000, 1500, 15000, 270, 900, 100, 1200]
lancamento = [2010, 2026, 2009, 2005, 1997, 2001, 2022]

produtos_ordenados = sorted(produtos)

vendas_ordenadas = sorted(vendas)

lancamento_ordenado = sorted(lancamento, reverse=True)

print("\n".join(produtos_ordenados))

print(vendas_ordenadas)
print(lancamento_ordenado)





#6
texto_produtos = "apple tv, mac, iphone x, iPad, apple watch, mac book, airpods"

lista_produtos = texto_produtos.split(", ")

print(lista_produtos)

print(len(lista_produtos))

busca = input("Digite o produto que deseja encontrar: ")

if busca in lista_produtos:
    posicao = lista_produtos.index(busca)
    print(f"O produto está na posição: {posicao}")
else:
    print("Produto indisponível")





#7
lista1 = ["apple tv", "mac", "iphone 12", "iPad", "notebook"]

lista2 = lista1.copy()

lista2[4] = "pc"

print(f"Lista Original: {lista1}")
print(f"Lista Alterada: {lista2}")




#8
vendedores = ["Lira", "Joao", "Diego", "Alon"]
produtos = ["ipad", "iphone"]
vendas = [
    [100, 200],
    [300, 500],
    [50, 1000],
    [900, 10]   ]


print(f"Vendas totais do João: {vendas[1]}")

venda_iphone_diego = vendas[2][1]
print(f"Vendas de iPhone do Diego: {venda_iphone_diego}")

busca = input("Digite o nome do vendedor: ")

if busca in vendedores:
    i = vendedores.index(busca)
    quantidade_total = sum(vendas[i])
    print(f"O vendedor {busca} vendeu um total de {quantidade_total} unidades.")
else:
    print("Vendedor não encontrado")
