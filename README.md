<details>
<summary><strong>📍 Sobre</strong></summary>

O **Echo Music** é um projeto de análise de dados para antecipação de riscos em eventos públicos de grande porte. Utiliza dados sintéticos inspirados em fontes reais para detectar padrões associados a tumultos, crimes e situações de emergência. A proposta é contribuir com estratégias de prevenção em eventos como shows, festivais e grandes manifestações, por meio da análise de dados em tempo real.

</details>

<details>
<summary><strong>🚨 O problema</strong></summary>

Eventos públicos enfrentam desafios de segurança complexos, especialmente em grandes centros urbanos. Respostas tradicionais tendem a ser reativas. O Echo Music busca transformar esse cenário com soluções analíticas baseadas em dados, promovendo antecipação e monitoramento dinâmico.

</details>

<details>
<summary><strong>🔍 Fontes de dados e coleta</strong></summary>

Este projeto utiliza dados sintéticos simulando múltiplas fontes reais, incluindo:

- Redes sociais (Twitter, Facebook, Instagram)
- Câmeras públicas (CCTV, vídeos em tempo real)
- Transporte público (dados GTFS, mobilidade urbana)
- Dados meteorológicos (temperatura, chuva, vento)
- Histórico de crimes e ocorrências policiais
- Sensores urbanos (movimentação, ruído, luminosidade)
- Mapas geográficos e posicionamento por GPS

</details>

<details>
<summary><strong>📓 Acesso aos notebooks</strong></summary>

Os notebooks estão disponíveis na pasta `Notebooks Echo Music/`, e cobrem desde o pré-processamento até análises de sentimento e detecção de anomalias:

- `pre_processamento_dados.ipynb`
- `analise_sentimentos.ipynb`
- `detecção_anomalias.ipynb`
- `clustering_multidoes.ipynb`
- e outros

Para executar localmente:

```bash
git clone https://github.com/seu-usuario/echo-music.git
cd echo-music

python -m venv venv
source venv/bin/activate  # Linux/macOS
venv\Scripts\activate  # Windows

pip install -r requirements.txt
```

Abra os notebooks com Jupyter Lab ou Notebook:

```bash
jupyter lab
```

</details>

<details>
<summary><strong>📊 Insights</strong></summary>

<details>
<summary><strong>1. Redes sociais</strong></summary>

![Insight redes sociais](Visualizações/relatorio_redes_sociais.png)

**Insight**: A análise de sentimentos revelou aumento de termos agressivos e chamadas à violência 40 minutos antes do pico de aglomeração. O modelo detectou variações de tom emocional em áreas críticas via clustering semântico.

</details>

<details>
<summary><strong>2. Câmeras públicas</strong></summary>

![Insight câmeras públicas](Visualizações/relatorio_cameras.png)

**Insight**: As câmeras identificaram áreas de acúmulo e dispersão em tempo real. Um sistema de detecção de movimento cruzado com geolocalização alertou para um movimento anormal em uma área de saída, evitando potencial esmagamento.

</details>

<details>
<summary><strong>3. Transporte público</strong></summary>

![Insight transporte público](Visualizações/relatorio_transporte.png)

**Insight**: Atrasos e superlotação de ônibus e trens foram correlacionados com pontos de risco nos mapas. Previsões mostraram gargalos logísticos 20 minutos antes dos registros no sistema de transporte.

</details>

<details>
<summary><strong>4. Meteorologia</strong></summary>

![Insight meteorologia](Visualizações/relatorio_meteorologia.png)

**Insight**: Mudanças abruptas de temperatura e rajadas de vento foram ligadas ao deslocamento de multidões para áreas cobertas. A integração com previsão em tempo real gerou alertas preventivos.

</details>

<details>
<summary><strong>5. Histórico de crimes</strong></summary>

![Insight histórico de crimes](Visualizações/relatorio_ocorrencias.png)

**Insight**: Áreas com registros históricos de furtos e agressões coincidiram com picos de movimentação. Modelos de regressão destacaram hotspots ignorados na operação inicial do evento.

</details>

<details>
<summary><strong>6. Sensores urbanos</strong></summary>

![Insight sensores urbanos](Visualizações/relatorio_sensores.png)

**Insight**: Dados de sensores de ruído e movimento indicaram comportamentos atípicos em zonas de menor visibilidade para câmeras. A integração com clusters de tweets elevou a confiança de detecção.

</details>

<details>
<summary><strong>7. Mapas e localização</strong></summary>

![Insight mapas e localização](Visualizações/relatorio_mapas.png)

**Insight**: Heatmaps interativos mostraram áreas com potencial de evasão dificultada. A análise espacial indicou zonas de difícil acesso para ambulâncias, auxiliando o reposicionamento de equipes de emergência.

</details>

</details>
