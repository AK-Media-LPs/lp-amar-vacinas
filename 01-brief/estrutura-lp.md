# Estrutura da landing page — Amar Vacinas

> Ordem das seções, elemento-assinatura e o que anima em cada momento.
> É o roteiro de construção — o Claude Design segue esta ordem.

## Regras estruturais (inegociáveis)
- Uma página, um objetivo: captura de lead (formulário/WhatsApp).
- 3 CTAs com a mesma ação (hero, meio, final) — textos em `01-brief/copy.md`, nunca repetir a mesma frase.
- Sem menu de navegação, sem links de fuga que compitam com o CTA.
- Mobile-first, tipografia fluida, touch targets ≥ 48px.

## Para onde os CTAs apontam
Todo botão de CTA da landing aponta pra este link do WhatsApp (já com a mensagem pré-preenchida).

```
https://wa.me/558699334058?text=Ol%C3%A1!%20Vim%20pelo%20site%20e%20quero%20agendar.%20Pode%20me%20ajudar%3F
```

(abrir em nova aba: `target="_blank" rel="noopener"`)
Detalhes e checagem final em `05-tracking/LEIA-ME.md`.

## Elemento-assinatura (o personagem visual recorrente)
A 'Trilha da Caderneta': uma linha fina pontilhada com marcadores circulares (representando cada dose do calendário vacinal) que corre discretamente pela página, acompanhada pelo Mascote da marca flutuando sobre ela como quem guia a mãe pelo caminho. Entra cedo no hero: trilha ainda apagada (cinza-azulada), mascote no ponto de partida, quieto e observando o título. Na seção Problema, a trilha permanece apagada e o mascote assume postura empática/preocupada ao lado dos cards de dor (sem exagero cômico). Na seção Solução — momento pinado da página — a trilha se desenha progressivamente (stroke que se acende em Azul Amar) sincronizada com a passagem dos 3 passos, e o mascote 'caminha' sobre ela, virando-se para apontar o próximo passo. Na Prova Social a trilha já está quase completa, acendendo marcador a marcador junto aos stats que sobem. Resolve-se no CTA final: trilha 100% preenchida atrás do título, mascote em pose de celebração calma ao lado do botão, com um leve gesto de apontar para o CTA e para o formulário — o arco fecha como 'calendário organizado, missão cumprida'. No mobile a trilha simplifica para uma versão vertical curta com no máximo 4 marcadores e o mascote reduz a amplitude de movimento (idle quase estático) para não pesar performance.

## Ordem das seções

### 1. Hero
Fundo Branco Puro, layout split assimétrico ~60/40: headline (linha1 leve + linha2 em Azul Amar) e subheadline à esquerda, foto real da Enf. Antonia com recorte de borda suave à direita (asset fornecido, não gerado) com o Mascote pequeno ao canto inferior olhando para o CTA. CTA principal em pílula Azul Amar + cta_hint abaixo em Public Sans discreto. Trilha da Caderneta nasce aqui, ainda apagada.

**O que anima:** Mask reveal na headline linha a linha; mascote em idle float leve; trilha aparece como traço fino estático (ainda não acesa); CTA com hover elevação sutil.

### 2. Problema — a rotina de mãe que decide sozinha
Fundo Névoa Azulada #F5F7FF para marcar a primeira quebra de tom da página. Kicker + título centralizados, seguidos de 3 cards de dor em grid assimétrico (primeiro card ocupa 1.4x a largura dos outros dois, quebrando a grade previsível de 3 colunas iguais). Mascote pequeno com expressão empática no canto, sem competir com o texto.

**O que anima:** Cards entram com leve slide+fade escalonado ao scroll; parallax leve de 2 camadas entre fundo e cards; trilha permanece apagada nesta seção (contraste narrativo com a Solução).

