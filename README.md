# Pedra-Papel-ou-tesoura
Pedra Papel ou tesoura no Visualg
o "semnome"
//
//
// Descrição   : Pedra(1) papel(2)ou tesoura(3)
// Autor(a)    : Lucas Abreu Leite Nepomuceno
// Data atual  : 21/03/2023
Var
   player,cpu:inteiro

Inicio

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

   senao
      se(((player=1) e (cpu=3))ou((player=2) e (cpu=1))ou((player=3) e (cpu=2))) entao
         escreval(" vitória ")
      senao
         escreval(" derrota")

      fimse
   fimse


Fimalgoritmo
