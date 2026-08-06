# Política de Segurança

## Segredos e credenciais

Nunca versionar:

- `.env` ou `.env.local`;
- `SUPABASE_SERVICE_ROLE_KEY`;
- senha do banco ou `DATABASE_URL` com senha;
- tokens pessoais do Supabase;
- `VERCEL_TOKEN` ou tokens OIDC;
- chaves privadas ou segredos JWT.

A URL e a chave pública/anon do Supabase usadas pelo frontend não substituem as políticas RLS. A proteção dos dados depende da autorização no banco.

## Controle de acesso

- somente usuários vinculados à organização podem acessar os dados;
- ações administrativas críticas exigem papel `ADMIN`;
- exclusões usam lixeira restaurável e trilha de auditoria;
- registros de auditoria não devem ser apagados pela interface.

## Comunicação de vulnerabilidades

Falhas devem ser registradas de forma privada com o administrador do projeto antes de qualquer divulgação pública. Não incluir credenciais, dados de clientes ou informações financeiras em issues públicas.
