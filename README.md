# Elevação Topográfica como Parâmetro para o Geofencing Ambiental de VANTs

Repositório contendo o notebook experimental utilizado no artigo *"Elevação Topográfica como Parâmetro para o Geofencing Ambiental de VANTs: Uma Análise Estatística da Cobertura Florestal"* (UFSCar – Campus Sorocaba).

## Conjunto de Dados
* **Nome:** Covertype (UCI Machine Learning Repository – ID 31)
* **DOI:** `10.24432/C50K5N`
* **Licença:** CC BY 4.0
* **Instâncias:** 581.012 registros (sem valores ausentes)

## Estrutura do Repositório
* `analise_elevacao_geofencing_vants.ipynb`: Notebook Python com a extração dos dados, análise exploratória, teste de Levene, ANOVA clássica e de Welch, cálculo de tamanho de efeito ($\eta^2$), implementação do teste *post-hoc* de Games-Howell, treinamento da Árvore de Decisão rasa (`max_depth=3`, `random_state=42`) e geração dos gráficos.

## Requisitos e Execução
O experimento foi desenvolvido em **Python 3.12** (Google Colab). Para executar localmente:

```bash
pip install ucimlrepo pandas==2.2.2 numpy==2.0.2 scipy==1.16.3 scikit-learn==1.6.1 matplotlib seaborn
