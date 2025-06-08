<details>
<summary><strong>📍 Sobre</strong></summary>

O **Echo Music** é um projeto de análise de dados para antecipação de riscos em eventos públicos de grande porte. Utiliza dados sintéticos inspirados em fontes reais para detectar padrões associados a tumultos, crimes e situações de emergência. A proposta é contribuir com estratégias de prevenção em eventos como shows, festivais e grandes manifestações, por meio da análise de dados em tempo real.

</details>

<details>
<summary><strong>🚨 O problema</strong></summary>

**Problema e a justificativa do uso de dados.**

## Descrição detalhada do problema:

Grandes eventos públicos, como manifestações políticas, shows, jogos esportivos e festivais culturais, reúnem milhares ou até milhões de pessoas em um único local. Apesar da importância social e cultural desses eventos, eles também apresentam riscos elevados de tumultos, atos de violência, vandalismo e até ataques terroristas. A dificuldade está em monitorar, em tempo real, o comportamento de grandes multidões e antecipar situações que possam evoluir para crises de segurança.  
Além disso, a resposta das forças de segurança costuma ser reativa, ou seja, ocorre depois que o problema já se instalou, o que dificulta a contenção e aumenta os riscos para a população e para a infraestrutura local.

---

Eficiência do uso de análise de dados

* Estudos apontam que o uso de modelos preditivos e monitoramento em tempo real reduz em até 40% o tempo de resposta a incidentes em grandes eventos (fonte: International Association of Venue Managers).  
* A utilização de análise de sentimentos em redes sociais pode antecipar mobilizações ou comportamentos de risco com até 3 horas de antecedência (fonte: MIT Media Lab).

---

## Conclusão

Este projeto é altamente relevante porque:

* Atua preventivamente, não apenas de forma reativa.  
* Reduz riscos para meio milhão de pessoas em um único evento.  
* Pode ser replicado para outros eventos em larga escala no Brasil e no mundo.  
* Fortalece a confiança social na realização de eventos públicos seguros, estimulando a participação cidadã.

## Exemplo real:

Tentativa de atentado no show gratuito de Lady Gaga em Copacabana (2025).  
Em 3 de maio de 2025, Lady Gaga realizou um show gratuito na Praia de Copacabana, no Rio de Janeiro, que atraiu mais de 2 milhões de pessoas, tornando-se o maior evento da carreira da artista.  
Durante o evento, as autoridades brasileiras impediram um plano de ataque com coquetéis molotov e outros explosivos improvisados, que visava especificamente o público LGBTQIA+ e crianças. A operação de segurança, denominada "Operação Fake Monster", foi conduzida de forma sigilosa para evitar pânico entre os participantes. [BBC](https://www.bbc.com/portuguese/articles/c1drv6ey6gxo?utm_source=chatgpt.com)  
As investigações revelaram que o grupo responsável pelo plano disseminava discursos de ódio online e recrutava adolescentes para realizar os ataques. A polícia identificou e prendeu um homem no Rio Grande do Sul por posse ilegal de armas e um adolescente no Rio de Janeiro por posse de material pornográfico infantil.  
Como a análise de dados ajudou?  
A análise de dados desempenhou um papel fundamental na prevenção desse atentado:  
Monitoramento de redes sociais: As autoridades monitoraram ativamente redes sociais e aplicativos de mensagens para identificar postagens suspeitas e coordenar ações preventivas.  
Análise de padrões de comportamento: Através da análise de dados, foi possível identificar padrões de comportamento que indicavam a preparação de um ataque, permitindo uma resposta rápida e eficaz.  
Integração de informações: A colaboração entre diferentes agências de segurança e o uso compartilhado de dados foram essenciais para desarticular o plano de ataque de forma coordenada.

Graças a essas estratégias baseadas em dados, o evento transcorreu sem incidentes graves, garantindo a segurança do público e o sucesso do show.   

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
