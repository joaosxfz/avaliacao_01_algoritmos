```bash
algoritmo "Sisteminha"
Var
  nomes: Vetor[1..10] de Caractere
  cargos: Vetor[1..10] de Caractere
  salarios: Vetor[1..10] de Caractere
  admissoes: Vetor[1..10] de Caractere
  ok: Inteiro
  total: Inteiro
  opcao: Inteiro
  busca: Caractere
  encontrado: Logico

inicio
  total <- 0

  
    Escreval("")
    Escreval("== MENU ==")
    Escreval("1 - Cadastrar funcionario")
    Escreval("2 - Pesquisar funcionario pelo nome")
    Escreval("3 - Exibir todos os funcionarios")
    Escreval("4 - Sair")
    Escreva("Opcao: ")
    Leia(opcao)



    Se opcao = 1 Entao
      Se total = 10 Entao
        Escreval("Nao e possivel cadastrar mais funcionarios.")
      Senao
        total <- total + 1
        Escreva("Nome: ")
        Leia(nomes[total])
        Escreva("Cargo: ")
        Leia(cargos[total])
        Escreva("Salario: ")
        Leia(salarios[total])
        Escreva("Data de admissao: ")
        Leia(admissoes[total])
        Escreval("Cadastrado!")
      FimSe
    FimSe



    Se opcao = 2 Entao
      Se total = 0 Entao
        Escreval("Nenhum funcionario cadastrado.")
      Senao
        Escreva("Nome: ")

        Leia(busca)

        encontrado <- Falso
        Para ok de 1 ate total faca
          Se nomes[ok] = busca Entao

            Escreval("Nome:  ", nomes[ok])
            Escreval("Cargo: ", cargos[ok])

            encontrado <- Verdadeiro
          FimSe
        FimPara
        Se nao encontrado Entao
          Escreval("Nenhum resultado para a pesquisa.")
        FimSe


      FimSe
    FimSe




    Se opcao = 3 Entao
      Se total = 0 Entao
        Escreval("Nenhum funcionario cadastrado.")
      Senao
        Para ok de 1 ate total faca
          Escreval("---")
          Escreval("Nome:     ", nomes[ok])
          Escreval("Cargo:    ", cargos[ok])
          Escreval("Salario:  ", salarios[ok])
          Escreval("Admissao: ", admissoes[ok])
        FimPara

      FimSe
    FimSe

    Se opcao = 4 Entao
      Escreval("Ate logo!")
    FimSe

    Se (opcao < 1) ou (opcao > 4) Entao
      Escreval("Opcao invalida.")
    FimSe







fimalgoritmo



```