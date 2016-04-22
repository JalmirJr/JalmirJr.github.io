---
title: "Jogo da Velha"
# jekyll-seo-tag
description: "Desenvolvendo um Jogo da Velha em Python"
image:        "http://placehold.it/400x200"
author:       "Osuh"
---

## Criando o tabuleiro
O tabuleiro de um jogo da velha tem o formato 3x3, ou seja, 9 espaços. Para se representar isso
em Python, vamos primeiro criar uma lista com nove elementos. O proximo passo e exibir esse lista,
para isso usamos um loop para imprimir todos os 9 elementos dela. Porem nao sera representada na
forma 3x3, para isso precisaremos usar um contador para se qubrar uma linha: 

``` python
	board = [1, 2, 3, 4, 5, 6, 7, 8, 9]
	def board_show():
		count = 1

		for i in board:
			if count % 3 == 0:
				print i
			else:
				print i,
			count = count + 1