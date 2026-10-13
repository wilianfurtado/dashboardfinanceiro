# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users
Casal (Willian & Marina) gerenciando as finanças conjuntas da casa, despesas recorrentes e compras parceladas compartilhadas, além de painel pessoal dedicado para controle de gastos individuais.

## Product Purpose
Prover visibilidade financeira cristalina e controle de fluxo de caixa em tempo real para o casal, garantindo equidade proporcional nas contribuições, acompanhamento progressivo de quitação de compras e suporte à tomada de decisões orçamentárias.

## Positioning
Dashboard financeiro para casais focado em divisão proporcional justa e acompanhamento tátil de parcelas, operando como uma Single Page Application estática de alta performance integrada diretamente ao Google Sheets (via Google Apps Script), sem custos recorrentes ou dependência de servidores intermediários.

## Operating Context
- **Mobile-first cotidiano:** Acesso frequente no smartphone para conferir parcelas do mês, marcar acertos e registrar novas compras ou despesas variáveis.
- **Desktop e planejamento:** Sessões de fechamento mensal, simulação de projeções de 18 meses com IA e ajustes de meta orçamentária.
- **Ambiente de sincronização:** Integração direta com Google Apps Script Web App com fila local offline (`PENDING_SYNC`) e cache no `localStorage`.

## Capabilities and Constraints
- Autenticação segura via Google Identity Services (GSI).
- Sincronização assíncrona POST/GET com backend no Google Apps Script.
- Motor de cálculo proporcional dinâmico baseado na proporção da renda de cada integrante do casal.
- Acompanhamento granular de parcelas com dots interativos, status de acerto do mês e histórico de 18 meses.
- Gráficos visuais com Chart.js adaptados dinamicamente para os temas claro e escuro.
- Assistente financeiro conversacional Gemini para análise de gastos e simulação de novas despesas.
- **Restrição arquitetural durável:** SPA estática pura unificada (HTML5, CSS moderno e Vanilla JavaScript), sem build tools, transpiladores ou frameworks externos.

## Brand Commitments
- **Nome:** Casa Nova.
- **Identidade:** Design System moderno (inspirado no beUI), tipografia `DM Sans` + `DM Serif Display`, contraste WCAG AA/AAA, acabamento com micro-bordas translúcidas e motion tokens fluidos.
- **Voz:** Prática, confiável, colaborativa e focada em tranquilidade financeira para o casal.

## Evidence on Hand
- Aplicação completa em produção no arquivo `index.html`.
- Planilha Google Sheets ativa e integrada via Apps Script.
- Credenciais e fluxos de autenticação Google GSI configurados.

## Product Principles
1. **Equidade e Clareza:** Contribuições calculadas proporcionalmente à renda de forma transparente, eliminando ruídos no relacionamento.
2. **Microinterações sem Fricção:** Marcação de parcelas e acertos com resposta tátil elástica e feedback instantâneo.
3. **Resiliência de Dados:** Operação tolerante a falhas com fila offline local que sincroniza automaticamente quando online.
4. **Previsibilidade Financeira:** Projeção clara de compromissos futuros e insights via IA para garantir que nunca falte saldo livre.

## Accessibility & Inclusion
- Suporte total a temas Dark/Light com contraste calibrado.
- Alvos táteis mobile de no mínimo 44x44px e preenchimento seguro de Safe Area.
- Alinhamento numérico tabular (`font-variant-numeric: tabular-nums`) para legibilidade financeira imediata.
