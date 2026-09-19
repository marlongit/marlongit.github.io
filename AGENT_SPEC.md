# Especificação para reprodução por agente de IA

## 1. Papel
Você é um Senior UX/UI Designer + Frontend Engineer especializado em portfólios profissionais, acessibilidade WCAG, responsive design e GitHub Pages.

## 2. Fonte de verdade
Use o currículo PDF fornecido pelo usuário como fonte principal para:
- nome;
- resumo;
- experiência;
- datas;
- empresas;
- responsabilidades;
- formação;
- certificações/cursos;
- competências;
- idioma;
- contatos.

Não invente métricas, cargos, empresas, certificações ou tecnologias. Se uma informação não estiver na fonte, não crie uma versão factual dela.

## 3. Objetivo de produto
Transformar `marlongit.github.io` em um currículo digital:
- profissional;
- contemporâneo;
- rápido;
- acessível;
- responsivo;
- interativo sem excesso de animações;
- adequado para recrutadores, Engineering Managers e contatos profissionais;
- pronto para impressão/PDF;
- adequado para GitHub Pages.

## 4. Arquitetura de informação
Ordem recomendada:
1. Hero / identidade profissional
2. Indicadores de carreira
3. About / resumo
4. Experience / timeline
5. Technical Skills / filtros
6. Education & Certifications
7. Contact
8. Footer

## 5. Direção visual
- Estética: editorial tech / premium engineering.
- Base escura com acentos cyan/violeta.
- Tema claro opcional.
- Tipografia: Inter para texto; JetBrains Mono para metadados técnicos.
- Cards discretos, bordas sutis, alto contraste.
- Evitar excesso de gradientes, glassmorphism pesado ou animações decorativas.
- Espaçamento generoso.
- Hierarquia tipográfica forte.

## 6. Responsividade
Breakpoints sugeridos:
- desktop: > 900px;
- tablet: 701–900px;
- mobile: <= 700px.

O layout deve funcionar em:
- 320px;
- 375px;
- 390px;
- 430px;
- 768px;
- 1024px;
- 1280px;
- 1440px+.

Não usar largura fixa para o conteúdo principal.

## 7. Acessibilidade
Obrigatório:
- `lang="en"` ou idioma efetivamente usado pela interface;
- HTML semântico;
- skip link;
- foco visível;
- navegação por teclado;
- labels/nomes acessíveis em controles;
- `aria-expanded` para menu;
- `aria-pressed` para filtros;
- `aria-live` para feedback;
- contraste adequado;
- `prefers-reduced-motion`;
- não depender apenas de cor para transmitir informação;
- links externos com `rel="noopener noreferrer"`.

## 8. Interações
Manter apenas interações que aumentem utilidade:
- menu mobile;
- tema claro/escuro;
- filtros de skills;
- barra de progresso;
- voltar ao topo;
- impressão/salvar PDF;
- copiar e-mail;
- links profissionais.

## 9. Performance
Preferir:
- HTML/CSS/JS vanilla;
- nenhum framework obrigatório;
- nenhuma dependência npm;
- nenhuma imagem pesada;
- fontes externas opcionais;
- assets locais quando adicionados futuramente;
- scripts no final do body ou `defer`;
- evitar bibliotecas para interações simples.

## 10. SEO
Incluir:
- `title`;
- `meta description`;
- `meta viewport`;
- Open Graph básico;
- JSON-LD `Person`;
- URLs canônicas quando houver domínio definitivo.

## 11. Segurança
- HTTPS para todos os recursos externos.
- `noopener noreferrer` em links externos com `target="_blank"`.
- Não inserir chaves, tokens ou credenciais.
- Não utilizar APIs secretas no frontend.
- Não colocar informações que não sejam destinadas a publicação pública.

## 12. GitHub Pages
O projeto deve funcionar como site estático.
O arquivo de entrada deve ser `index.html` na raiz da fonte publicada.
Não depender de PHP, Python, banco de dados ou servidor.
Se não houver necessidade de Jekyll, usar `.nojekyll`.

## 13. Critérios de aceite
O agente deve validar:
- página abre sem erros;
- menu mobile funciona;
- tema funciona e persiste;
- filtros de skills funcionam;
- impressão funciona;
- links não estão quebrados;
- teclado consegue acessar todos os controles;
- layout não cria scroll horizontal em 320px;
- texto permanece legível;
- conteúdo do CV permanece fiel à fonte;
- site funciona sem JavaScript para leitura básica do currículo.

## 14. Evolução futura
Possíveis extensões, somente se desejadas:
- página `/projects`;
- página `/articles`;
- projetos do GitHub via API pública;
- botão de download de PDF;
- versão PT-BR/EN com seletor de idioma;
- página 404 visual;
- sitemap/robots;
- testes automatizados Lighthouse/axe.
