# Marlongit.github.io — CV / Portfolio refresh

## Objetivo
Substituir a página atual do `marlongit.github.io` por um currículo digital moderno, acessível, responsivo e interativo, sem depender de backend.

## Arquivos
- `index.html` — página completa, autocontida: HTML + CSS + JavaScript + SEO/JSON-LD.
- `.nojekyll` — evita processamento Jekyll quando a publicação é feita como site estático.
- `404.html` — fallback simples para URLs inexistentes.
- `AGENT_SPEC.md` — especificação para um agente de IA reproduzir, manter ou evoluir o layout.

## Deploy no GitHub Pages
1. Abra o repositório que publica `marlongit.github.io`.
2. Faça backup da versão atual.
3. Substitua/adicone `index.html` na raiz da fonte de publicação.
4. Adicione `.nojekyll` na raiz se o site for servido como arquivos estáticos sem Jekyll.
5. Faça commit/push.
6. Em Settings > Pages, confirme a branch/pasta de publicação.
7. Aguarde a publicação e valide em desktop, tablet e celular.

## Princípios de UX/UI implementados
- Mobile-first e layout fluido.
- HTML semântico (`header`, `nav`, `main`, `section`, `article`, `footer`).
- Skip link para teclado.
- Estados `:focus-visible`.
- Contraste baseado em variáveis de tema.
- Tema claro/escuro persistido no `localStorage`.
- Navegação mobile com `aria-expanded`.
- Filtros de skills com `aria-pressed`.
- `prefers-reduced-motion`.
- Impressão / salvar como PDF via navegador.
- Barra de progresso de leitura.
- Botão voltar ao topo.
- Cópia do e-mail usando Clipboard API com fallback visual.
- JSON-LD para `Person`.
- Sem frameworks ou build obrigatório.
- Sem imagens externas obrigatórias.

## Conteúdo
O conteúdo profissional foi estruturado a partir do PDF de currículo fornecido para esta conversa. Não foram adicionadas experiências profissionais não presentes no documento.
Brach: Tinypress
Repositório de código aberto utilizando o Tinypress

