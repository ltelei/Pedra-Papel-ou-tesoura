Algoritmo "semnome"
//
//
// Descrição   : Pedra(1) papel(2)ou tesoura(3)
// Autor(a)    : Lucas Abreu Leite Nepomuceno
// Data atual  : 21/03/2023
Var
   player,cpu,pause,op, vit, emp, der:inteiro


Inicio
   enquanto op <>  2 faca

      escreval( " escolha: ")
      escreval (" Pedra(1) ")
      escreval(" Papel(2) ")
      Escreval ( " ou tesoura(3) " )
      leia (player)
      cpu <-randi(3)+1



      escolha (player)
      caso 1
         escreva(" PLAYER : PEDRA")
      caso 2
         escreval(" PLAYER : PAPEL")
      caso 3
         escreval(" PLAYER : TESOURA ")
      fimescolha



      escolha (cpu)
      caso 1
         escreva(" CPU : PEDRA")
      caso 2
         escreval(" CPU : PAPEL")
      caso 3
         escreval(" CPU : TESOURA ")
      fimescolha




      se (player = cpu)entao
         escreval (" empate ")
         emp<-emp+1
      senao
         se(((player=1) e (cpu=3))ou((player=2) e (cpu=1))ou((player=3) e (cpu=2))) entao
            escreval(" vitória ")
            vit<-vit+1
         senao
            escreval(" derrota")
            der<-der+1
         fimse
      fimse

      escreval (" Voce deseja continuar? S = 1, N = 2 : ")
      leia (op)
      escreval ("Vitorias" , vit)
      escreval ("Empates" , emp)
      escreval ("Derrotas",der)


   fimenquanto



Fimalgoritmo
