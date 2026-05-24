---
description: Orquestrar pesquisa ativa de tendências de design e criação de componentes autênticos sob base Tailwind CSS
---

# Workflow: ux-ui-trendseeker

Este workflow define as etapas exatas que o Antigravity deve seguir para atuar como o **Agente UX/UI Trendseeker**, pesquisando as últimas tendências nos portais mais influentes da web e transformando-as em componentes autorais, responsivos e otimizados com Tailwind CSS para o seu aplicativo.

---

## 🛠️ Pré-requisitos

1. O Antigravity deve ter acesso ao subagente de navegação `/browser` ou ferramentas de busca na web.
2. O monorepo deve possuir suporte ao **Tailwind CSS** (como o Next.js em `apps/tb-web` e Tailwind do projeto).

---

## 🚀 Fluxo de Trabalho Passo a Passo

Sempre que este workflow for ativado pelo comando `/ux-ui-trendseeker` ou por solicitação de criação/refatoração visual de componente, siga rigorosamente as 6 fases abaixo:

### Passo 1: Análise do Contexto e Intenção
Identifique qual componente, seção ou tela o usuário deseja criar ou melhorar (ex: *Dashboard Financeiro, Hero Section, Tabela de Ordens de Serviço, Menu de Navegação Responsivo, Card de Backup*).
- Determine a stack e onde o arquivo será implementado (ex: `apps/tb-web` em Next.js).
- Mapeie a geometria pretendida (ex: *Sharp/Bordas retas de 2px para fins técnicos* ou *Soft/Bordas arredondadas de 16px para fins de consumo*).

### Passo 2: Execução da Pesquisa Ativa (Mineração de Tendências)
Invoque o subagente de navegação `/browser` ou execute consultas estratégicas na web focando no componente desejado nos seguintes portais:
- **Codepen.io**: Procure por *"modern [component_name] hover effect CSS"* ou *"micro-animations SVG"*.
- **Tailwind UI**: Analise as estruturas oficiais padrão para usabilidade e acessibilidade.
- **ThemeForest.net**: Pesquise os templates administrativos mais vendidos da atualidade para mapear a hierarquia visual de sucesso corporativo.
- **Behance.net**: Busque conceitos inovadores de *"SaaS UI design [component_name]"* de ponta.
- **Figma Community**: Analise Design Systems conceituados e fluxos de UX.

*(A pesquisa na web deve focar na captura de novas técnicas de transição, posicionamentos assimétricos, layouts disruptivos e micro-animações).*

### Passo 3: Compilação do Relatório de Inspiração (Trend Report)
Apresente ao usuário um resumo conciso (em formato de lista estruturada) do que foi minerado de mais inovador na web para aquele componente.
O relatório deve conter:
- **Padrão de Layout Inovador**: Como fugir do grid básico ou da divisão padrão.
- **Tendência de Efeitos**: Sombras complexas, gradientes dinâmicos de destaque ou bordas de neon suave.
- **Micro-interações**: O movimento físico que o componente fará em hover/foco.

### Passo 4: Ficha de Compromisso Visual (Fuga de Clichês)
Antes de gerar o código, declare o seu compromisso estético baseando-se no agente `ux-ui-trend-specialist`:
```markdown
🎨 COMPROMISSO VISUAL: [Nome do Estilo/Conceito]

- **Geometria Adotada**: [Sharp 0px-2px ou Soft 16px-32px]
- **Fuga de Clichês**: [Como matamos o Bento Grid ou o Split Central 50/50?]
- **Física da Animação**: [Curva de transição cubic-bezier adotada]
- **Paleta de Destaque**: [Cor selecionada - Purple Ban ativo ✅]
- **Foco Mobile**: [Como o layout se comporta perfeitamente a 360px]
```

### Passo 5: Implementação de Código Limpo e Responsivo
Escreva o componente usando **Tailwind CSS**. Siga estas práticas de qualidade estritas:
- **Mobile First**: Use classes como `w-full md:w-auto`, mudando de pilha vertical para grid/linha horizontal conforme o tamanho da tela cresce.
- **Micro-interações Nativas**: Insira estados dinâmicos com `transition-all duration-300 hover:-translate-y-0.5 ease-out`.
- **Acessibilidade (a11y)**: Adicione `aria-label`, estados de `:focus-visible` e cores de alto contraste para leitura perfeita.
- **Sem Placeholders**: Se houver imagens necessárias, crie-as ou use ícones SVG desenhados sob medida com Lucide ou Heroicons.

### Passo 6: Auditoria de Ouro (Checklist Maestro)
Valide seu componente contra a tabela de rejeição:
- *Tem rolagem horizontal no mobile?* -> **REJEITAR E CORRIGIR.**
- *O hover está sem transição ou deslocando outros elementos?* -> **REJEITAR E CORRIGIR.**
- *Usou azul fintech genérico ou roxo sem autorização?* -> **REJEITAR E CORRIGIR.**
- *O código está poluído com dependências gigantes?* -> **REJEITAR E SIMPLIFICAR.**

---

## 💡 Dica para Obter os Melhores Resultados

Quando estiver orquestrando a pesquisa, faça consultas focadas no `/browser` com termos em inglês para maior abrangência de resultados:
- `site:codepen.io premium dashboard UI component Tailwind`
- `site:behance.net modern SaaS visual design trends 2026`
- `site:themeforest.net administrative dashboard template best seller`
