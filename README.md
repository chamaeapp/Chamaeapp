# Chamaê — protótipo PWA

## O que já funciona
- Interface responsiva para celular e computador.
- Cadastro local de perfil de cliente ou profissional.
- Anúncios de serviços com categoria, descrição, cidade e preço.
- Busca e filtros por categoria.
- Solicitações e aceite de pedidos em uma demonstração local.
- Manifest e service worker para instalação/cache quando servido por HTTPS.

## Limitações importantes
Esta é uma primeira versão de frontend. Os dados ficam no armazenamento local do navegador (`localStorage`), portanto:
- não são compartilhados entre celulares ou usuários;
- não há autenticação real, recuperação de senha ou verificação de telefone;
- não há banco de dados, painel administrativo, pagamentos ou notificações push;
- os anúncios demonstrativos não representam empresas reais.

## Como testar
Sirva esta pasta por HTTPS ou em localhost. Por exemplo, com Python:
`python -m http.server 8000`
Depois abra `http://localhost:8000`. A instalação PWA exige HTTPS em produção (localhost é aceito para testes).

## Próxima etapa para produção
Conectar um backend com autenticação, banco de dados, regras de acesso por usuário, armazenamento de fotos, moderação, privacidade e proteção contra fraude. Só então clientes e prestadores poderão usar contas e anúncios compartilhados em dispositivos diferentes.
