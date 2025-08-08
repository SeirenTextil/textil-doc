# 01. Introdução
## Objetivo
O objetivo deste documento é mostrar como está funcionando a disposição dos campos do cartão instrução. Será abordado e comparado as funcionalidades do sistema antigo com o novo.
Sua utilização é para consultar e servir de instrução de uso de ambos sistemas.
## Escopo
será documentada e instruída a seguir, a tela de Cartão instrução.
## Público alvo
Desenvolvedores, Lideres.

--- 
# 02. Metodologia

## Critérios de Comparação:
- localização dos itens
- Funcionalidades
- Abstração de dados
- Nova interatividade
- Legenda de implementação ✅ ou ❌
# 03. O Documento 

## **1. Identificação da Tela**

- **Nome da Tela**:  Cartão Instrução
- **Versão do Protótipo**: v1.0 Agosto/2025
- **Status**: #Rascunho
- **Link direto no Figma**:  ---

## **2. Objetivo da Tela**

- Qual é a função principal dessa tela?
> 	Permite que o usuário visualize o cartão instrução do produto escolhido.
- Em qual etapa do fluxo ela se encaixa?
> 	Inicio do fluxo, montagem do cartão (Importa Romaneio > Criação Cartão > Visualização Cartão Instrução )
## **3. Elementos da interface (UI Components)**

Lista de todos os componentes visíveis na tela e suas funções:  

| **Componente**               | **Tipo**            | **Descrição/Funcionalidade**                              | **Obrigatório?** |
| ---------------------------- | ------------------- | --------------------------------------------------------- | ---------------- |
| Campo "Cartão"               | Visual - PartNumber | Visualiza e copia o Núm. do Cartão                        | Sim ✔️           |
| Campo "Largura Cru"          | Visual - Metragem   | Visualiza Largura **Crua** do tecido                      | Sim ✔️           |
| Campo "Largura Solicitada"   | Visual - Metragem   | Visualiza Largura **Solicitada** do tecido                | Sim ✔️           |
| Campo "Largura Real"         | Visual - Metragem   | Visualiza Largura **Real** do tecido                      | Sim ✔️           |
| Campo "Divisão"              | Visual - Tipo       | Visualiza a Divisão do tecido (CXT, TXT)                  | Sim ✔️           |
| Campo "Composição"           | Visual - Tipo       | Visualiza a Composição do tecido (PES)                    | Sim ✔️           |
| Campo "Gramatura DataColor"  | Visual - Metragem   | Visualiza a Gramatura do DataColor                        | Sim ✔️           |
| Campo "gramatura Cru"        | Visual - Metragem   | Visualiza a Gramatura Cru                                 | Sim ✔️           |
| Campo "gramatura Solicitada" | Visual - Metragem   | Visualiza a Gramatura Solicitada                          | Sim ✔️           |
| Campo "gramatura Rama"       | Visual - Metragem   | Visualiza a Gramatura Rama                                | Sim ✔️           |
| Campo "Cor"                  | Visual - Cor        | Visualiza a Cor e seu Cód. Solicitado                     | Sim ✔️           |
| Campo "Localização Atual"    | Visual - Estado     | Visualiza o fluxo/Localização atual do cartão             | Sim ✔️           |
| Botão "Localizar"            | Botão               | Vai para a aba de localização de cartões                  | Não ❌            |
| Botão "Compartilhar"         | Botão               | Compartilha Cartão                                        | Não ❌            |
| Botão "Lista de Peças"       | Botão               | Exibe tabela de peças e suas especificações               | Sim ✔️           |
| Botão "Pós Tinto"            | Botão               | Exibe tabela de pós tinto das peças                       | Sim ✔️           |
| Botão "Máq. Lote"            | Botão               | Exibe tabela de Máq. Lotes                                | Sim ✔️           |
| Interação "Estoque"          | Fluxo de endereço   | Exibe um fluxo dos caminhos                               | Sim ✔️           |
| Campo "Cliente"              | Botão               | Ao Clicar no "@" do cliente, exibe informações sobre ele. | Sim ✔️           |


## **4. Comportamento e Interações (UX Flow)**
- Fluxo de Entrada: Como se chega a essa tela?
	> No menu Lateral esquerdo, clicar em "Cartão Instrução" Abrirá a página.
- Fluxo de saída: O que acontece após ações principais?
	> Visualiza campos, Copia Cód. Cartão e compartilha Cartão.
- Validações:
	- Componente Cartão Instrução não altera/edita dados.
- Estados da Tela:
	-  Estados que a tela pode estar: vazia, Preenchida, Erro (com Cód. erro possível. ex: 500)
## **5.  Dados e requisitos**

- Campos e Regras:

| **Campo**              | **Tipo de Dado**  | **Valor Padrão** | **Regras/Máscara** |
| ---------------------- | ----------------- | ---------------- | ------------------ |
| Botão "Localizar"      | Botão             | -                | -                  |
| Botão "Compartilhar"   | Botão             | -                | -                  |
| Botão "Lista de Peças" | Botão             | -                | -                  |
| Botão "Pós Tinto"      | Botão             | -                | -                  |
| Botão "Máq. Lote"      | Botão             | -                | -                  |
| Interação "Estoque"    | Fluxo de endereço | -                | -                  |
| Campo "Cliente"        | Botão             | -                | -                  |


## **6. Observações e Limitações do Protótipo**

- Itens **Não Funcionais**: 
	- O campo "Cor" não tem interação real
- Itens Abstraídos:
	- O campo "Novo/Consulta" do Cartão Instrução Legado foi abstraído.
- Dependências: 
	- Essa tela presume que o cartão já está formado/feito.
## **7. Screenshots e Anotações Visuais.**

Na Imagem abaixo é possível visualizar o conteúdo inicial do cartão instrução.
![[01. Imagem Tela Cartão Novo.png]]
*Figura 1: Pagina Cartão Instrução*

Na imagem abaixo refere-se sobre os campos de visualização e interação do cartão, onde conterá as informações principais. 
![[03. Imagem Cartão Instrução Novo.png]]
*Figura 2: Campo de especificações do Cartão Instrução*

Na imagem abaixo consta a tabela com a Lista de Peças, podendo alternar entre: Pós Tinto e Máq. Lote
![[05. Imagem Tabela Cartão Instrução Novo.png]]*Figura 3: Campo/Tabela Lista de Peças *

# 04. Conclusão
## **Resumo principais mudanças.**
Foi reformulado totalmente a tela Cartão instrução comparado com o sistema legado. Deixando com o aspecto visual mais atraente e intuitivo, abstraindo itens desnecessários ou em lugares errados. 
## **Próximos passos.**
- Validação do documento
- Validação da Tela Cartão instrução.