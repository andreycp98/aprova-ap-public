# Aprova AP

Plataforma educacional da Norton Empreendimentos para preparação em concursos
públicos, inicialmente focada em SESA-AP e PC-AP e estruturada para expansão a
outros concursos.

## Proposta

O Aprova AP organiza estudo, prática e revisão em uma experiência única:

- banco de questões autorais;
- explicação individual obrigatória para cada alternativa de A a E;
- resumo didático e indicação de fontes;
- caderno de erros e simulados;
- estatísticas, gamificação e ranking;
- trilhas por concurso, cargo, disciplina e tópico;
- apoio editorial e educacional com IA, sempre sujeito a controles e revisão.

## Estado do projeto

O produto está em desenvolvimento e validação para uma versão beta. Ainda não
há URL pública de produção.

## Arquitetura em alto nível

O produto usa Next.js e TypeScript na aplicação, PostgreSQL/Supabase na camada
de dados e autenticação, e serviços especializados para pagamentos,
observabilidade, analytics e comunicação. A arquitetura preserva isolamento
entre dados de alunos, conteúdo editorial e operações administrativas.

Mais detalhes públicos:

- [Visão do produto](docs/product.md)
- [Fluxos principais](docs/app-flow.md)
- [Arquitetura e segurança](docs/architecture.md)
- [Política de segurança](SECURITY.md)

## Sobre este repositório

Este é um repositório público de apresentação. O código do produto, migrations,
configurações operacionais, prompts, integrações financeiras, regras de acesso
e documentação interna permanecem em repositório privado.

## Direitos

Copyright (c) 2026 Norton Empreendimentos. Todos os direitos reservados.
Consulte [NOTICE.md](NOTICE.md).
