# Trabalhos-da-faculdade
First university assignment - simple produce market system in C language
Sistema de Gestão de Estoque e Vendas

O sistema de gestão de estoque e vendas é um programa desenvolvido em linguagem C que visa facilitar o gerenciamento de estoque e vendas de uma loja de frutas e produtos lácteos. O sistema oferece uma interface intuitiva e fácil de usar, permitindo que os usuários realizem diversas operações.

Funcionalidades do Sistema

O sistema apresenta as seguintes funcionalidades:

1. Mostrar Estoque: Exibe a lista de produtos com seus respectivos preços, quantidades em estoque e tipo de preço (por kg ou unidade).
2. Registrar Entrada de Produtos: Permite adicionar novos produtos ao estoque ou atualizar quantidades de produtos existentes.
3. Processar Venda: Realiza vendas, atualiza o estoque e emite nota fiscal.
4. Emitir Relatório de Reposição: Gera um relatório com produtos que precisam ser reabastecidos com base em um limite mínimo de estoque definido.
5. Emitir Relatório do Dia: Gera um relatório com as vendas realizadas no dia, incluindo o total recebido por método de pagamento.

Funcionalidades do Sistema

O sistema apresenta as seguintes funcionalidades:

1. Mostrar Estoque: Exibe a lista de produtos com seus respectivos preços, quantidades em estoque e tipo de preço (por kg ou unidade).
2. Registrar Entrada de Produtos: Permite adicionar novos produtos ao estoque ou atualizar quantidades de produtos existentes.
3. Processar Venda: Realiza vendas, atualiza o estoque e emite nota fiscal.
4. Emitir Relatório de Reposição: Gera um relatório com produtos que precisam ser reabastecidos com base em um limite mínimo de estoque definido.
5. Emitir Relatório do Dia: Gera um relatório com as vendas realizadas no dia, incluindo o total recebido por método de pagamento.

Demonstração do Funcionamento

Para demonstrar o funcionamento do sistema, vamos realizar algumas operações:

1. Iniciar o programa e selecionar a opção "Mostrar Estoque" para visualizar a lista de produtos. Nesse momento, o sistema utiliza a variável produtos para armazenar a lista de produtos e a função mostrarEstoque() para exibir os dados.


void mostrarEstoque(Produto* produtos[], int tamanho) {
 printf("\nTECFFRUIT\n");
 printf("| Produto | Preco (R$) | Estoque (Kg) | Estoque (Unidade) | Tipo Preco |\n");
 printf("|----------|------------|--------------|-------------------|-------------|\n");
 for (int i = 0; i < tamanho; i++) {
     // ...
 }
}


2. Selecionar a opção "Registrar Entrada de Produtos" para adicionar um novo produto ao estoque. Aqui, o sistema utiliza a variável produtoEscolhido para armazenar o produto selecionado e a função registrarEntradaProduto() para atualizar o estoque.


void registrarEntradaProduto(Produto* produtos[], int* tamanho) {
 // ...
 Produto* produtoEscolhido = NULL;
 // ...
 produtoEscolhido->quantidadeEstoqueKg += peso;
 produtoEscolhido->quantidadeEstoqueUnidade += unidades;
 // ...
}


3. Selecionar a opção "Processar Venda" para realizar uma venda e emitir nota fiscal. Nesse caso, o sistema utiliza a variável totalGeral para calcular o total da venda e a função gerarNotaFiscal() para emitir a nota fiscal.


void gerarNotaFiscal(int numeroSerie, Produto* produtos[], int tamanho, float totalGeral, const char* metodoPagamento) {
 // ...
 fprintf(arquivo, "Total Geral: R$%.2f\n", totalGeral);
 // ...
}


4. Selecionar a opção "Emitir Relatório de Reposição" para gerar um relatório de produtos que precisam ser reabastecidos. Aqui, o sistema utiliza a variável MIN_QUANTIDADE_ESTOQUE para definir o limite mínimo de estoque.


#define MIN_QUANTIDADE_ESTOQUE 10


5. Selecionar a opção "Emitir Relatório do Dia" para gerar um relatório das vendas realizadas no dia. Nesse momento, o sistema utiliza a variável totalDinheiro para calcular o total recebido em dinheiro.


float totalDinheiro = 0.0;

Vantagens do Sistema

- Facilita o gerenciamento de estoque e vendas
- Otimiza a eficiência e produtividade da loja
- Fornece relatórios detalhados sobre as vendas e estoque
- Permite a emissão de notas fiscais
- É fácil de usar e intuitivo

