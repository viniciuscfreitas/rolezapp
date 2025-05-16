# PRD: MVP - App Mobile First de Rede Social de Eventos

> Consulte também: [Modelo de Negócio e Plano Financeiro](./modelo-negocio-e-plano-financeiro.md)

## 1. Visão do Produto

Criar um aplicativo mobile nativo (React Native + Expo), moderno e social, que conecta pessoas, organizadores, artistas e influenciadores em torno de eventos presenciais e experiências culturais. O app deve ser rápido, intuitivo, visualmente atraente e fácil de usar, inspirado em apps como Instagram, Messenger e outros produtos mobile da Meta.

## 2. Público-Alvo

- Jovens adultos urbanos (18-35 anos)
- Organizadores e produtores independentes
- Artistas locais, bandas, DJs
- Influenciadores digitais e microinfluenciadores

## 3. Problemas a Resolver

- Dificuldade de descobrir eventos relevantes e experiências sociais locais
- Falta de engajamento e comunidade em apps de ticketing tradicionais
- Processo de compra de ingressos pouco fluido e mobile
- Pouca visibilidade para artistas e eventos independentes

## 4. Funcionalidades Essenciais (MVP)

- Cadastro/login (e-mail, redes sociais, autenticação via Auth0/Clerk/Firebase)
- Feed de eventos recomendados (rolagem vertical, stories no topo)
- Busca de eventos (cidade, data, categoria, palavra-chave)
- Criação e divulgação de eventos (nome, descrição, data, local, preço, ingressos, imagem)
- Compra/venda de ingressos (pagamento integrado, QR code)
- Perfil do usuário (foto, bio, eventos frequentados, conquistas)
- Lista de amigos e convites para eventos
- Notificações push (eventos próximos, convites, ingressos)
- Gamificação leve (badges por participação, ranking simples)
- Perfis profissionais para atrações (artistas, DJs) com portfólio básico
- Comunidades/grupos temáticos (mínimo viável)
- Networking entre participantes de um mesmo evento
- Destaque pago para eventos (eventos promovidos)
- Anúncios segmentados (simples)
- Deep linking para compartilhamento de eventos e convites
- Permissões de câmera/localização para funcionalidades sociais

## 5. Requisitos Técnicos

- Stack React Native (Expo), Tamagui, NativeWind, React Navigation
- Gerenciamento de estado com Zustand/Redux Toolkit
- React Query para dados, Axios/fetch para APIs
- Autenticação com Auth0, Clerk ou Firebase Auth
- Notificações push com Expo Notifications/FCM
- Analytics com Segment, Amplitude, Mixpanel ou Firebase Analytics
- Testes com Jest, React Native Testing Library, Detox
- CI/CD com EAS Build/Submit (Expo)
- Monitoramento com Sentry, debug com Flipper
- OTA updates via Expo
- Publicação nas lojas (App Store/Google Play)

## 6. Métricas e Critérios de Sucesso

- Número de eventos criados e ingressos vendidos no primeiro mês
- Engajamento no feed e comunidades (posts, comentários, convites)
- Taxa de conversão de visitantes em compradores
- Retenção de usuários (30 dias)
- Feedback positivo dos primeiros usuários beta

## 7. Restrições e Considerações

- Foco inicial em mobile nativo (React Native/Expo)
- Simplicidade e clareza visual como prioridade
- Escalabilidade e performance para picos de acesso em eventos grandes
- Privacidade e LGPD desde o início
- Cumprimento das diretrizes da App Store e Google Play

## 8. Roadmap Resumido

1. Wireframes e protótipo visual (Figma)
2. Setup do projeto com Expo, Tamagui, NativeWind
3. Implementação dos fluxos principais (onboarding, feed, evento, compra)
4. Integração de pagamentos, autenticação e notificações push
5. Testes e validação com usuários reais
6. Publicação nas lojas (App Store/Google Play)
7. Lançamento beta fechado

## 9. Referências Visuais e de UX
- Instagram, Facebook, Messenger, Brex, Cameo, Discord
- [Tamagui](https://tamagui.dev/), [NativeWind](https://www.nativewind.dev/)
- [Expo](https://expo.dev/), [React Native](https://reactnative.dev/)
- [UX Planet - Mobile Design Concepts](https://uxplanet.org/15-stylish-and-user-friendly-mobile-design-concepts-2987319ac81e)
- [UX Design Institute - Mobile App Design Guide](https://www.uxdesigninstitute.com/blog/ultimate-guide-to-mobile-app-design/)

## 10. Pontos Cegos e Estratégias de Mitigação

- **Capacidade de Execução Solo:** O projeto é tocado apenas por uma pessoa e uma IA, exigindo foco extremo no MVP e automação máxima.
- **Validação Externa Limitada:** Não há acesso direto a usuários reais, então decisões são baseadas em benchmarking, tendências e pesquisa web contínua.
- **Viés de Confirmação:** Para evitar decisões enviesadas, aplicamos técnicas como pré-mortem, red teaming e buscamos feedback externo sempre que possível.
- **Atualização Contínua:** Utilizamos pesquisa web para manter o projeto alinhado com tendências e melhores práticas do mercado.
- **Referências:**  
  - [OpenHubNews: Pontos cegos da liderança](https://openhubnews.com/bo-os-pontos-cegos-da-lideranca/)  
  - [NaPratica.org.br: Técnicas para identificar pontos cegos](https://napratica.org.br/tecnicas-pontos-cegos-decisoes/) 