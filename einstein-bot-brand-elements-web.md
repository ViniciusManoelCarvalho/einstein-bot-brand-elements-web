# Einstein Bot — Elementos de Marca (Brand Elements) — Versão WEB

> **Escopo:** Este documento descreve o que pode ser alterado no visual do **Einstein Bot / Agentforce na janela de chat incorporada (Embedded Chat) da versão WEB** — ou seja, **Messaging for Web**.
> **Fonte base:** Salesforce Help — *Brand Elements* (`service.ec_brand_elements_2.htm`) + documentação Messaging for Web.
> Não cobre a versão **In-App (mobile)**, que tem configurações próprias.

A ideia dos *Brand Elements* é alinhar a experiência do chat (cores, fontes, ícones e logos) ao tom visual do seu site e da sua marca.

---

## 1. Cores (Color Settings)

As cores podem ser definidas escolhendo no seletor de cores ou digitando o código hexadecimal direto no campo `#`.

### Botão de Chat e Convites (Chat Button and Invitations)
| Elemento | O que controla |
|---|---|
| **Background** | Cor de fundo do botão de chat e do pop-up de convite automático |
| **Text** | Cor do texto do pop-up de convite automático |
| **Dismiss Invitation Button** | Cor do "✕" (fechar) nos pop-ups |

| Configuração | Exemplo |
|---|---|
| ![Configuração Chat Button and Invitation](imagens/Chat%20Button%20and%20Invitation.png) | ![Exemplo Chat Button and Invitation](imagens/Chat%20Button%20and%20Invitation%20Example.png) |

### Cabeçalho (Header)
| Elemento | O que controla |
|---|---|
| **Background** | Cor de fundo do cabeçalho |
| **Text and Navigation Icons** | Cor do texto do cabeçalho, do botão de minimizar e do ícone de menu |

| Configuração | Exemplo |
|---|---|
| ![Configuração Header](imagens/Header.png) | ![Exemplo Header](imagens/Header%20Example.png) |

### Agente de IA / Bot e Representante (AI Agent and Service Representative)
| Elemento | O que controla |
|---|---|
| **Background** | Fundo das mensagens, avatares e miniaturas iniciais |
| **Text** | Cor do texto do lado do agente de IA / bot |
| **Link** | Cor dos links no lado do agente de IA / bot |

| Configuração | Exemplo |
|---|---|
| ![Configuração AI Agent and Service Rep](imagens/AI%20Agent%20and%20Service%20REP.png) | ![Exemplo AI Agent and Service Rep](imagens/AI%20Agent%20and%20Service%20REP%20Example.png) |

### Usuário Final (End User)
| Elemento | O que controla |
|---|---|
| **Background** | Fundo das mensagens e miniaturas do usuário final |
| **Text** | Cor do texto do usuário final |
| **Link** | Cor dos links do usuário final |

| Configuração | Exemplo |
|---|---|
| ![Configuração End User](imagens/End%20User.png) | ![Exemplo End User](imagens/End%20User%20Example.png) |

### Corpo da Conversa (Conversation Body)
| Elemento | O que controla |
|---|---|
| **Text** | Cor do texto inserido pelo sistema e do corpo das mensagens do usuário |

| Configuração | Exemplo |
|---|---|
| ![Configuração Conversation Body](imagens/Conversation%20Body.png) | ![Exemplo Conversation Body](imagens/Conversation%20Body%20Example.png) |

### Rodapé (Footer)
| Elemento | O que controla |
|---|---|
| **Icon** | Cor dos ícones de anexo, emoji e enviar |
| **Footer** | Cor da borda do rodapé |

| Configuração | Exemplo |
|---|---|
| ![Configuração Footer](imagens/Footer.png) | ![Exemplo Footer](imagens/Footer%20Example.png) |

### Citações (Citations)
| Elemento | O que controla |
|---|---|
| **Background** | Cor de destaque do fundo da seção de título da fonte |
| **Text** | Cor do texto do título do link da fonte citada |

