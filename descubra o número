import random
#ainda não resolvi entrada de char para as jogadas no meio do jogo
#adicionar uma char no meio do jogo causa um break
n = str(input("Escreva seu nome: ")) #escrever o nome do jogador
e = 'S' #variavel 'e', usada em um looping
if e == 'S': #Se 'e' =='S' executar o jogo
	while e != 'N': #enquanto

		x = int(input("Digite o tamanho do intervalo que deseja para o jogo:\n10 - easy as never\n100 - getting interesting\n1000 - agora é sério\n10000 - Tu é TOP\n100000 - Hard Core\n1000000 - Crazy as ever\n"))
		print("Let's start\n\nVai chutando aí o valor até acertar.\nO número de tentativas será guardado")
		if x < 21:
			t = x / 6 #'t' é o número de tentativas possíveis
		if x < 101:
			t = x / 10
		if x < 5001:
			t = x / 50
		if x < 10001:
			t = x / 120
		else:
			t = x / 500
		i = 0 #'i' é a quantidade de tentativas
		tent = 0 #'tent' é para uso no loop. Repare que 'tent' recebe o valor de 'i'
		#acert = 0 #'acert' é a quantidade de acertos. Seria usado para uma memoria de jogo (criar arquivo em máquina para guardar histórico)
		z = random.randint(1, int(x)) #gerador no numero aleatório
		while tent < t:
			#print(i) #usado para printar o nº da jogada
			#print(z) #usado para printar o nº a ser adivinhado
			y = int(input("\nManda bala:"))
			if y > z:
				print("O número é menor")
			if y < z:
				print("Um pouco mais")
			if y == z:
				print("Congrats my friend")
				tent = t - 1 #operação para finalizar o loop
			i = i + 1 #acrescenta a tentativa feita
			tent = tent + 1 #parametro para o loop
		if i == t or y != z:
			print("Lamento mas você não consguiu...\n Suas tentativas foram:\n"+ str(i))
		if y == z:
			print("Top!!\nVocê acertou após "+ str(i) +" jogadas")
		tent = 0 
		e = input("Jogar novamente?\nS - Sim,   N - Não  : \n")
		e = e.upper() #se a entrada 'e' for minuscula, converterá para maiúscula, e será usada no primeiro loop
else:
	pass
