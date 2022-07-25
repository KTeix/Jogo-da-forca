# Jogo-da-forca
Em desenvolvimento
programa
{
		inclua biblioteca Texto --> tx
	cadeia palavra 
	cadeia letra 
	inteiro tam
	inteiro cont = 0
	inteiro cont1 = 0
	cadeia vet[10]
	inteiro controle = 1
	cadeia baseforca[10]
	funcao inicio()
	{


	
	escreva("Jogador 1, digite a frase")
	leia(palavra)
	limpa()
	tam = tx.numero_caracteres(palavra)
	
	/*escreva("_____________\n")
	escreva("I           I\n")
	escreva("I\n")
	escreva("I\n")
	tamanho = tx.numero_caracteres(palavra)
	para(conttamanho = 0; conttamanho <= tamanho; conttamanho++){
	escreva(" _")
	}*/
	enquanto(controle == 1){
	escreva("Jogador2, digite uma letra valendo sua vida \n")
	leia(letra)
		para(cont=0; cont < tam; cont++){
			vet[cont] = tx.extrair_subtexto(palavra,cont, cont+1)
		
		se(letra == vet[cont]){
		baseforca[cont] = letra
		} 
		senao se (palavra == baseforca[cont]){
			escreva("Você venceu")
			controle = 1
		}
		
		}
		para(cont = tam; tam > 0; tam--){
			
		}
	}
	}
}
