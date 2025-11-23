# 💡 Visão Geral do Projeto – Microsoft Graph + IA  
Bootcamp CAIXA – Inteligência Artificial na Prática (DIO + Microsoft)

Este repositório reúne experimentos, consultas e aprendizados realizados durante o Bootcamp “Inteligência Artificial na Prática”, promovido pela CAIXA, Microsoft e DIO.  
O objetivo principal é registrar o uso do **Microsoft Graph Explorer**, armazenar respostas da API (anonimizadas) e consolidar boas práticas de documentação, versionamento e integração entre **Microsoft Graph + IA + Microsoft 365**.

---

## 🎯 Objetivos do Repositório
- Demonstrar domínio operacional do **Microsoft Graph Explorer**  
- Documentar cada requisição e sua resposta em **JSON**  
- Criar um histórico organizado de consultas para referência futura  
- Consolidar práticas de versionamento com **Git + GitHub**  
- Criar uma base sólida para projetos futuros envolvendo **IA + Microsoft 365 + Microsoft Graph**

---

## 🧪 Consultas Realizadas no Microsoft Graph

As consultas executadas incluíram:

- `GET /v1.0/me` — Informações básicas do usuário (`User.Read`)
- `GET /beta/me/profile` — Perfil detalhado (endpoint beta)
- `GET /v1.0/me/messages` — Mensagens de e-mail (`Mail.Read`)
- `GET /v1.0/me/mailFolders` — Pastas de e-mail (`Mail.Read`)
- `GET /v1.0/me/events` — Eventos de calendário (`Calendars.Read`)
- `GET /v1.0/me/photo` — Foto do perfil (`User.Read`)
- `GET /v1.0/me/drive/root/children` — Arquivos do OneDrive (`Files.Read`)

⚠ **Atenção:** Endpoints da rota `/beta` são experimentais e podem mudar. Evite utilizá-los em aplicações de produção.

---

## 📊 Endpoints e Escopos Necessários

| Endpoint | Descrição | Escopo mínimo |
|---------|-----------|---------------|
| `GET /v1.0/me` | Informações do usuário | User.Read |
| `GET /beta/me/profile` | Perfil detalhado (beta) | User.Read |
| `GET /v1.0/me/messages` | E-mails do usuário | Mail.Read |
| `GET /v1.0/me/mailFolders` | Pastas de e-mail | Mail.Read |
| `GET /v1.0/me/events` | Eventos do calendário | Calendars.Read |
| `GET /v1.0/me/photo` | Foto do perfil | User.Read |
| `GET /v1.0/me/drive/root/children` | Arquivos do OneDrive | Files.Read |

---

## 🚀 Como Reproduzir no Microsoft Graph Explorer

1. Acesse o **Microsoft Graph Explorer**  
2. Autentique com uma conta da sandbox **Microsoft 365 Developer Program (E5)**  
3. Em **Permissões**, conceda os escopos necessários conforme a tabela acima  
4. Informe o endpoint desejado e execute a requisição  
5. Baixe ou copie o JSON retornado  
6. **Anonimize todos os dados sensíveis**, como:  
   - nomes reais  
   - e-mails  
   - telefones  
   - IDs  
7. Salve o arquivo em `docs/responses/` usando nomes consistentes

---

## 📁 Estrutura de Diretórios

```bash
docs/
├── overview.md             # Visão geral da documentação
├── responses/              # Respostas anonimizadas das consultas Graph
│   ├── me.json
│   ├── profile_beta.json
│   ├── mailFolders.json
│   ├── events.json
│   ├── messages.json
screenshots/
└── .gitkeep                # Placeholder para capturas de tela
```

💡 **Dica:**
- Armazene todas as respostas da API em `docs/responses/`.
- Coloque evidências visuais em `screenshots/` (prints, capturas de execução etc.).

---

## 📚 Aprendizados Consolidados

- Uso prático da API **Microsoft Graph**
- Domínio de endpoints e escopos de autenticação
- Estruturação, leitura e documentação de **JSONs**
- Organização profissional de projetos no GitHub
- Integração entre **IA + Copilot + Graph + Microsoft 365**
- Boas práticas de versionamento e documentação técnica

---

## 🧩 Próximos Passos Evolutivos

- Criar scripts para consumir o Graph via **Python** ou **JavaScript**
- Explorar automações com **Power Automate**
- Criar dashboards com dados do Graph
- Desenvolver soluções reais usando **IA + Microsoft 365 + Copilot**
- Iniciar uma API própria consumindo dados do Graph

---

## 🔐 Boas Práticas e Segurança

- **Anonimizar sempre**: substitua dados reais por valores fictícios  
- **Nunca** versionar tokens, cookies, anexos pessoais ou credenciais sensíveis  
- Mantenha a estrutura JSON **idêntica** à devolvida pelo Graph  
- Utilize mensagens de commit claras e padrão semântico, como:
  - `chore: add Graph responses`
  - `docs: update overview`
  - `feat: add screenshots folder`

---
## 🔗 Referências Oficiais

- [Microsoft Graph Overview](https://learn.microsoft.com/graph/overview)
- [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer)
- [Documentação de Permissões e Escopos](https://learn.microsoft.com/graph/permissions-reference)
- [Microsoft Learn – Inteligência Artificial na Prática](https://learn.microsoft.com/)


## 👩‍💻 Autoria e Créditos

**Joelma Campos**  
Participante do *Bootcamp CAIXA – Inteligência Artificial na Prática*  
Microsoft 365 Developer Program  
GitHub: [jfcampos5](https://github.com/jfcampos5)

⭐ Se este repositório te ajudou, considere deixar uma estrela!

## 📄 Licença

Este projeto está licenciado sob a **MIT License**.  
Consulte o conteúdo completo em:  
[LICENSE](./LICENSE)
