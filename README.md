# Predição do Campeonato Brasileiro por Monte Carlo

Projeto desenvolvido para a disciplina **ME524 – Computação Aplicada a Estatística**, da UNICAMP.

O objetivo é utilizar **simulação de Monte Carlo** para prever possíveis resultados do Campeonato Brasileiro de 2026 a partir dos resultados já realizados.

## 🏆 Sobre o projeto

Foram utilizados os resultados de **246 das 380 partidas** do Campeonato Brasileiro realizadas até 03/09/2026. A partir desses dados, foram estimados parâmetros de gols marcados e sofridos para cada equipe e simuladas as partidas restantes do campeonato.

O modelo foi baseado em distribuições de **Poisson**, e foram realizadas **10.000 simulações de Monte Carlo** para estimar:

* Probabilidade de cada equipe conquistar o título;
* Probabilidade de rebaixamento;
* Probabilidade de ocorrência de empates na classificação;
* Pontuação esperada do campeão;
* Pontuações associadas a determinadas probabilidades de título e permanência na Série A.

Também foi utilizado **Bootstrap**, com 2.000 reamostragens por equipe, para avaliar a variabilidade das estimativas de gols marcados e sofridos.

## ⚽ Modelo com mando de campo

Como extensão, foi desenvolvido um modelo que incorpora fatores de desempenho **como mandante e visitante**, ajustando as taxas esperadas de gols de acordo com esses efeitos. Foram realizadas novamente 10.000 simulações para comparação com o modelo original.

## 🛠️ Tecnologias

* Python
* Pandas
* NumPy
* Matplotlib
* SciPy
* Simulação de Monte Carlo
* Bootstrap

## 📊 Principais resultados

No modelo original, Flamengo e Palmeiras concentraram **96,5%** das simulações de título. A pontuação esperada do campeão foi de **76,82 pontos**.

As simulações também indicaram que:

* **79 pontos** correspondem a uma probabilidade estimada de pelo menos 90% de título;
* **41 pontos** correspondem a uma probabilidade estimada de pelo menos 95% de não ser rebaixado.

A comparação com o modelo que incorpora os efeitos de mando e visitante mostrou mudanças relevantes nas probabilidades estimadas entre as principais equipes.

## 👩‍💻 Autores

**Iuri Santos Oliveira**
**Julia Folgueral**
**Luiz Fernando de Oliveira Pereira**

Universidade Estadual de Campinas (UNICAMP)
Instituto de Matemática, Estatística e Computação Científica
ME524 – Computação Aplicada a Estatística

---

*Projeto desenvolvido em maio de 2026.*
