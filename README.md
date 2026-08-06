# L&A Gestão

Sistema web/PWA financeiro e operacional da L&A Serralheria.

## Produção

- URL oficial: https://lagestao.vercel.app
- Release: `1.0.1`
- Fonte canônica: commit local `19d1793`, preservado no ZIP final e no Git bundle de entrega
- Supabase: projeto `wrlafgdrvrjjvdokmtks`
- Vercel: deployment de produção `dpl_A7xWBWKSQvdmFA2bPkeQgSQAd6Qe`

## Conteúdo deste repositório

O diretório `release-payload/` contém blocos do build compilado usados para reconstrução verificável na Vercel. O build valida o SHA-256 do pacote e os hashes dos 62 arquivos finais antes da publicação.

O código-fonte completo, migrations, testes, documentação, histórico Git e evidências estão no pacote ZIP final entregue pelo projeto. Nenhuma credencial, arquivo `.env`, `node_modules`, cache ou token administrativo é versionado aqui.

## Segurança

- RLS ativa nas 30 tabelas públicas do Supabase;
- cadastro público não faz parte do fluxo do aplicativo;
- operações administrativas críticas exigem papel ADMIN e auditoria;
- lixeira restaurável preserva rastreabilidade;
- tokens e segredos não devem ser enviados ao repositório.

Consulte `RELEASE_1.0.1.md` e `SECURITY.md` para detalhes.