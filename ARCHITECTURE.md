# 🏗️ Arquitetura do NARA CONNECT HUB

## Visão Geral

O NARA CONNECT HUB é um agente de IA conversacional construído com arquitetura moderna e escalável, focado em conectar pessoas a oportunidades.

## Diagrama de Fluxo

## Componentes

### 1. Frontend (Interface do Usuário)
- **Tecnologia:** Next.js + React + TypeScript
- **Função:** Interface conversacional amigável em português
- **Deploy:** Vercel / Lovable

### 2. Backend (API)
- **Tecnologia:** Node.js com rotas TypeScript
- **Função:** Gerencia as requisições e comunicações
- **Estrutura:** Pastas `app/api/` com rotas organizadas

### 3. Inteligência Artificial
- **Tecnologia:** Google Gemini API
- **Função:** Processa as conversas e gera respostas contextualizadas
- **Personalidade:** Configurada via `SYSTEM_PROMPT_NARA.md`

### 4. Funcionalidades
- **Chats:** Sistema de conversas com histórico
- **Voz:** Recursos de speak e transcribe
- **Autenticação:** Login de usuários
- **Sponsors:** Área para patrocinadores

## Fluxo de Dados

1. Usuário acessa o site `connect-hub-br.lovable.app`
2. Faz uma pergunta ou escolhe um tema
3. Frontend envia para a API
4. API consulta a IA Gemini com o prompt do sistema
5. IA gera resposta contextualizada
6. Resposta volta para o usuário

## Segurança e Privacidade

- Dados sensíveis em variáveis de ambiente (`.env`)
- Arquivos de configuração ignorados via `.gitignore`
- Comunicação segura via HTTPS

## Próximas Evoluções

- Integração com AWS Strands Agents (para Agents for Humans)
- Base de dados de oportunidades atualizada
- Versão mobile nativa
- Parcerias com escolas e cooperativas

---

**Criado por:** Márcia Abrantes  
**Conecta. Compreende. Transforma.**
