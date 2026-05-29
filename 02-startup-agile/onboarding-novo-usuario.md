# Módulo 02 — Onboarding do Novo Usuário

> **Escopo:** Guia de primeiros passos para novos usuários de plataforma SaaS B2B.
> **Objetivo:** Reduzir o Time-to-Value (TTV) para menos de 15 minutos e minimizar tickets de suporte de nível 1.
> **Público-alvo:** Novos usuários finais, gestores de equipe, time de Customer Success.
> **Versão:** 1.0.0 | **Última atualização:** 2026-05-29 | **Owner:** Alexandre Claudino

---

## 🎯 O que você vai conquistar em 15 minutos

Ao final deste guia, você terá:

✅ Criado sua conta e configurado a autenticação em dois fatores (2FA)  
✅ Conectado sua fonte de dados principal (planilha, banco ou API)  
✅ Visualizado seu primeiro dashboard com métricas em tempo real  
✅ Compartilhado o acesso com um colega de equipe  

> [!TIP]
> **Time-to-Value (TTV)** é o tempo entre você criar a conta e extrair o primeiro insight acionável do produto. Quanto menor o TTV, maior a probabilidade de adoção contínua.

---

## 🚀 Passo a Passo

### Passo 1 — Crie sua conta (2 minutos)

1. Acesse [app.nomedaproduto.com/cadastro](https://app.nomedaproduto.com/cadastro).
2. Preencha seu e-mail corporativo e defina uma senha segura.
3. Confirme seu e-mail clicando no link enviado para sua caixa de entrada.

> [!IMPORTANT]
> Utilize **sempre** seu e-mail corporativo. Contas criadas com e-mails pessoais (Gmail, Yahoo, etc.) não terão acesso aos recursos de colaboração em equipe e relatórios avançados.

---

### Passo 2 — Ative a Autenticação em Dois Fatores (2FA) (3 minutos)

A segurança dos seus dados é prioridade. A 2FA é **obrigatória** para todos os usuários.

1. No canto superior direito, clique em seu avatar → **Configurações de Segurança**.
2. Clique em **Ativar 2FA**.
3. Escaneie o QR Code com seu aplicativo autenticador (Google Authenticator, Authy ou Microsoft Authenticator).
4. Digite o código de 6 dígitos gerado pelo app para confirmar.

> [!WARNING]
> **Não perca seu dispositivo autenticador.** Se você perder o acesso, a recuperação de conta exigirá contato direto com o time de segurança e pode levar até 48 horas úteis.

---

### Passo 3 — Conecte sua primeira fonte de dados (5 minutos)

A plataforma aceita três tipos de entrada. Escolha a que melhor se adequa ao seu cenário:

| Tipo de Fonte | Ideal para | Tempo estimado | Pré-requisito |
|:---|:---|:---|:---|
| **Planilha (CSV/Excel)** | Análises pontuais, dados históricos | 2 minutos | Arquivo com no máximo 100.000 linhas |
| **Banco de Dados** | Dashboards em tempo real, pipelines recorrentes | 4 minutos | Credenciais de acesso (host, porta, usuário, senha) |
| **API REST** | Integrações com sistemas próprios ou terceiros | 5 minutos | URL do endpoint + token de autenticação |

#### Para Planilhas:
1. Clique em **Nova Fonte de Dados** → **Upload de Arquivo**.
2. Arraste seu arquivo ou clique para selecionar.
3. Revise a pré-visualização das colunas e confirme os tipos de dados (texto, número, data).
4. Clique em **Importar**.

#### Para Banco de Dados:
1. Clique em **Nova Fonte de Dados** → **Banco de Dados**.
2. Selecione o tipo (PostgreSQL, MySQL, SQL Server, BigQuery).
3. Preencha as credenciais de conexão.
4. Teste a conexão e salve.

> [!NOTE]
> As credenciais são criptografadas com AES-256 e nunca expostas na interface. Mesmo administradores da plataforma não conseguem visualizar suas senhas.

---

### Passo 4 — Visualize seu primeiro dashboard (3 minutos)

Com os dados importados, a plataforma gera automaticamente um dashboard sugerido com base no tipo de dados detectado.

1. Clique em **Dashboards** no menu lateral.
2. Selecione o dashboard sugerido (rótulo: **Sugerido para você**).
3. Explore os widgets interativos — passe o mouse sobre os gráficos para ver detalhes.
4. (Opcional) Clique em **Personalizar** para ajustar cores, filtros e períodos.

> [!TIP]
> Dashboards podem ser exportados em PDF ou PNG para apresentações executivas. Use o ícone ⬇️ no canto superior direito de cada widget.

---

### Passo 5 — Convide um membro da equipe (2 minutos)

A colaboração amplifica o valor da plataforma.

1. Vá em **Configurações** → **Membros da Equipe**.
2. Clique em **Convidar membro**.
3. Insira o e-mail corporativo do colega e defina o nível de permissão:

| Permissão | O que pode fazer | Quem deve ter |
|:---|:---|:---|
| **Administrador** | Gerenciar fontes de dados, convidar membros, alterar configurações de segurança | Gestores de produto / TI |
| **Editor** | Criar e editar dashboards, compartilhar visualizações | Analistas de dados, operadores |
| **Visualizador** | Apenas visualizar dashboards compartilhados | Stakeholders executivos, clientes |

4. O convidado receberá um e-mail com link de ativação válido por 24 horas.

---

## ❓ Perguntas Frequentes (FAQ)

> **Dúvidas que desoneram o time de Customer Success e aceleram sua autonomia.**

**P: Esqueci minha senha. Como recupero?**  
**R:** Na tela de login, clique em **Esqueci minha senha**. Você receberá um link de redefinição válido por 1 hora. Se não receber em 5 minutos, verifique sua caixa de spam.

---

**P: Posso alterar meu e-mail de acesso?**  
**R:** Sim. Acesse **Configurações** → **Perfil** → **Alterar e-mail**. Será necessário confirmar o novo e-mail e reautenticar sua sessão.

---

**P: Meu arquivo CSV tem 500.000 linhas. Posso fazer upload?**  
**R:** Planilhas acima de 100.000 linhas devem ser carregadas via **Banco de Dados** ou **API** para garantir performance. Entre em contato com nosso time de suporte para orientação de arquitetura.

---

**P: O dashboard sugerido não faz sentido para meus dados. E agora?**  
**R:** O algoritmo de sugestão funciona melhor com dados tabulares estruturados. Se seus dados forem não estruturados (texto livre, JSON aninhado), recomendamos criar um dashboard do zero usando nosso **Builder Visual**. Acesse **Dashboards** → **Criar do zero**.

---

**P: Como cancelo minha conta?**  
**R:** Acesse **Configurações** → **Conta** → **Encerrar conta**. Seus dados serão excluídos permanentemente em até 30 dias, conforme nossa Política de Privacidade e LGPD.

---

**P: Preciso de ajuda além deste guia.**  
**R:** Nosso time de Customer Success está disponível via:
- 💬 Chat ao vivo (dentro da plataforma, ícone no canto inferior direito)
- 📧 E-mail: [suporte@nomedaproduto.com](mailto:suporte@nomedaproduto.com)
- 📚 Base de conhecimento completa: [help.nomedaproduto.com](https://help.nomedaproduto.com)

---

## ✅ Checklist de Conclusão

Marque cada item conforme você avança:

- [ ] Conta criada com e-mail corporativo
- [ ] 2FA ativada e backup de recuperação salvo
- [ ] Primeira fonte de dados conectada e validada
- [ ] Dashboard visualizado e personalizado
- [ ] Pelo menos 1 membro da equipe convidado

> **Parabéns!** Você está pronto para extrair valor da plataforma. O próximo passo recomendado é explorar nossos [Templates de Dashboard por Indústria](https://help.nomedaproduto.com/templates).

---

> **Documento versionado via Git.** Última revisão por: Alexandre Claudino | Technical Writer Sênior
> 
> *Este guia é atualizado continuamente. Para sugerir melhorias, abra uma Issue neste repositório.*
