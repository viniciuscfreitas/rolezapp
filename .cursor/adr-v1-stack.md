# ADR: Stack Tecnológica Monorepo Fullstack (Web + Mobile + Backend)

## Contexto
O projeto demanda alta produtividade, integração entre web/mobile/backend, consistência visual e tipagem compartilhada. O objetivo é acelerar o desenvolvimento, facilitar manutenção e garantir experiência moderna para usuários e desenvolvedores.

## Stack Escolhida

### Organização
- **Monorepo com Turborepo**: gerenciamento centralizado de apps (web, mobile, backend) e pacotes compartilhados (UI, tipos, utils).

### Frontend
- **Next.js (React + TypeScript)**: web app SSR/SSG, integração com Vercel.
- **React Native (Expo)**: app mobile iOS/Android, build simplificado, hot reload.
- **Tamagui**: design system compartilhado entre web e mobile.
- **react-hook-form + zod**: formulários performáticos e validação typesafe.
- **React Navigation**: navegação mobile.
- **lucide-react**: ícones modernos e leves.

### Backend
- **Node.js + TypeScript**: API e lógica de negócio.
- **tRPC**: integração direta, typesafe, sem duplicação de tipos.
- **Prisma**: ORM moderno, migrations, integração com TypeScript.
- **PostgreSQL**: banco de dados relacional robusto.

### Deploy
- **Vercel**: web (Next.js)
- **Expo**: mobile
- **Railway/Render/Vercel Functions**: backend

### Autenticação (sugestão)
- **Clerk/Auth0/Firebase Auth**: integração fácil com web/mobile, compatível com tRPC.

## Alternativas Consideradas
- REST/GraphQL em vez de tRPC (maior boilerplate, menos integração typesafe)
- Monorepo com Nx (Turborepo é mais simples para JS/TS)
- Design system próprio (Tamagui acelera e já resolve web/mobile)
- MongoDB (PostgreSQL é mais robusto para relacionamentos)

## Vantagens
- Tipagem compartilhada end-to-end (menos bugs, refatoração fácil)
- UI consistente entre web e mobile
- Produtividade máxima (menos retrabalho, mais reuso)
- Deploy simplificado (Vercel/Expo)
- Facilidade de onboarding para novos devs

## Possíveis Desafios
- Curva de aprendizado inicial para monorepo/tRPC/Tamagui
- Integração de libs nativas no Expo pode exigir ajustes
- Se precisar expor API pública REST/GraphQL, será necessário endpoint separado

## Estrutura Sugerida do Monorepo

```
/apps
  /web         # Next.js
  /mobile      # React Native (Expo)
  /backend     # Node.js + tRPC + Prisma
/packages
  /ui          # Componentes Tamagui compartilhados
  /types       # Tipos TypeScript compartilhados
  /utils       # Utilitários compartilhados
```

## Links Oficiais
- [Turborepo](https://turbo.build/)
- [Next.js](https://nextjs.org/)
- [React Native](https://reactnative.dev/)
- [Expo](https://expo.dev/)
- [Tamagui](https://tamagui.dev/)
- [tRPC](https://trpc.io/)
- [Prisma](https://www.prisma.io/)
- [PostgreSQL](https://www.postgresql.org/)
- [react-hook-form](https://react-hook-form.com/)
- [zod](https://zod.dev/)
- [lucide-react](https://lucide.dev/)
- [Clerk](https://clerk.dev/) / [Auth0](https://auth0.com/) / [Firebase Auth](https://firebase.google.com/products/auth)
- [Vercel](https://vercel.com/)
- [Railway](https://railway.app/) / [Render](https://render.com/)

## Critério de Sucesso
- ADR detalhado, claro, atualizado e alinhado ao objetivo do projeto. 