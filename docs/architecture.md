# Arquitetura e segurança

## Visão geral

```text
Navegador
   |
   v
Aplicação Next.js
   |-- autenticação e autorização no servidor
   |-- regras de assinatura e limites
   |-- fluxo editorial
   |
   v
PostgreSQL / Supabase
   |-- isolamento por políticas de acesso
   |-- armazenamento privado
   |-- trilha de auditoria e versionamento
   |
   +--> pagamento, e-mail, observabilidade e analytics
```

## Fronteiras de confiança

O navegador é considerado não confiável. Identidade, papéis, acesso a dados,
limites de uso, publicação e processamento de pagamentos são revalidados no
servidor e no banco de dados.

## Controles centrais

- papéis separados para aluno, editor, revisor e administração;
- políticas de acesso por linha no banco de dados;
- gabaritos indisponíveis antes do envio da resposta;
- validação de propriedade para impedir acesso indevido entre usuários;
- idempotência em operações financeiras e de geração em lote;
- armazenamento privado e validação de uploads;
- limitação de abuso e proteção dos recursos de IA;
- revisão humana antes da publicação editorial;
- ambientes de desenvolvimento, homologação e produção separados.

Detalhes exploráveis, identificadores de infraestrutura, migrations, regras
internas e credenciais não fazem parte deste repositório público.
