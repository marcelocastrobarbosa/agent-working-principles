---
name: interface-design-direction
description: Oriente a criação, alteração e revisão de interfaces com coerência entre telas e estabilidade visual durante o carregamento. Use em trabalho de UI, incluindo componentes e estados assíncronos.
---

# Direção de design de interfaces

## Coerência do conjunto

Reconheça os padrões das telas e componentes relacionados antes de alterar a interface. Reutilize e consolide estruturas comuns, preservando diferenças intencionais. Avalie a mudança no contexto de seus consumidores e da navegação do produto, respeitando a identidade e a direção de design do projeto.

## Estabilidade durante o carregamento

O estado de carregamento deve preservar o espaço do componente e a posição do conteúdo ao redor. Ao substituir conteúdo já exibido, mantenha suas dimensões durante a espera. Na primeira carga, reserve um espaço coerente com a estrutura esperada. Isso vale para qualquer indicador de carregamento, incluindo fallbacks de `Suspense`.

Mudanças de tamanho devem decorrer do conteúdo real ou de uma interação, sem oscilações causadas pelo fallback. O conteúdo final pode crescer ou diminuir conforme sua necessidade; preserve o espaço durante a espera sem impor altura fixa permanente nem cortar conteúdo.

Por exemplo: um componente de 200 px deve manter esse espaço enquanto carrega, em vez de encolher para um indicador de 50 px e depois voltar. Se o novo conteúdo exigir 1.000 px, a expansão na chegada do conteúdo é legítima.

Verifique as transições de carregamento além do estado final, incluindo atualizações de conteúdo já visível, para identificar deslocamentos intermediários.
