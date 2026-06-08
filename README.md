# Connecting the Dots

> *Um diagnóstico comportamental de alta fidelidade para jovens de 17 a 24 anos.*

**Connecting the Dots** é uma experiência de autoconhecimento interativa construída como uma única página (`index.html`) — sem dependências externas, sem banco de dados, sem servidor. Abre direto no browser.

---

## Demo

Basta abrir `index.html` no navegador. Nenhuma instalação necessária.

Para publicar via **GitHub Pages**:

1. Acesse **Settings → Pages**
2. Em *Source*, selecione o branch `main` e a pasta `/ (root)`
3. Salve — o link estará disponível em `https://<seu-usuario>.github.io/<repositorio>/`

---

## O que é

Um teste de perfil comportamental com três atos:

| Fase | Descrição |
|------|-----------|
| **18 perguntas** | Situações de decisão reais — sem respostas certas ou erradas |
| **3 dinâmicas interativas** | Três pausas que capturam o que perguntas diretas não conseguem |
| **Resultado completo** | Perfil principal, traço secundário, pontuações e guia de relacionamento |

---

## Os 4 Arquétipos

| Arquétipo | Tagline |
|-----------|---------|
| 🛡️ **O Guardião** | Você constrói sistemas que sobrevivem a você. |
| ⚡ **O Catalisador** | Você não gerencia pessoas. Você ativa o que elas já são. |
| 🔭 **O Visionário** | Você não resolve problemas. Você dissolve as condições que os geram. |
| 🚀 **O Acelerador** | Você não espera pelas condições ideais. Você as cria enquanto se move. |

Cada resultado inclui: descrição do perfil, traço secundário (quando relevante), barra de pontuações por arquétipo, ações concretas para a semana e um **guia de relacionamento** com os outros três perfis.

---

## As 3 Dinâmicas

### 1 · Três Movimentos
Três dimensões comportamentais capturadas de forma não-declarativa:

- **Espectro Cognitivo** — slider nativo de estrutura ↔ complexidade
- **Calibração Social** — escala de 5 pontos: decisão autônoma ↔ sensível ao grupo
- **Orientação Temporal** — 4 cards: passado / presente / futuro próximo / futuro estratégico

### 2 · Gravidade
Quatro esferas (PROCESSO, PESSOAS, ESTRATÉGIA, PERFORMANCE) distribuídas em **4 órbitas concêntricas**. O usuário clica para avançar de órbita; se a órbita de destino estiver ocupada, as esferas trocam de lugar (swap). Sem empates. Pontuação calculada **apenas uma vez**, na confirmação — bug de acúmulo eliminado.

### 3 · Trajetória
*(integrada ao fluxo após a pergunta 15)*

---

## Estrutura do projeto

```
connecting-the-dots/
├── index.html        ← tudo em um único arquivo
└── README.md
```

Toda a lógica — HTML, CSS, JavaScript, dados das perguntas, traduções e conteúdo dos resultados — está contida em `index.html`. Não há bundler, framework ou dependência de npm.

**Dependências externas carregadas via CDN:**
- Google Fonts: `Cormorant Garamond` + `DM Sans`
- Nenhuma outra biblioteca

---

## Funcionalidades

- ✅ **Zero dependências** de npm ou build tools
- ✅ **Multilíngue** — Português (padrão), English, Español
- ✅ **Responsivo** — mobile, tablet e desktop
- ✅ **Canvas animado** — estrelas e constelação de fundo
- ✅ **Micro revelação** — pausa narrativa entre blocos de perguntas
- ✅ **Guia de relacionamento** — como cada perfil se relaciona com os outros três
- ✅ **Resultado dinâmico** — gerado em tempo real com base nos pontos acumulados
- ✅ **Sem cookies, sem tracking, sem analytics**

---

## Pontuação

O sistema acumula pontos em quatro variáveis (`C`, `M`, `E`, `K`) ao longo de toda a experiência:

| Fonte | Peso máximo |
|-------|-------------|
| 18 perguntas | ~18 pts (1 pt por pergunta) |
| Três Movimentos | até ~2.2 pts |
| Gravidade (4 órbitas) | até 1.2 pts |
| Trajetória | variável |

O perfil com maior pontuação é o resultado principal. Se o segundo lugar tiver ≥ 4 pts, é exibido como traço secundário.

---

## Sobre o projeto

**Connecting the Dots** faz parte de um ecossistema maior de autoconhecimento comportamental voltado para jovens de 17 a 24 anos — a plataforma **Connecting the Dots**, desenvolvida com foco em inteligência emocional, identidade e desenvolvimento de carreira.

O teste foi construído do zero, com framework próprio baseado em:
- Teoria de identidade narrativa (McAdams)
- Autoeficácia (Bandura)
- Pesquisa em meaning-making

---

## Licença

Todos os direitos reservados. Este repositório é público para fins de portfólio e demonstração. Não é permitido uso comercial ou redistribuição sem autorização.
