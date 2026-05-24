# Guia do Agente Especialista UX/UI Trendseeker

Este guia ensina como **instalar**, **utilizar** e **replicar** o agente especialista em **UX/UI Trendseeker** em qualquer projeto que utilize o ecossistema **Antigravity**.

---

## 🎨 Sobre o Agente UX/UI Trendseeker

O **UX/UI Trendseeker** é uma persona altamente especializada, projetada para atuar em duas frentes fundamentais:
1. **Mineração Ativa de Tendências**: Rastreia novidades estéticas, transições físicas e componentes modernos nos portais mais influentes de design digital (como *Codepen, Behance, Figma Community, ThemeForest, e Tailwind UI*).
2. **Criação de Componentes Autorais e Premium**: Desenvolve interfaces sob uma base utilitária de **Tailwind CSS**, mas focando em **autenticidade visual**, micro-animações ricas e **responsividade absoluta (mobile first)**.

---

## 📦 Como Instalar em Outros Projetos (Replicação)

A arquitetura do Antigravity é inteiramente portátil. Para levar este agente especialista e seus comandos automatizados para qualquer outro repositório, siga os passos abaixo:

### Passo 1: Copiar os Arquivos do Agente
Navegue até o diretório `.agent` do seu projeto atual e copie os seguintes arquivos para o mesmo local no projeto de destino:

1. **Definição da Persona**:
   - Origem: `.agent/agents/ux-ui-trend-specialist.md`
   - Destino no novo projeto: `.agent/agents/ux-ui-trend-specialist.md`
   
2. **Workflow de Execução**:
   - Origem: `.agent/workflows/ux-ui-trendseeker.md`
   - Destino no novo projeto: `.agent/workflows/ux-ui-trendseeker.md`

### Passo 2: Reiniciar o Antigravity
Após colar os arquivos no novo projeto, reinicie a sessão da sua IA ou recarregue a IDE. O Antigravity lerá automaticamente a pasta `.agent/agents/` e adicionará a persona `ux-ui-trend-specialist` à sua lista de subagentes utilizáveis.

---

## 🚀 Como Utilizar o Agente no Dia a Dia

Há duas formas principais de interagir com o agente: invocando a persona diretamente nas suas instruções ou ativando o workflow oficial de mineração.

### Método 1: Chamando o Workflow de Mineração (Recomendado)
Para iniciar uma pesquisa de tendências ativa e criar um componente a partir de referências modernas da internet, digite no chat:

> **`/browser /ux-ui-trendseeker Quero criar uma seção de Hero para um aplicativo de telemetria em nuvem usando Tailwind`**

#### O que o Antigravity fará automaticamente:
1. **Análise de Contexto**: Entenderá que você precisa de uma seção de Hero com características de telemetria.
2. **Pesquisa Ativa (Navegação)**: O subagente `/browser` acessará os portais de design buscando referências modernas de designs de dashboard, grafismo e efeitos de luz/vidro.
3. **Ficha de Compromisso**: Declarará no chat as escolhas visuais tomadas para escapar dos layouts clichês da internet (como grids hexagonais ou o split tradicional de 50/50).
4. **Implementação**: Escreverá o componente em Tailwind CSS otimizado para GPU (com foco em responsividade e micro-interações).
5. **Auditoria**: Garantirá que o componente se ajuste perfeitamente em telas móveis de 360px sem quebras.

---

### Método 2: Invocação Direta da Persona
Se você já possui um arquivo existente e deseja apenas que o especialista em UX/UI audite a interface ou faça melhorias estéticas específicas, você pode marcar a persona diretamente na mensagem:

> **`@ux-ui-trend-specialist Revise o meu arquivo /apps/tb-web/components/Navbar.tsx e adicione micro-interações suaves no menu de navegação responsivo.`**

#### O que ele auditará com prioridade:
- **Responsividade**: Se o menu móvel flui suavemente e não causa rolagem horizontal.
- **Miller's & Von Restorff Laws**: Se o menu está limpo (máximo de 7 elementos visuais) e o botão principal (CTA) se destaca corretamente.
- **Micro-interações**: Se os botões possuem transições fluidas no hover (`duration-200` ou `ease-out`) e um toque de escala física no clique (`hover:scale-105 active:scale-95`).

---

## 📜 Regras de Ouro e Diretrizes Estéticas que o Agente Segue

Ao projetar componentes com este agente, ele sempre aplicará os seguintes princípios:

| Princípio | Aplicação Prática |
| :--- | :--- |
| **Responsividade Impecável** | O design é pensado de baixo para cima (mobile-first). Imagens e grids se empilham perfeitamente a 360px. |
| **Bordas Inteligentes** | Bordas afiadas e elegantes (`0px` a `2px`) para dashboards e ERPs técnicos de alta performance; bordas arredondadas e amigáveis (`16px` a `32px`) para cards de marketing. Evitamos o arredondado padrão clichê de 8px. |
| **Purple Ban Ativo** | Cores roxas/violetas são proibidas como padrão. O agente usará paletas customizadas vibrantes (como verde ácido, cinzas premium e laranja mecânico) para garantir originalidade. |
| **Animações Otimizadas** | Transições de cor, opacidade e translação animadas com física natural (`cubic-bezier`) e rodando 100% sob aceleração de hardware (GPU). |
