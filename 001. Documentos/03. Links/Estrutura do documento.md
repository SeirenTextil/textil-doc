tags: #template 
Link: [[Documentação Cartão Instrução]]
### **Estrutura Sugerida para a Documentação**  

#### **1. Introdução**  
- **Objetivo**: Explicar o propósito do documento (comparar o sistema legado com o protótipo no Figma).  
- **Escopo**: Listar quais telas serão documentadas.  
- **Público-alvo**: Quem deve ler este documento (desenvolvedores, designers, PO, etc.).  

#### **2. Metodologia de Comparação**  
- Como a comparação será feita (critérios usados, como funcionalidades, fluxos, dados, interações).  
- Legenda de status (ex: "✅ Implementado no Figma", "❌ Removido no protótipo", "⚠️ Abstraído/Simplificado").  

#### **3. Padrão de Documentação por Tela** *(Repetir para cada tela)*  

##### **1. Identificação da Tela**

- **Nome da Tela**: (Ex: "Cadastro de Cliente")
- **Versão do Protótipo**: (Ex: v1.0 - Agosto/2024)
- **Status**: (Rascunho ✔️ | Revisado ✔️ | Validado ✔️)
- **Link direto no Figma**: (Se aplicável)

##### **2. Objetivo da Tela**

- Qual é a função principal dessa tela?
- Em qual etapa do fluxo ela se encaixa?
- Exemplo:
    
    > "Permite que o usuário cadastre um novo cliente no sistema, coletando informações básicas para posterior consulta."
    

##### **3. Elementos da Interface (UI Components)**

Liste todos os componentes visíveis na tela e suas funções:

|**Componente**|**Tipo**|**Descrição/Funcionalidade**|**Obrigatório?**||
|---|---|---|---|---|
|Campo "Nome"|Input Texto|Recebe o nome completo do cliente.|Sim ✔️||
|Botão "Salvar"|Botão Primário|Salva os dados e redireciona para a lista.|Sim ✔️||
|Seção "Contatos"|Grupo de Campos|Agrupa e-mail e telefone.|Não ✖️||

_(Inclua todos: inputs, botões, tabelas, modais, dropdowns, etc.)_

##### **4. Comportamento e Interações (UX Flow)**

Descreva como o usuário interage com a tela:

- **Fluxo de entrada**: Como se chega a essa tela? (Ex: "Clicar em 'Novo Cliente' na dashboard").
- **Fluxo de saída**: O que acontece após ações principais? (Ex: "Ao clicar em 'Salvar', redireciona para a lista de clientes").
- **Validações**:
    - "O campo 'E-mail' exibe erro se não estiver no formato válido."
    - "Botão 'Salvar' só é habilitado quando todos os campos obrigatórios estão preenchidos."
- **Estados da tela**:
    - Vazia (sem dados)
    - Preenchida (com dados de exemplo)
    - Erro (validação falhou)

##### **5. Dados e Requisitos**

- **Campos e Regras**:

|**Campo**|**Tipo de Dado**|**Valor Padrão**|**Regras/Máscara**||
|---|---|---|---|
|Nome| Texto|-|Máx. 100 caracteres||
|Telefone|Número|-|Formato (XX) XXXXX-XXXX||

- **Dados dinâmicos**:
    - Se a tela exibe uma tabela, descreva a origem dos dados (Ex: "Lista busca da API `/clientes`").

##### **6. Observações e Limitações do Protótipo**

- Itens **não funcionais** no Figma (Ex: "O dropdown de 'Estado' não tem interação real").
- Itens **abstraídos** (Ex: "Validação de CPF não foi incluída no protótipo, mas será implementada no desenvolvimento").
- **Dependências**:
    
    > "Esta tela presume que o backend já terá a API de cadastro pronta."
    

##### **7. Screenshots e Anotações Visuais**

- Incluir imagem da tela no Figma (com anotações se necessário).
- Exemplo:
    
    > “link_ou_imagem” is not created yet. Click to create.  
    > _Legenda: "Botão 'Voltar' retorna à lista sem salvar alterações."_

#### **4. Conclusão**  
- Resumo das principais mudanças.  
- Próximos passos (o que ainda precisa ser validado ou ajustado no protótipo).  

---  

### **Exemplo Prático (Modelo para uma Tela de "Cadastro de Cliente")**  

#### **3.1. Tela de Cadastro de Cliente**  
- **Objetivo**: Registrar novos clientes no sistema.  
- **Contexto**: Acessada a partir do menu principal → "Clientes" → "Novo Cadastro".  

| **Item**            | **Sistema Antigo**               | **Protótipo Figma**          | **Diferenças/Justificativas** |  
|---------------------|----------------------------------|-----------------------------|------------------------------|  
| **Campos**          | Nome, CPF, Telefone, Endereço... | Nome, E-mail, Telefone      | CPF e Endereço removidos (serão em outra etapa) |  
| **Tabelas**         | Histórico de compras visível    | Não incluído                | Será em uma tela separada    |  
| **Botões**          | "Salvar", "Cancelar", "Imprimir"| "Salvar", "Voltar"          | "Imprimir" removido (pouco uso) |  
| **Validações**      | CPF obrigatório                 | E-mail obrigatório          | Foco em contato digital      |  

**Observações**:  
- O Figma não tem a validação em tempo real (será implementada no front).  
- O botão "Imprimir" pode ser reintroduzido se houver demanda.  

---  

### **Dicas para Padronizar entre Telas**  
1. **Mantenha a mesma tabela de comparação** para todas as telas.  
2. **Use ícones/cores** para destacar status (✅❌⚠️).  
3. **Inclua screenshots** lado a lado (VBA vs. Figma) para referência visual.  
4. **Adicione um glossário** se houver termos técnicos específicos.  

Se precisar de mais detalhes ou um template em formato DOCX/Google Docs, posso ajudar a elaborar!
