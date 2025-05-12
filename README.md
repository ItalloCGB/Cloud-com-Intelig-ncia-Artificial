# 📚 Resumos & Dicas sobre Máquinas Virtuais no Azure  

Este repositório contém anotações simplificadas e dicas práticas para quem está começando com **Microsoft Azure**, especialmente focado em **Máquinas Virtuais (VMs)**.  

---

## 🚀 **Como Criar uma VM no Azure (Passos Básicos)**  
Siga o [guia oficial da Microsoft](https://docs.microsoft.com/pt-br/azure/virtual-machines/windows/quick-create-portal):  

1. **Acesse o [Portal Azure](https://portal.azure.com)** → Faça login.  
2. **Criar um recurso** → Busque por "Máquina Virtual" → Clique em **"Criar"**.  
3. **Preencha os dados básicos**:  
   - **Assinatura**: Selecione sua conta (Free Tier, se disponível).  
   - **Grupo de recursos**: Crie um novo (ex: `MeuGrupoVM`).  
   - **Nome da VM**: Ex: `MinhaVM-Windows`.  
   - **Região**: Escolha a mais próxima (ex: *Brasil Sul*).  
   - **Imagem**: Selecione o OS (ex: *Windows Server 2022*).  
   - **Tamanho**: Para testes, use **B1s** (econômico).  
4. **Credenciais de acesso**:  
   - **Usuário**: `adminuser` (não use "admin" puro).  
   - **Senha**: Defina uma senha forte.  
5. **Portas de entrada**:  
   - Habilite **RDP (3389)** se for acessar remotamente (apenas para testes!).  
6. **Revise + Crie** → Clique em **"Criar"**


# 🗃️ Laboratório Azure: Configuração de Banco de Dados SQL

## 🔧 Configuração Passo a Passo

### 1. Acesso Inicial
- Acessar o [Portal Azure](https://portal.azure.com)
- Verificar assinatura ativa (Free Tier recomendado)

### 2. Criação do Banco de Dados
1. "Criar um recurso" > "Bancos de Dados" > "SQL Database"
2. Configurações básicas:
   - Grupo de recursos: novo (ex: 'lab-db-group')
   - Nome do banco: 'meu-banco-lab'
   - Servidor: novo (anote usuário e senha!)
   - Localização: Brasil Sul
   - Camada de preço: Básico
3. Revisar e criar

+ IMPORTANTE: Habilitar "Permitir acesso a serviços do Azure"
+ Adicionar IP atual nas regras de firewall

🛡️ Melhores Práticas
Área	Recomendação
Segurança	Usar autenticação do Azure Active Directory
Custos	Configurar alertas de gastos na assinatura
Backup	Habilitar retenção automática (7 dias mínimo)


💡 Dica: Use o Azure CLI para automação:
az sql db create --name MeuBanco --resource-group MeuGrupo  