| Configuração | Exemplo |
|---|---|
| ![Configuração Citations](imagens/Citations.png) | ![Exemplo Citations](imagens/Citations%20Example.png) |

### Selos e Botões (Badges and Buttons)
| Elemento | O que controla |
|---|---|
| **Badge** | Cor do selo "ir para a mensagem mais recente" |
| **Button** | Cor do botão "Iniciar" e botões semelhantes |

| Configuração | Exemplo |
|---|---|
| ![Configuração Badges and Buttons](imagens/Badges%20and%20Buttons.png) | ![Exemplo Badges and Buttons](imagens/Badges%20and%20Buttons%20Example.png) |

---

## 2. Fontes (Font Settings)

| Configuração | Opções |
|---|---|
| **Seleção de Fonte** | 13 fontes pré-definidas (Arial, Georgia, Times New Roman, etc.) |
| **Fonte Personalizada** | Subir um *static resource* e informar o nome da família da fonte (font family) |
| **Tamanho da Fonte** | Pequeno (Small), Médio (Medium) ou Grande (Large) |

![Configuração de Fontes](imagens/Font.png)

---

## 3. Imagens (Image Settings)

| Elemento | O que controla |
|---|---|
| **Avatar do Representante (Service Representative Avatar)** | Imagem à esquerda das mensagens do atendente humano |
| **Avatar do Bot / Agente de IA (Bot and AI Agent Avatar)** | Imagem à esquerda das mensagens do bot / agente de IA |
| **Logo** | Logo exibido no cabeçalho do chat (recomendado formato quadrado) |
| **Chat Button** | Imagem exibida no próprio botão de chat |

Também é possível personalizar (em fluxos de pré-chat): imagem de fundo do pré-chat, logo, imagem de estado de espera (*waiting state*) e os avatares/fotos do atendente e do Einstein Bot.

![Configuração de Imagens](imagens/Images.png)

---

## 4. Tamanho da Janela de Chat (Chat Window Size)

| Dimensão | Mínimo | Padrão |
|---|---|---|
| **Largura (Width)** | 80 px | 320 px |
| **Altura (Height)** | 120 px | 480 px |

![Configuração de dimensões da janela de chat](imagens/Chat%20Window%20and%20Dimension.png)

---

## 5. Personalização Avançada do Cabeçalho (somente Web)

Na versão WEB é possível ir além das opções padrão e customizar o cabeçalho via código:

- **`customHeader.html`** — adiciona os componentes e botões do cabeçalho que serão renderizados na UI.
- **`customHeader.css`** — define o estilo (cores, espaçamento, etc.) desses componentes e botões.

> Isso permite um cabeçalho totalmente sob medida, recurso exclusivo da implementação Web (Enhanced/Lightning Web Components).

---

## Resumo rápido — o que dá pra mudar

- **Cores:** botão de chat, convites, cabeçalho, mensagens do bot, mensagens do usuário, links, corpo da conversa, rodapé/ícones, citações, selos e botões.
- **Fontes:** família (13 opções + personalizada) e tamanho.
- **Imagens:** avatar do atendente, avatar do bot/IA, logo do cabeçalho, imagem do botão de chat, imagens de pré-chat/espera.
- **Dimensões:** largura e altura da janela.
- **Cabeçalho (Web):** personalização total via `customHeader.html` + `customHeader.css`.

---

### Observações
- Este conteúdo refere-se à **versão WEB (Messaging for Web / Embedded Chat)**.
- A página oficial da Salesforce Help é carregada dinamicamente (JavaScript), por isso o conteúdo foi consolidado a partir da documentação da Salesforce e materiais de referência equivalentes.
- Recomenda-se conferir a página original para a sua versão/release específica:
  `https://help.salesforce.com/s/articleView?id=service.ec_brand_elements_2.htm&type=5`
