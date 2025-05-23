# 💻 Resumo do Lab - Criação de Máquina Virtual na Azure

Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do lab na plataforma DIO, cujo tema foi a **criação de uma Máquina Virtual (VM) na Microsoft Azure**. Durante o laboratório, percorremos todas as etapas essenciais para configurar uma VM na nuvem, com ênfase especial na etapa **Básico**, onde se concentram as configurações fundamentais da máquina virtual.

---

## 🧠 Etapas e Conceitos Aprendidos

### 🔹 1. Básico (Foco Principal)

A etapa "Básico" foi o coração do laboratório. Aqui estão os principais pontos explorados:

- **Assinatura**  
  Selecionamos qual conta de cobrança seria usada para provisionar os recursos da Azure.

- **Grupo de Recursos (Resource Group)**  
  Criamos ou reutilizamos um agrupamento lógico de recursos, facilitando a organização, gerenciamento e automação.

- **Nome da Máquina Virtual**  
  Escolhemos um nome significativo e único dentro do grupo de recursos. Exemplo: `vm-lab-dio`.

- **Região (Region)**  
  Selecionamos o data center onde a VM seria criada. A escolha da região impacta diretamente na latência, disponibilidade e preço.  
  Exemplo: `Brazil South` ou `East US`.

- **Disponibilidade (Availability options)**  
  Analisamos opções como:
  - Nenhuma (padrão)
  - Conjuntos de disponibilidade (para alta disponibilidade local)
  - Zonas de disponibilidade (para redundância entre datacenters)

- **Imagem do SO (Image)**  
  Escolhemos o sistema operacional que seria instalado na VM:
  - Windows Server (diversas versões)
  - Ubuntu, Debian, CentOS (para VMs Linux)
  - Custom images (se aplicável)

- **Tamanho da VM (Size)**  
  Escolhemos a configuração de hardware da VM com base no uso previsto:
  - Número de vCPUs (núcleos virtuais)
  - Memória RAM  
  Exemplo: `Standard B1s` (uso geral, baixo custo) ou `D2s_v3` (desempenho intermediário)

- **Conta Administrativa**  
  Definimos o método de autenticação:
  - Nome de usuário e senha (Windows/Linux)
  - Chave pública SSH (Linux)

- **Portas de Entrada (Inbound Ports)**  
  Selecionamos quais portas seriam abertas para acesso externo à VM:
  - RDP (porta 3389) para acesso remoto a VMs Windows
  - SSH (porta 22) para acesso remoto a VMs Linux
  - Nenhuma (para ambientes fechados ou acessos internos)

Essa etapa foi crucial para o sucesso da configuração, pois define as bases da VM, segurança inicial e compatibilidade com os demais recursos da nuvem.

---

### 💽 2. Discos

Exploramos os diferentes tipos de armazenamento disponíveis:
- Disco do SO (geralmente SSD).
- Opção de adicionar discos de dados.
- Tipos de disco: **Premium SSD**, **Standard SSD** e **Standard HDD**.
- Configuração do cache e criptografia.

---

### 🌐 3. Rede

Configuramos:
- A criação de uma **rede virtual (VNet)** e **sub-rede**.
- O **IP público**, **grupo de segurança de rede (NSG)** e regras de entrada.
- A atribuição automática ou manual de endereços IP.

---

### 🔧 4. Gerenciamento

Definimos:
- Opções de **monitoramento e diagnóstico**.
- Habilitação do **Auto-shutdown**.
- Configurações de backup e recuperação.

---

### 📊 5. Monitoramento

- Ativação de logs e métricas via Azure Monitor.
- Utilização de alertas e visualizações no portal.
- Integração com Log Analytics.

---

### ⚙️ 6. Avançado

- Inserção de scripts de inicialização.
- Integração com **domínio Active Directory**.
- Habilitação de **identidade gerenciada**.

---

### 🏷️ 7. Marcas (Tags)

- Adicionamos **tags** para facilitar organização e controle de custos.  
  Exemplo: `Projeto=LabAzure`, `Ambiente=Teste`.

---

### ✅ 8. Revisar + Criar

- Revisamos todas as configurações.
- A plataforma validou as opções escolhidas.
- Clicamos em **"Criar"** para provisionar a máquina virtual.

---

## 🚀 Conclusão

Este lab foi essencial para compreender, na prática, como provisionar uma máquina virtual na Azure, com forte ênfase na etapa "Básico", que define toda a fundação da configuração. O exercício reforçou a importância do planejamento de recursos, segurança e performance no ambiente de nuvem.


