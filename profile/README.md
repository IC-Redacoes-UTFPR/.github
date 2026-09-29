# IC Redações UTFPR

Iniciação Científica na UTFPR: **Correção Automática de Redações em Português com Modelos de Linguagem Pré-Treinados e Geração de Feedback Formativo**.

O objetivo é pontuar redações no formato do ENEM nas cinco competências (C1 a C5, de 0 a 200 cada) usando modelos de linguagem, e gerar feedback formativo que explique ao estudante onde e como melhorar.

## Equipe

- Yuri Matsumoto Santos, bolsista
- Monica Paula Oliveira Mackert
- Orientação: Profa. Eliane Maria De Bortoli Fávero

## Estado atual

- Base de dados: corpus essay-br, avaliação cross-prompt (temas do teste não vistos no ajuste), métrica principal QWK na nota total.
- Melhor configuração: Gemini Flash Lite pontuando uma competência por vez, com redações âncora como exemplo de cada faixa de nota, rubrica refinada da C5 e contagem de desvios do LanguageTool como apoio na C1. QWK de 0,63 na nota total (0,61 após correção de viés), contra 0,35 da primeira fase do projeto (modelos de 7B em zero-shot).
- Faixa publicada para o essay-br: QWK de 0,60 a 0,73.

## Repositório

- [CorrecaoRedacao](https://github.com/IC-Redacoes-UTFPR/CorrecaoRedacao): código, notebooks, resultados e o [log datado de experimentos](https://github.com/IC-Redacoes-UTFPR/CorrecaoRedacao/blob/main/docs/log_experimentos.md).
