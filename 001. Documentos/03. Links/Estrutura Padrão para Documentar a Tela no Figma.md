#### **1. Identificação da Tela**  
- **Nome da Tela**: (Ex: "Cadastro de Cliente")  
- **Versão do Protótipo**: (Ex: v1.0 - Agosto/2024)  
- **Status**: (Rascunho ✔️ | Revisado ✔️ | Validado ✔️)  
- **Link direto no Figma**: (Se aplicável)  

#### **2. Objetivo da Tela**  
- Qual é a função principal dessa tela?  
- Em qual etapa do fluxo ela se encaixa?  
- Exemplo:  
  > "Permite que o usuário cadastre um novo cliente no sistema, coletando informações básicas para posterior consulta."  

#### **3. Elementos da Interface (UI Components)**  
Liste todos os componentes visíveis na tela e suas funções:  

| **Componente**   | **Tipo**        | **Descrição/Funcionalidade**               | **Obrigatório?** |     |
| ---------------- | --------------- | ------------------------------------------ | ---------------- | --- |
| Campo "Nome"     | Input Texto     | Recebe o nome completo do cliente.         | Sim ✔️           |     |
| Botão "Salvar"   | Botão Primário  | Salva os dados e redireciona para a lista. | Sim ✔️           |     |
| Seção "Contatos" | Grupo de Campos | Agrupa e-mail e telefone.                  | Não ✖️           |     |

*(Inclua todos: inputs, botões, tabelas, modais, dropdowns, etc.)*  

#### **4. Comportamento e Interações (UX Flow)**  
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

#### **5. Dados e Requisitos**  
- **Campos e Regras**:  
  | **Campo**    | **Tipo de Dado** | **Valor Padrão** | **Regras/Máscara**       |  
  |--------------|------------------|------------------|--------------------------|  
  | Nome         | Texto            | -                | Máx. 100 caracteres      |  
  | Telefone     | Número           | -                | Formato (XX) XXXXX-XXXX  | 
- **Dados dinâmicos**:  
  - Se a tela exibe uma tabela, descreva a origem dos dados (Ex: "Lista busca da API `/clientes`").  

#### **6. Observações e Limitações do Protótipo**  
- Itens **não funcionais** no Figma (Ex: "O dropdown de 'Estado' não tem interação real").  
- Itens **abstraídos** (Ex: "Validação de CPF não foi incluída no protótipo, mas será implementada no desenvolvimento").  
- **Dependências**:  
  > "Esta tela presume que o backend já terá a API de cadastro pronta."  

#### **7. Screenshots e Anotações Visuais**  
- Incluir imagem da tela no Figma (com anotações se necessário).  
- Exemplo:  
  > ![Tela de Cadastro](link_ou_imagem)  
  > *Legenda: "Botão 'Voltar' retorna à lista sem salvar alterações."*  

---

### **Exemplo Prático (Documentação da Tela "Login")**  

#### **1. Identificação da Tela**  
- **Nome**: Login  
- **Versão**: v2.1  
- **Status**: Validado ✔️  
- **Link no Figma**: [https://figma.com/...](...)  

#### **2. Objetivo**  
> "Autenticar usuários no sistema mediante e-mail e senha válidos."  

#### **3. Elementos da Interface**  
| **Componente**       | **Tipo**          | **Descrição**                                  |  
|----------------------|-------------------|-----------------------------------------------|  
| Campo "E-mail"       | Input Texto       | Recebe o e-mail do usuário.                   |  
| Campo "Senha"        | Input Password    | Senha com toggle para mostrar/ocultar.        |  
| Botão "Entrar"       | Botão Primário    | Aciona o login. Desabilitado se campos vazios.|  

#### **4. Comportamento**  
- **Validações**:  
  - Mensagem de erro se e-mail não for válido.  
  - Após 3 tentativas falhas, exibe link "Esqueci minha senha".  
- **Fluxo**:  
  - Sucesso: Redireciona para a dashboard.  
  - Falha: Exibe toast "Credenciais inválidas".  

#### **5. Dados**  
| **Campo** | **Tipo**  | **Regras**               |  
|-----------|-----------|--------------------------|  
| E-mail    | Texto     | Formato "user@domain.com"|  
| Senha     | Texto     | Mín. 6 caracteres        |  

#### **6. Observações**  
- "O protótipo não simula delay de carregamento após clicar em 'Entrar'."  
- "Link 'Criar conta' redireciona para outra tela (não prototipada ainda)."  

---

### **Dicas para Padronização**  
1. **Use templates** (como tabelas acima) para manter consistência entre telas.  
2. **Inclua versão do Figma** para rastrear mudanças.  
3. **Adicione um glossário** se usar termos técnicos (ex: "Toast = notificação temporária").  

Essa estrutura garante que sua documentação seja:  
- **Clara** (qualquer pessoa entende a tela).  
- **Completa** (cobre UI, UX e regras).  
- **Pronta para comparação** (basta adicionar uma coluna com o sistema legado depois).  

Quer ajustar algo ou incluir outros tópicos?