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
6. **Revise + Crie** → Clique em **"Criar"**.  
