programa {
   funcao inicio() {
      
      inteiro vetor[10], i, j, aux

      vetor[0] = 2
      vetor[1] = 5
      vetor[2] = 1
      vetor[3] = 3
      vetor[4] = 4
      vetor[5] = 9
      vetor[6] = 7
      vetor[7] = 8
      vetor[8] = 10
      vetor[9] = 6

      para (i = 0; i < 9; i++) {
         para (j = 0; j < 9 - i; j++) {
            se (vetor[j] < vetor[j + 1]) {
              
               aux = vetor[j]
               vetor[j] = vetor[j + 1]
               vetor[j + 1] = aux
            }
         }
      }

      
      escreva("Vetor em ordem decrescente: ")
      para (i = 0; i < 10; i++) {
         escreva(vetor[i], " ")
      }
   }
}
