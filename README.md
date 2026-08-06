# LP Amar Vacinas — Pacote de briefing (LUVRE)

> Gerado pelo LUVRE (TRACKR/AK Media) em 06/08/2026. Este repositório NÃO é a
> landing page — é o **pacote documental** pro Claude Design construir a
> landing page premium. Depois de pronta, a LP final volta pra este mesmo
> repositório (upload do ZIP no TRACKR) e o deploy sai daqui.

## O que tem aqui

| Pasta | Conteúdo |
| --- | --- |
| `01-brief/` | Pesquisa de mercado, copy completa e estrutura da página |
| `02-imagens/` | Imagens da página, nomeadas por uso |
| `03-referencias/` | VAZIA — você cura referências de EXECUÇÃO aqui (ver LEIA-ME) |
| `04-direcao-visual/` | Direção de design system do Diretor de Arte |
| `05-tracking/` | Códigos de head/body e destino do lead |

Cada pasta tem um `LEIA-ME.md` próprio explicando o que é e como usar.

## Passo a passo — levando este pacote ao Claude Design

**Antes de começar:** baixe as fontes (links abaixo) e, se quiser elevar o
nível de motion, preencha `03-referencias/` (o LEIA-ME de lá ensina).

### 1ª mensagem — construir o design system
Anexe: `04-direcao-visual/direcao-cliente.md` + `01-brief/pesquisa.md`.

Prompt sugerido:
> Você vai construir uma landing page premium. Antes de qualquer página,
> construa o design system a partir da direção anexada (direcao-cliente.md):
> tokens de cor, tipografia (par Fraunces + Public Sans), componentes e a linguagem
> de motion descrita. A pesquisa anexada dá o contexto de mercado. Me mostre
> o design system aplicado num trecho de exemplo antes de seguir.

### 2ª mensagem — construir a página
Anexe: `01-brief/copy.md` + `01-brief/estrutura-lp.md`.

Prompt sugerido:
> Agora construa a landing page completa com o design system aprovado.
> Siga a ordem de seções de estrutura-lp.md e use a copy de copy.md
> EXATAMENTE como está (não reescreva textos). O elemento-assinatura e o
> plano de animação estão em estrutura-lp.md.
> Todos os CTAs apontam para: https://wa.me/558699334058?text=Ol%C3%A1!%20Vim%20pelo%20site%20e%20quero%20agendar.%20Pode%20me%20ajudar%3F

### 3ª mensagem (opcional) — elevar a execução
Anexe: o conteúdo que você curou em `03-referencias/`.

Prompt sugerido:
> Estas são referências de EXECUÇÃO (nível de motion/qualidade) — não de
> estética. Eleve as animações da página pra este nível, mantendo o design
> system como está.

### 4º passo — revisar e fechar
- Revise a prova social (pode conter depoimentos/números fictícios plausíveis
  — substitua por dados reais do cliente antes de publicar).
- Confira se todo CTA aponta pra ação certa: `https://wa.me/558699334058?text=Ol%C3%A1!%20Vim%20pelo%20site%20e%20quero%20agendar.%20Pode%20me%20ajudar%3F` (ver `05-tracking/LEIA-ME.md`).
- Insira os códigos de `05-tracking/head.txt` e `body.txt` na página.

### 5º passo — publicar
Exporte o ZIP da página pronta no Claude Design e faça o upload na tela do
LUVRE no TRACKR (histórico → "Subir LP final"). O TRACKR normaliza o ZIP
(index.html na raiz) e publica neste repositório — o deploy (Vercel) sai daqui.

## Fontes deste projeto — Fraunces + Public Sans

| Fonte | Papel | Download | Licença |
| --- | --- | --- | --- |
| Fraunces | Display (headlines) | https://fonts.google.com/specimen/Fraunces | SIL Open Font License 1.1 (Google Fonts) |
| Public Sans | Texto (corpo) | https://fonts.google.com/specimen/Public+Sans | SIL Open Font License 1.1 (Google Fonts) |

## Resumo da direção
Acolhedor com autoridade clínica: a página deve parecer uma sala de atendimento clara e calma, não um posto de saúde nem uma clínica fria de metal e vidro. A promessa central — 'um rosto de confiança, não uma fila' — vira direção de arte: espaço em branco generoso, curvas suaves, tipografia serifada macia para dar calor humano, e um personagem-guia que acompanha a mãe como quem segura a mão dela no processo. Nada de urgência ou susto: o ritmo visual é o de quem tem tempo e cuidado, porque é exatamente isso que falta no posto público.
