# Release 1.0.1 — Estabilização

Data: 2026-08-06

## Produção

- URL: https://lagestao.vercel.app
- Vercel project: `prj_ORRLQIQXtKXx6xttJSnTKR1BbNgB`
- Deployment: `dpl_A7xWBWKSQvdmFA2bPkeQgSQAd6Qe`
- Código-fonte canônico: commit `19d1793`
- Supabase project: `wrlafgdrvrjjvdokmtks`

## Correções principais

- saldo consolidado sempre branco no Painel;
- escala assinada no gráfico de fluxo de caixa;
- gráficos complementares visíveis no celular;
- invalidação centralizada de Painel, caixa, contas e relatórios;
- lixeira restaurável para documentos e lançamentos;
- agrupamento correto de transferências e pares de estorno;
- restauração com recomposição de parcelas;
- criação de serviços corrigida;
- privilégio `TRUNCATE` removido dos rascunhos;
- integridade entre documentos excluídos e parcelas;
- configuração canônica da empresa;
- exportação CSV da auditoria.

## Evidências

- Supabase `ACTIVE_HEALTHY`;
- 30/30 tabelas públicas com RLS;
- 42/42 testes SQL aprovados;
- lint aprovado;
- TypeScript strict aprovado;
- evidência anterior de 292 testes unitários, 36 E2E públicos, 29 E2E autenticados e build PWA aprovado;
- build de produção verificou SHA-256 do pacote e 62/62 arquivos finais;
- nenhuma ocorrência de erro de runtime registrada após a publicação.

## Limitações conhecidas

- MFA depende de configuração pelo administrador no próprio dispositivo;
- a proteção contra senhas vazadas permanece desativada no Supabase Auth;
- a reinstalação independente das dependências neste ambiente foi limitada pelo registro interno, que não disponibilizou os pacotes nativos Linux exigidos pelo Rollup;
- o smoke autenticado final com as credenciais reais de Victor e Luciano depende de sessão/credenciais inseridas fora do chat.
