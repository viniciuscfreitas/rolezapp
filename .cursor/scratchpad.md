# Sumário

- [Sumário](#sumário)
  - [Project Status Board](#project-status-board)
  - [Executor's Feedback or Assistance Requests](#executors-feedback-or-assistance-requests)
    - [1. Onboarding](#1-onboarding)
    - [2. Login/Cadastro](#2-logincadastro)
    - [3. Navegação](#3-navegação)
    - [4. Criação de Evento](#4-criação-de-evento)
    - [5. Compra de Ingresso](#5-compra-de-ingresso)
- [1. Visão Geral e Motivação](#1-visão-geral-e-motivação)
- [2. Público-Alvo](#2-público-alvo)
- [3. Concorrentes e Inspirações](#3-concorrentes-e-inspirações)
  - [Brasil](#brasil)
  - [Internacional](#internacional)
  - [Tendências Globais](#tendências-globais)
- [4. Diferenciais e Estratégia de Mercado](#4-diferenciais-e-estratégia-de-mercado)
- [5. Funcionalidades Essenciais (MVP)](#5-funcionalidades-essenciais-mvp)
  - [Para Fases Futuras](#para-fases-futuras)
- [6. Funcionalidades Avançadas e Ideias Fora da Caixinha](#6-funcionalidades-avançadas-e-ideias-fora-da-caixinha)
- [7. Estratégias para Celebridades, Influenciadores e Atrações](#7-estratégias-para-celebridades-influenciadores-e-atrações)
  - [Celebridades e Influenciadores](#celebridades-e-influenciadores)
  - [Atrações (Músicos, DJs, Artistas)](#atrações-músicos-djs-artistas)
- [8. Monetização](#8-monetização)
  - [MVP](#mvp)
  - [Futuro](#futuro)
- [9. Roadmap e Tarefas](#9-roadmap-e-tarefas)
  - [Roadmap](#roadmap)
  - [Tarefas do MVP](#tarefas-do-mvp)
- [10. Indicadores de Sucesso (KPIs)](#10-indicadores-de-sucesso-kpis)
- [11. Riscos e Mitigação](#11-riscos-e-mitigação)
- [12. Lições Aprendidas](#12-lições-aprendidas)
- [High-level Task Breakdown](#high-level-task-breakdown)
  - [1. Definir fluxos e telas do MVP](#1-definir-fluxos-e-telas-do-mvp)
  - [2. Implementar cadastro/login](#2-implementar-cadastrologin)
  - [3. Implementar criação e divulgação de eventos](#3-implementar-criação-e-divulgação-de-eventos)
  - [4. Implementar compra/venda de ingressos (com marketplace fee)](#4-implementar-compravenda-de-ingressos-com-marketplace-fee)
  - [5. Implementar perfil de usuário](#5-implementar-perfil-de-usuário)
  - [6. Implementar feed e busca de eventos](#6-implementar-feed-e-busca-de-eventos)
  - [7. Implementar lista de amigos e convites](#7-implementar-lista-de-amigos-e-convites)
  - [8. Implementar notificações básicas](#8-implementar-notificações-básicas)
  - [9. Implementar gamificação leve](#9-implementar-gamificação-leve)
  - [10. Implementar perfis profissionais para atrações](#10-implementar-perfis-profissionais-para-atrações)
  - [11. Implementar comunidades/grupos temáticos (mínimo viável)](#11-implementar-comunidadesgrupos-temáticos-mínimo-viável)
  - [12. Implementar networking em eventos](#12-implementar-networking-em-eventos)
  - [13. Implementar destaque pago para eventos](#13-implementar-destaque-pago-para-eventos)
  - [14. Implementar anúncios segmentados](#14-implementar-anúncios-segmentados)
  - [15. Testes e validação](#15-testes-e-validação)

## Project Status Board

- [x] Remover arquivos redundantes: adr-v0-stack.md, referencias-benchmarks.md, auth-integracao.md, setup-deploy.md
- [x] Sugerir fusão de conteúdos técnicos no README e ADR
- [x] Pasta .cursor enxuta e organizada

## Executor's Feedback or Assistance Requests

- Arquivos redundantes removidos da pasta `.cursor`.
- Recomendo que conteúdos técnicos (setup, deploy, autenticação, benchmarks) fiquem centralizados no README principal e/ou ADR para facilitar consulta e manutenção.
- A estrutura da pasta `.cursor` agora está mais enxuta, sem duplicidade de informações.
- Pronto para seguir com a próxima etapa do projeto!

---

# 1. Visão Geral e Motivação

O objetivo é criar um aplicativo mobile first, nichado, que funcione como uma rede social de eventos. O app conecta pessoas, organizadores e atrações, permitindo criar, divulgar e vender ingressos para eventos, além de promover engajamento social, networking e experiências gamificadas.

# 2. Público-Alvo

- Jovens adultos urbanos interessados em eventos culturais, festas, shows e experiências sociais presenciais
- Organizadores e produtores independentes de eventos
- Artistas locais, bandas, DJs e atrações independentes
- Influenciadores digitais, microinfluenciadores e criadores de conteúdo

# 3. Concorrentes e Inspirações

## Brasil
- Sympla ([link](https://www.sympla.com.br/)): ticketing, ferramentas para organizadores, integração social
- Ingresse ([link](https://www.ingresse.com/)): shows, festas, app mobile, Apple Wallet
- Eventbrite Brasil ([link](https://www.eventbrite.com.br/)): marketing, relatórios, integração Facebook
- Even3 ([link](https://www.even3.com.br/)): eventos acadêmicos, certificados, submissão de trabalhos
- Meetup Brasil ([link](https://www.meetup.com/pt-BR/)): comunidades, networking, eventos de nicho
- BaladApp ([link](https://www.baladapp.com.br/)): festas, baladas, parcerias com casas noturnas

## Internacional
- Eventbrite ([link](https://www.eventbrite.com/)): referência mundial em eventos, ticketing, gestão
- Meetup ([link](https://www.meetup.com/)): comunidades, networking, engajamento social
- Fever ([link](https://feverup.com/)): experiências exclusivas, curadoria, parcerias
- Bandsintown ([link](https://www.bandsintown.com/)): shows, integração Spotify, alertas personalizados
- Dice ([link](https://dice.fm/)): experiência mobile, lista de espera, revenda
- Universe/Ticketmaster ([link](https://www.universe.com/)): grandes eventos, integração Ticketmaster
- Facebook Events ([link](https://www.facebook.com/events/)): alcance massivo, RSVP fácil

## Tendências Globais
- TikTok, Instagram, Discord, Twitch, Likee, LINE, Viber ([fonte](https://pt.semrush.com/blog/maiores-redes-sociais/)): comunidades, lives, eventos virtuais, gifts, badges, microtransações

# 4. Diferenciais e Estratégia de Mercado

- Foco em comunidade e engajamento social, não só ticketing
- Recursos mobile-first, gamificação e networking
- Benefícios para artistas, influenciadores e organizadores
- Monetização diversificada (ingressos, anúncios, destaque, microtransações)
- Destaque para eventos de artistas locais e independentes
- Ferramentas de networking entre participantes
- Comunidades/grupos temáticos
- Ferramentas para experiências gamificadas presenciais (caça ao tesouro, QR codes, desafios)
- Sistema de recomendações personalizadas
- Feed social, mural de fotos/vídeos, stories e chat/comentários em eventos

# 5. Funcionalidades Essenciais (MVP)

- Cadastro/login simples (e-mail/redes sociais)
- Criação e divulgação de eventos (nome, descrição, data, local, preço, ingressos)
- Compra/venda de ingressos (pagamento integrado, com marketplace fee)
- Perfil do usuário (foto, bio, eventos frequentados)
- Feed de eventos recomendados e busca por cidade/localização
- Lista de amigos e convites para eventos
- Notificações básicas (eventos próximos, convites, ingressos)
- Gamificação leve (badges por participação, ranking simples)
- Perfis profissionais para atrações (artistas, DJs) com portfólio básico
- Comunidades/grupos temáticos (mínimo viável)
- Networking entre participantes de um mesmo evento
- Destaque pago para eventos (eventos promovidos)
- Anúncios segmentados (simples)

## Para Fases Futuras
- Lives e transmissões
- Stories
- Marketplace de produtos
- API pública
- Experiências gamificadas avançadas
- Branded content e parcerias
- Ferramentas avançadas para influenciadores e atrações
- Integrações externas

# 6. Funcionalidades Avançadas e Ideias Fora da Caixinha

- Lives e transmissões de eventos (streaming integrado)
- Stories para usuários e organizadores
- Marketplace de produtos relacionados a eventos (merchandising, acessórios)
- API pública para integração com outros apps e plataformas
- Experiências gamificadas avançadas (caça ao tesouro, desafios, QR codes)
- Branded content, parcerias e conteúdo patrocinado
- Ferramentas avançadas para influenciadores e atrações (analytics, monetização, dashboard)
- Integrações externas (calendários, streaming, redes sociais)
- Modo anônimo para explorar eventos/comunidades
- Sistema de denúncias/moderação colaborativa
- Agenda colaborativa e sugestões de eventos entre amigos
- Sistema de enquetes e votações em comunidades e eventos
- Feed personalizado por comunidade
- Mural colaborativo de fotos/vídeos dos eventos
- Match de eventos (tipo "Tinder de eventos")
- Ranking de usuários mais ativos/influentes
- Sistema de recompensas por engajamento (pontos, moedas virtuais, prêmios)

# 7. Estratégias para Celebridades, Influenciadores e Atrações

## Celebridades e Influenciadores
- Perfis verificados
- Ferramentas exclusivas (dashboard de engajamento, analytics de seguidores, insights de eventos)
- Criação de eventos exclusivos ou privados para fãs/seguidores
- Lives e Q&A exclusivos para seguidores
- Sistema de parcerias e monetização (comissão por venda de ingressos, promoções, cupons)
- Destaque de eventos e perfis no feed principal
- Ranking de influenciadores mais engajados
- Gamificação especial para criadores (badges, conquistas, desafios para seguidores)
- Ferramentas de divulgação integrada (compartilhamento fácil em outras redes, links personalizados)
- Espaço para conteúdo patrocinado e branded content
- Convites VIP e experiências exclusivas
- Suporte dedicado para onboarding
- Comunidades exclusivas para fãs
- Integração com plataformas de streaming/redes sociais
- Notificações personalizadas para seguidores

## Atrações (Músicos, DJs, Artistas)
- Perfis profissionais detalhados
- Portfólio multimídia: vídeos, músicas, fotos, agenda de shows
- Ferramentas para divulgação de lançamentos e eventos próprios
- Sistema de reservas/contratações integrado
- Analytics de público: seguidores, engajamento, alcance
- Venda de merchandising/produtos digitais
- Lives e transmissões de shows exclusivos
- Espaço para interação com fãs (Q&A, enquetes, comentários)
- Ranking de atrações populares e em ascensão
- Gamificação para artistas (desafios, conquistas, badges)
- Destaque em eventos parceiros e festivais
- Networking entre artistas, produtores e organizadores
- Notificações para fãs sobre novidades
- Suporte dedicado para onboarding
- Integração com plataformas de streaming/redes sociais

# 8. Monetização

## MVP
- Taxa sobre venda de ingressos (marketplace fee)
- Destaque pago para eventos
- Anúncios segmentados (simples)

## Futuro
- Planos premium para organizadores (mais destaque, analytics avançado, eventos ilimitados)
- Planos premium para usuários (acesso antecipado a eventos, descontos, benefícios exclusivos)
- Comissões sobre merchandising/produtos digitais
- Taxa sobre reservas/contratações de atrações
- Microtransações (gifts, stickers, badges)
- Funcionalidades extras pagas em comunidades (enquetes, lives, personalização)
- Parcerias com marcas e patrocinadores
- Taxa sobre experiências VIP ou ingressos premium
- Cobrança por integração com plataformas externas (API, streaming, etc.)
- Marketplace de serviços para eventos (buffet, fotografia, etc.)

# 9. Roadmap e Tarefas

## Roadmap
1. MVP: Lançamento com funcionalidades essenciais e monetização básica
2. Fase 2: Expansão de comunidades, networking, gamificação e recursos para artistas
3. Fase 3: Integrações externas, marketplace, experiências VIP, funcionalidades avançadas para influenciadores
4. Fase 4: Internacionalização, API pública, parcerias estratégicas

## Tarefas do MVP
- [ ] Definir fluxos e telas do MVP
- [ ] Escolher stack tecnológica
- [ ] Implementar cadastro/login
- [ ] Implementar criação e divulgação de eventos
- [ ] Implementar compra/venda de ingressos (com marketplace fee)
- [ ] Implementar perfil de usuário
- [ ] Implementar feed e busca de eventos
- [ ] Implementar lista de amigos e convites
- [ ] Implementar notificações básicas
- [ ] Implementar gamificação leve
- [ ] Implementar perfis profissionais para atrações
- [ ] Implementar comunidades/grupos temáticos (mínimo viável)
- [ ] Implementar networking em eventos
- [ ] Implementar destaque pago para eventos
- [ ] Implementar anúncios segmentados
- [ ] Testes e validação

# 10. Indicadores de Sucesso (KPIs)

- Número de eventos criados por mês
- Total de ingressos vendidos
- Taxa de conversão de visitantes em compradores
- Engajamento em comunidades (posts, comentários, enquetes)
- Número de artistas/atrações cadastrados
- Receita gerada por taxas e anúncios
- Retenção de usuários (30/60/90 dias)
- NPS (Net Promoter Score) dos organizadores e participantes

# 11. Riscos e Mitigação

- **Fraudes em ingressos:** Implementar QR code único, validação na entrada, monitoramento de transações suspeitas
- **Moderação de conteúdo:** Ferramentas de denúncia, moderação colaborativa, filtros automáticos, equipe de moderação
- **Privacidade e LGPD:** Políticas claras, consentimento explícito, controles de privacidade, anonimização de dados
- **Baixa adesão de artistas/atrações:** Estratégias de onboarding, benefícios exclusivos, divulgação, parcerias
- **Dependência de receita de ingressos:** Diversificar monetização com anúncios, planos premium, marketplace, microtransações
- **Concorrência com grandes players:** Foco em nicho, diferenciação por comunidade, gamificação e experiência mobile
- **Baixo engajamento inicial:** Campanhas de lançamento, parcerias com influenciadores, incentivos de engajamento

# 12. Lições Aprendidas

- Incluir informações úteis para debugging na saída do programa.
- Ler o arquivo antes de tentar editar.
- Se aparecerem vulnerabilidades no terminal, rodar npm audit antes de prosseguir.
- Sempre perguntar antes de usar o comando git -force.
- Sempre consultar as documentações oficiais e links atualizados das tecnologias da stack antes de implementar ou atualizar dependências, para evitar erros por informações antigas.

# High-level Task Breakdown

## 1. Definir fluxos e telas do MVP
- Mapear todos os fluxos principais do usuário (onboarding, login, navegação, criação de evento, compra de ingresso, etc.)
- Criar wireframes de baixa fidelidade para cada tela essencial
- Validar os fluxos e wireframes com base em benchmarks e referências
- Critério de sucesso: todos os fluxos essenciais mapeados e wireframes aprovados

## 2. Implementar cadastro/login
- Configurar autenticação (Auth0, Clerk ou Firebase Auth)
- Implementar telas de login, cadastro e recuperação de senha
- Validar autenticação social (Google, Apple, Facebook)
- Critério de sucesso: usuário consegue criar conta, logar e recuperar senha

## 3. Implementar criação e divulgação de eventos
- Criar tela/formulário para novo evento (nome, descrição, data, local, preço, ingressos, imagem)
- Implementar upload de imagem e seleção de local
- Salvar evento no backend e exibir confirmação
- Critério de sucesso: organizador consegue criar e publicar evento

## 4. Implementar compra/venda de ingressos (com marketplace fee)
- Integrar gateway de pagamento (Stripe/Mercado Pago)
- Implementar fluxo de compra de ingresso (seleção, pagamento, confirmação)
- Gerar QR code único para cada ingresso
- Critério de sucesso: usuário compra ingresso, recebe QR code e fee é registrada

## 5. Implementar perfil de usuário
- Criar tela de perfil (foto, bio, eventos frequentados, conquistas)
- Permitir edição de dados e upload de foto
- Exibir histórico de eventos e badges
- Critério de sucesso: usuário visualiza e edita perfil, vê conquistas

## 6. Implementar feed e busca de eventos
- Implementar feed de eventos recomendados (rolagem vertical, stories no topo)
- Implementar busca por cidade, data, categoria, palavra-chave
- Exibir detalhes do evento ao clicar
- Critério de sucesso: usuário navega pelo feed e encontra eventos

## 7. Implementar lista de amigos e convites
- Permitir busca e adição de amigos
- Implementar envio de convites para eventos
- Exibir lista de amigos e convites recebidos
- Critério de sucesso: usuário adiciona amigos e envia/recebe convites

## 8. Implementar notificações básicas
- Configurar push notifications (Expo Notifications/FCM)
- Enviar notificações para eventos próximos, convites e ingressos
- Critério de sucesso: usuário recebe notificações relevantes

## 9. Implementar gamificação leve
- Definir badges e critérios de conquista
- Implementar sistema de ranking simples
- Exibir badges e ranking no perfil
- Critério de sucesso: usuário recebe badges e ranking é atualizado

## 10. Implementar perfis profissionais para atrações
- Criar tela de perfil profissional (artista, DJ)
- Permitir portfólio básico (fotos, vídeos, agenda)
- Exibir eventos associados ao perfil
- Critério de sucesso: artista cria perfil e associa eventos

## 11. Implementar comunidades/grupos temáticos (mínimo viável)
- Criar tela/lista de comunidades
- Permitir criação e entrada em grupos temáticos
- Exibir feed básico de cada grupo
- Critério de sucesso: usuário entra/cria grupo e interage no feed

## 12. Implementar networking em eventos
- Permitir visualização de participantes de um evento
- Implementar chat ou sistema de mensagens básico entre participantes
- Critério de sucesso: participantes interagem durante o evento

## 13. Implementar destaque pago para eventos
- Permitir que organizadores promovam eventos mediante pagamento
- Exibir eventos promovidos em destaque no feed
- Critério de sucesso: evento promovido aparece em destaque após pagamento

## 14. Implementar anúncios segmentados
- Integrar sistema simples de anúncios (banner ou card)
- Exibir anúncios segmentados por perfil/interesse
- Critério de sucesso: anúncios aparecem para o público-alvo

## 15. Testes e validação
- Escrever testes unitários e de integração para fluxos principais
- Realizar testes manuais e beta com usuários reais
- Corrigir bugs e ajustar UX
- Critério de sucesso: funcionalidades testadas, bugs corrigidos e feedback positivo

# Plano de Atualização da Documentação (Stack Monorepo Fullstack)

## Objetivo
Atualizar toda a documentação do projeto para refletir a stack escolhida:
- Monorepo com Turborepo
- Next.js (web), React Native (Expo) (mobile), Tamagui (UI compartilhada)
- Node.js + TypeScript (backend), tRPC (API), Prisma (ORM), PostgreSQL (DB)
- Pacotes compartilhados para tipos, componentes e utilitários

## Tarefas Detalhadas

1. **Recriar ADR (Architecture Decision Record) da Stack**
   - Justificativa da stack escolhida
   - Alternativas consideradas
   - Links oficiais das tecnologias
   - Vantagens e possíveis desafios
   - Estrutura sugerida do monorepo
   - Critério de sucesso: ADR detalhado, claro e atualizado

2. **Criar/Atualizar README do Monorepo**
   - Visão geral do projeto
   - Estrutura de pastas (apps, packages, etc.)
   - Como rodar localmente (web, mobile, backend)
   - Como rodar testes, lint, build, deploy
   - Como adicionar novos pacotes compartilhados
   - Links para docs oficiais
   - Critério de sucesso: README serve como guia de onboarding

3. **Atualizar Sumário e Status Board no .cursor/scratchpad.md**
   - Refletir nova stack e estrutura
   - Atualizar tarefas e próximos passos
   - Critério de sucesso: sumário e board fiéis ao novo contexto

4. **Orientações para Setup e Deploy**
   - Setup local (Node, Yarn/NPM, PostgreSQL, Expo CLI, etc.)
   - Deploy web (Vercel), mobile (Expo), backend (Railway/Render/Vercel Functions)
   - Variáveis de ambiente e segredos
   - Critério de sucesso: instruções claras e testadas

5. **Observações sobre Autenticação e Integração**
   - Sugestão de integração de Auth (Clerk/Auth0/Firebase) com tRPC
   - Compartilhamento de tipos e validações (zod)
   - Critério de sucesso: recomendações práticas e links úteis

6. **Referências e Benchmarks**
   - Links para exemplos de monorepo, design system, tRPC, etc.
   - Critério de sucesso: seção de referências útil para consulta

---

## High-level Task Breakdown (Atualizado)
- [ ] Recriar ADR da stack
- [ ] Criar/atualizar README do monorepo
- [ ] Atualizar sumário e status board
- [ ] Documentar setup e deploy
- [ ] Adicionar observações de autenticação/integracão
- [ ] Incluir referências e benchmarks

## Critérios de Sucesso Gerais
- Documentação clara, atualizada e alinhada à stack
- Facilitar onboarding e manutenção
- Servir de referência para decisões futuras

---

**Aguardando revisão/aprovação para iniciar execução (Executor).**