### 3. Solução — do balcão anônimo ao colo de confiança (seção pinada)
Momento de maior orçamento de ousadia da página: container pinado full-viewport onde os 3 passos aparecem lateralmente conforme o usuário scrolla, com fundo transicionando de Branco Puro para Azul Suave. CTA do meio ('Quero falar com a Enf. Antonia agora') ao final do pin, mascote apontando para ele.

**O que anima:** Scroll-driven pin: trilha se desenha (stroke-dashoffset) e acende marcador a marcador em sincronia com cada passo; fundo faz transição de cor gradual (não gradiente diagonal, transição sólida cross-fade); mascote caminha sobre a trilha e vira-se para apontar o próximo passo; ao final, gesto de apontar para o CTA do meio.

### 4. Quem cuida do seu filho — Enf. Antonia de Maria
Seção de autoridade, full-bleed fora do grid padrão: foto real e grande da Enf. Antonia ocupando ~55% da viewport à esquerda (assimétrico), fundo Azul Profundo #22317E à direita com nome, título profissional e COREN em destaque tipográfico (Public Sans 600 uppercase), reforçando 'responsável técnica identificada' exigido por compliance. Texto de proximidade/segurança em branco sobre o azul profundo.

**O que anima:** Foto entra com leve reveal de máscara (cortina que sobe); texto com mask reveal linha a linha; trilha passa discretamente pelo rodapé da seção, quase totalmente acesa a esta altura.

### 5. Prova social — mães que já confiam aqui
Fundo Branco Puro. Kicker+título, seguidos de fileira de stats com tratamento editorial (o '0' de 'minuto de fila' como peça isolada em Azul Amar, os outros dois stats menores), depoimentos em cards horizontais com aspas em Fraunces itálico, e fileira de selos (COREN, cadeia de frio, atendimento acolhedor) em pílulas Azul Suave.

**O que anima:** Stats fazem count-up ao entrar em viewport (uma vez); trilha acende os últimos marcadores em sincronia com o count-up; depoimentos só fade+slide curto (seção deliberadamente mais quieta que a Solução).

### 6. CTA final
Fundo Azul Profundo full-bleed, trilha 100% preenchida e visível como textura de fundo atrás do título. Título+texto em branco, botão CTA em pílula branca com label Azul Amar (inversão de contraste para fechar com força), risk_reversal abaixo do botão, formulário compacto (nome, WhatsApp, idade da criança opcional) com microcopy LGPD explícita — sem qualquer campo de saúde/diagnóstico. Mascote em pose de celebração calma ao lado do botão.

**O que anima:** Mask reveal no título; mascote com micro-gesto de destaque apontando para o botão e para o formulário; trilha estática e completa (resolução do arco, sem mais movimento de desenho); formulário sem animação de entrada elaborada, só foco de campo.

## Direção geral de motion
Baseline scroll-driven: a Trilha da Caderneta é desenhada via stroke-dashoffset atado ao progresso de scroll (não é reveal de entrada, é movimento contínuo com o scroll), e o mascote tem flutuação/respiração sutil em idle (translateY de poucos px, 3-4s de ciclo) com fallback totalmente estático quando prefers-reduced-motion está ativo. Momento pinado único (orçamento de ousadia): a seção Solução — container fixo na viewport enquanto os 3 passos avançam lateralmente e a trilha se acende passo a passo, com o fundo transicionando de Branco Puro para Azul Suave conforme o progresso; ao final do pin, o mascote aponta para o CTA do meio. Mask reveal em headlines: título do hero e títulos de seção revelados por clip-path linha a linha (não fade simples). Parallax leve de 2 camadas entre fundo Névoa e cards de dor. Contadores (stats) sobem em count-up só na primeira entrada em viewport, uma vez. O que fica quieto: cards de depoimento (apenas fade+slide curto), formulário (sem animação de entrada elaborada, só foco de campo), footer estático — motion orquestrado com 1-2 movimentos-âncora por seção, nunca efeito repetido em tudo.
