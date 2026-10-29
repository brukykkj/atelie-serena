# Ateliê Serena

Projeto de demonstração: landing page de um ateliê de beleza especializado em **sobrancelhas, cílios e estética facial**, com foco em atendimento personalizado e agendamento direto pelo WhatsApp.

## Funcionalidades

- Seções de início, serviços (com tabela de preços), portfólio, avaliações e localização
- Botões de agendamento que abrem o WhatsApp com mensagem pré-preenchida do serviço escolhido
- Mapa do Google Maps incorporado
- Layout responsivo (mobile first) e botão flutuante de WhatsApp
- Site estático: sem build, sem dependências

## Tecnologias

HTML5, CSS3 e JavaScript puro. Única dependência externa: fontes do Google Fonts (DM Sans e Playfair Display).

## Estrutura

```
.
├── index.html                    # página principal (HTML + CSS + JS)
├── politica-de-privacidade.html  # política de privacidade (exemplo)
├── termos-de-uso.html            # termos de uso (exemplo)
├── 404.html                      # página de erro personalizada
├── css/pages.css                 # estilos das páginas internas
├── img/                          # imagens do portfólio
└── README.md
```

## Rodando localmente

Basta abrir o `index.html` no navegador. Opcionalmente, com um servidor local:

```bash
python -m http.server 8000
# acesse http://localhost:8000
```

## Personalização

- **Número do WhatsApp:** altere a constante `WHATSAPP_NUMBER` no final do `index.html` (formato DDI + DDD + número, só dígitos, ex.: `5562993030110`).
- **Serviços e preços:** edite os cards `.service-card` em `index.html`.
- **Imagens:** substitua os arquivos em `img/` mantendo os nomes, ou atualize os `src` no HTML.

## Publicação (GitHub Pages)

O site é publicado gratuitamente pelo GitHub Pages a partir da branch `main`:

1. No repositório, vá em **Settings → Pages**.
2. Em **Build and deployment**, escolha **Deploy from a branch**.
3. Selecione a branch `main` e a pasta `/ (root)` e clique em **Save**.
4. Após cerca de 1 minuto o site estará em `https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO/`.

## Licença

Todos os direitos reservados. Defina uma licença caso queira permitir o reuso do código.
