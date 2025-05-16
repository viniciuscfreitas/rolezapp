# Plano de Teste (QA) - App Mobile First de Rede Social de Eventos

## 1. Objetivo
- Garantir a qualidade, segurança e usabilidade do app em todas as etapas do desenvolvimento e após o lançamento.

## 2. Tipos de Testes
- Testes unitários (Jest, Testing Library)
- Testes de integração (Jest, Playwright)
- Testes end-to-end (Playwright)
- Testes de usabilidade (testes com usuários reais)
- Testes de performance (Lighthouse, Vercel Analytics)
- Testes de segurança (verificação de autenticação, permissões, LGPD)
- Testes de regressão a cada release

## 3. Ferramentas
- Jest, Testing Library (unitários e integração)
- Playwright (E2E)
- Lighthouse (performance)
- Sentry (monitoramento de erros)
- Figma (prototipagem para testes de UX)

## 4. Processo
- Escrever testes automatizados junto com o desenvolvimento de cada funcionalidade
- Revisão de código obrigatória antes de mergear PRs
- Rodar testes automatizados em cada push/PR (CI/CD na Vercel)
- Testes manuais em dispositivos reais antes de releases importantes
- Coleta de feedback de usuários beta
- Correção de bugs priorizada antes de novas features

## 5. Responsabilidades
- Todos os desenvolvedores escrevem e mantêm testes para seu código
- QA (ou responsável designado) coordena testes manuais e de usabilidade
- Time monitora erros e feedbacks pós-lançamento

## 6. Critérios de Aceitação
- Cobertura mínima de testes automatizados (>80%)
- Sem bugs críticos conhecidos em produção
- Fluxos principais (cadastro, compra, navegação) funcionando em todos os dispositivos suportados
- Feedback positivo dos usuários beta 