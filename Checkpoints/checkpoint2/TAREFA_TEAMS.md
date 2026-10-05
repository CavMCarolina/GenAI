# Aula 10 - Checkpoint - Contexto Longo

## Objetivo
Reduzir um contexto de aproximadamente 40 mil tokens e obter uma resposta correta de um LLM sem ultrapassar os limites definidos.

## O que fazer
1. Extraia o ZIP e abra `atividade.ipynb`.
2. Execute as celulas na ordem e observe a falha inicial.
3. Implemente somente `reduzir_contexto(documentos, pergunta, orcamento)`.
4. Obtenha 100% de cobertura em `avaliar_solucao` com no maximo 5.000 tokens de contexto.
5. Chame o OpenRouter e obtenha aprovacao em `avaliar_resposta_llm`.
6. Aplique a mesma funcao ao exemplo LongBench sem usar `answers` na selecao.
7. Obtenha aprovacao em `avaliar_longbench` e preencha a conclusao.

## Regras
- Nao altere os limites de 5.000 tokens de contexto, 6.000 de entrada total e 400 de saida.
- Nao use `FATOS_CRITICOS` dentro de `reduzir_contexto`.
- Nao envie o dossie completo ao LLM.
- Nao inclua a chave da API na entrega.

## Entrega
Envie somente `atividade.ipynb` executado, contendo os dois cenarios, respostas reais do LLM, avaliacoes e conclusao.

## Rubrica
- Funcao de reducao implementada: 2,0 pontos.
- Cenario Aurora dentro do limite e com cobertura local de 100%: 2,0 pontos.
- Resposta Aurora aprovada: 1,5 ponto.
- LongBench dentro do limite e sem uso de `answers` na selecao: 1,5 ponto.
- Resposta LongBench aprovada: 1,5 ponto.
- Conclusao comparativa: 1,0 ponto.
- Seguranca e organizacao: 0,5 ponto.
