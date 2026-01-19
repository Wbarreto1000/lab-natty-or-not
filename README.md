

---
# **Estética Pro** - Sistema de Gestão para Profissionais de Estética

## 📒 Descrição

Sistema completo de gestão para profissionais da área de estética (biomédicos, esteticistas, dermatologistas). A aplicação permite gerenciar pacientes, agendamentos, protocolos de tratamento, anamnese, galeria de fotos, prescrições e prontuários médicos. O grande diferencial é a **geração automatizada de protocolos de tratamento personalizados com Inteligência Artificial**, que analisa a anamnese do paciente e sugere tratamentos específicos para avaliações faciais, corporais e capilares.

## 🤖 Tecnologias Utilizadas

### **Frontend**
| Tecnologia | Descrição |
|------------|-----------|
| **React 18** | Biblioteca JavaScript para construção de interfaces de usuário |
| **TypeScript** | Superset de JavaScript com tipagem estática |
| **Vite** | Build tool e dev server de nova geração |
| **Tailwind CSS** | Framework CSS utility-first para estilização |
| **shadcn/ui** | Componentes de UI reutilizáveis baseados em Radix UI |
| **Radix UI** | Primitivos de UI acessíveis e sem estilo |
| **React Router DOM** | Roteamento para aplicações React SPA |
| **TanStack React Query** | Gerenciamento de estado assíncrono e cache |
| **React Hook Form + Zod** | Formulários com validação de schema |
| **Recharts** | Biblioteca de gráficos para visualização de dados |
| **Lucide React** | Ícones modernos e customizáveis |
| **date-fns** | Manipulação de datas |
| **Embla Carousel** | Carrosséis e sliders |

### **Backend (Serverless)**
| Tecnologia | Descrição |
|------------|-----------|
| **Supabase** | Backend-as-a-Service (BaaS) |
| **PostgreSQL** | Banco de dados relacional |
| **Supabase Auth** | Autenticação com confirmação por email |
| **Supabase Storage** | Armazenamento de arquivos (fotos, documentos) |
| **Supabase Edge Functions** | Funções serverless em Deno/TypeScript |
| **Row Level Security (RLS)** | Segurança a nível de linha no banco de dados |

### **Integrações de IA e APIs**
| Tecnologia | Descrição |
|------------|-----------|
| **Lovable AI Gateway** | Gateway para modelos de IA generativa |
| **Google Gemini 2.5 Flash** | Modelo de IA para geração de protocolos e pós-cuidados |
| **Resend** | Serviço de envio de emails transacionais |

### **Plataforma de Desenvolvimento**
| Tecnologia | Descrição |
|------------|-----------|
| **Lovable** | Plataforma de desenvolvimento assistido por IA |
| **Lovable Cloud** | Infraestrutura cloud integrada |
| **GitHub** | Versionamento e colaboração de código |

## 🧐 Processo de Criação

O projeto foi desenvolvido utilizando a plataforma **Lovable**, que combina desenvolvimento assistido por IA com infraestrutura cloud integrada. O processo incluiu:

1. **Definição de Requisitos**: Mapeamento das necessidades de profissionais de estética para gestão de clínica
2. **Modelagem de Dados**: Criação do schema do banco de dados PostgreSQL com tabelas para pacientes, agendamentos, protocolos, anamnese, fotos, prescrições e prontuários
3. **Desenvolvimento Iterativo**: Implementação gradual de features através de prompts conversacionais com a IA do Lovable
4. **Integração de IA Generativa**: Configuração do Lovable AI Gateway para conectar ao modelo Gemini e gerar protocolos de tratamento personalizados
5. **Segurança**: Implementação de RLS (Row Level Security), validação de inputs com Zod, confirmação de email e políticas de senha forte
6. **Edge Functions**: Desenvolvimento de funções serverless para geração de protocolos, envio de emails e confirmação/cancelamento de agendamentos

## 🚀 Resultados

### **Funcionalidades Implementadas**
- ✅ Autenticação segura com confirmação por email e políticas de senha forte
- ✅ Cadastro completo de pacientes com foto de capa
- ✅ Sistema de lixeira para pacientes inativos com restauração
- ✅ Agenda interativa com drag-and-drop para reagendamentos
- ✅ Anamnese detalhada (facial, corporal, capilar)
- ✅ Galeria de fotos com categorização por tipo de avaliação
- ✅ **Geração de protocolos com IA** baseados na anamnese do paciente
- ✅ Orientações de pós-cuidados geradas automaticamente
- ✅ Sistema de prescrições com impressão personalizada
- ✅ Prontuário médico com histórico de sessões
- ✅ Upload de documentos do paciente
- ✅ Sistema de convites para novos profissionais
- ✅ Perfil profissional completo com logo da clínica
- ✅ Emails automáticos de confirmação de agendamento
- ✅ Interface responsiva e moderna

### **Edge Functions Desenvolvidas**
| Função | Descrição |
|--------|-----------|
| `generate-protocol` | Gera protocolos de tratamento personalizados usando IA |
| `send-appointment-email` | Envia emails de confirmação de agendamento |
| `send-appointment-reminder` | Envia lembretes de agendamentos |
| `confirm-appointment` | Confirma agendamentos via token |
| `cancel-appointment` | Cancela agendamentos via token |

## 💭 Reflexão

O maior desafio foi criar uma experiência **"natty"** (natural) com IA onde os protocolos gerados parecem ter sido escritos por um especialista humano. Para isso:

- **Prompts bem estruturados**: Foram criados prompts específicos para cada tipo de avaliação (facial, corporal, capilar) com instruções detalhadas de formatação
- **Contexto rico**: A IA recebe toda a anamnese do paciente, histórico de saúde, estilo de vida e contraindicações
- **Personalização**: Os protocolos consideram expectativas do paciente e observações clínicas
- **Consistência**: Uso de temperatura 0 para garantir resultados determinísticos e reproduzíveis

A plataforma Lovable mostrou-se extremamente eficiente para desenvolvimento rápido, permitindo iterar sobre features complexas através de conversação natural, enquanto mantém a flexibilidade de ajustar código diretamente quando necessário.

---

## 🔗 Links Interessantes

- [Documentação do Lovable](https://docs.lovable.dev/)
- [Supabase Docs](https://supabase.com/docs)
- [shadcn/ui Components](https://ui.shadcn.com/)
- [TanStack React Query](https://tanstack.com/query)
- [Google AI (Gemini)](https://ai.google.dev/)

Desenvolvido por Wagner Barreto


