# 💼 Treinamento MS-102 – Administração do Microsoft 365

Este repositório contém as **atividades práticas** realizadas durante o treinamento MS-102, com foco na administração de usuários, grupos, licenças, políticas e automações no Microsoft 365.

---

## 📚 Atividades Semanais

### ✅ 1. Criar 5 usuários com atributos personalizados

**Objetivo:** Aprender a criar usuários diretamente no portal Microsoft 365.

**Lógica:** Utilizar nomes consistentes (naming convention), atribuindo UPNs e senhas seguras.

---

### ✅ 2. Criar usuários e grupos em massa com PowerShell via CSV

**Objetivo:** Automatizar tarefas administrativas em escala.

**Lógica:** Utilizamos `Import-Csv` e `New-MsolUser` ou `New-AzADUser` em scripts PowerShell. Os dados são lidos de um arquivo `usuarios.csv`.

---

### ✅ 3. Criar 3 grupos

**Tipos de Grupos:**
- **Segurança:** Para permissões.
- **Microsoft 365:** Para colaboração em Teams.
- **Distribuição:** Para envio de emails em massa.

**Lógica:** Criados via portal e PowerShell, conforme o uso planejado.

---

### ✅ 4. Configurar domínio personalizado (Cloudns)

**Objetivo:** Adicionar domínio próprio à organização.

**Lógica:** Criado domínio gratuito em [Cloudns.net](https://cloudns.net), DNS TXT adicionado e validado no portal Microsoft 365.

---

### ✅ 5. Atribuir licenças a 3 usuários

**Objetivo:** Gerenciar assinaturas.

**Lógica:** Atribuição feita manualmente via portal e via PowerShell com `Set-MsolUserLicense`.

---

### ✅ 6. Criar uma Unidade Administrativa (UA)

**Objetivo:** Delegar tarefas administrativas com escopo reduzido.

**Lógica:** Criada UA e atribuída função de "User Administrator" a um usuário dentro dela.

---

### ✅ 7. Definir Naming Convention

**Objetivo:** Padronizar criação de usuários e grupos.

**Lógica:** Convenção aplicada:
- Usuários: `nome.sobrenome@dominio.com`
- Grupos: `GRP_Funcao_Local`

---

### ✅ 8. Política de expiração de senha personalizada

**Objetivo:** Gerenciar segurança de identidade.

**Lógica:** Criada política com 180 dias de validade e aplicada ao grupo de usuários.

---

### ✅ 9. Habilitar Self-Service Password Reset (SSPR)

**Objetivo:** Reduzir suporte técnico e aumentar a autonomia dos usuários.

**Lógica:** SSPR ativado para todos os usuários no portal Entra ID > Autenticação > SSPR.

---

### ✅ 10. Script PowerShell para listar todos os grupos e membros

**Objetivo:** Obter visão organizacional da estrutura de grupos.

**Lógica:** Criado script que usa `Get-AzureADGroup` e `Get-AzureADGroupMember`.

Arquivo: [`scripts/listar-grupos-membros.ps1`](./scripts/listar-grupos-membros.ps1)

---

## 🖼 Evidências Visuais

As capturas de tela estão na pasta [`evidencias`](./evidencias).

---

## 📄 Documentação

O relatório completo com imagens e explicações está disponível em:

📁 [`documentacao/MS102_Atividades.pdf`](./documentacao/MS102_Atividades.pdf)

---

## 🧠 Autor

**Instrutor:** Manuel Miguel  
**GitHub:** [@tmm1884](https://github.com/tmm1884)

---

