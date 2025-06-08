<details>
<summary><strong>📍 Sobre</strong></summary>

O **Echo Music** é um projeto de análise de dados para antecipação de riscos em eventos públicos de grande porte. Utiliza dados sintéticos inspirados em fontes reais para detectar padrões associados a tumultos, crimes e situações de emergência. A proposta é contribuir com estratégias de prevenção em eventos como shows, festivais e grandes manifestações, por meio da análise de dados em tempo real.

</details>

<details>
<summary><strong>🚨 O problema</strong></summary>

# **Problema e a justificativa do uso de dados.**

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

# **Fontes de dados levantadas e o método de coleta**

## **Fontes de Dados Prioritárias para o Projeto**

### **1\. Redes Sociais** (Twitter/X, Instagram, Facebook, TikTok)

**Descrição:**  
Plataformas onde usuários publicam conteúdos em tempo real sobre eventos, incluindo textos, imagens, vídeos e localização.  
**Tipo de dados:**  
Não estruturados: textos, imagens, vídeos.  
Semi-estruturados: posts com metadados (data, hora, localização geográfica, hashtags).  
**Métodos de acesso e coleta:**

* API Oficial:  
  Twitter/X API: permite acesso a tweets públicos em tempo real, com filtros por    palavras-chave, hashtags ou geolocalização.  
  Meta Graph API: para publicações públicas no Instagram e Facebook.  
  TikTok: não possui API pública oficial para coleta em massa; pode ser necessário       usar scraping com cautela.  
* Web Scraping:  
  Para dados públicos visíveis na web, com atenção às políticas de uso das plataformas.  
* Ferramentas especializadas:  
  GNIP (para Twitter), CrowdTangle (para Facebook/Instagram).  
  ---

### **2\. Câmeras Públicas de Monitoramento** (CCTV Online)

**Descrição:**  
Algumas cidades oferecem acesso público a câmeras de monitoramento de tráfego e espaços públicos.  
**Tipo de dados:**  
Não estruturados: vídeo em tempo real ou imagens.  
**Métodos de acesso e coleta:**

* Streams públicos: Sites de prefeituras ou órgãos de trânsito que disponibilizam câmeras online.  
* Web scraping: Extração de imagens ou fluxos, com cuidado legal.  
* Integração direta: Via acordos com prefeituras ou órgãos de segurança que disponibilizem feeds abertos.

---

### **3\. Dados de Transporte Público** (GTFS e APIs de mobilidade)

**Descrição:**  
Informações sobre fluxo de transporte público (metrô, ônibus), úteis para entender concentração e deslocamento de pessoas.  
**Tipo de dados:**  
Estruturados: horários, rotas, número de passageiros.  
**Métodos de acesso e coleta:**

* GTFS (General Transit Feed Specification): Formato padrão usado mundialmente para disponibilização de dados de transporte.  
* APIs locais: exemplos: SPTrans (São Paulo), Moovit API, Google Transit API.  
* Scraping: Para casos em que os dados são publicados em sites sem API.

---

### **4\. Dados Meteorológicos** (INMET, NOAA, OpenWeather)

**Descrição:**  
Condições climáticas podem impactar a segurança em eventos (tempestades, calor extremo).  
**Tipo de dados:**  
Estruturados: temperatura, umidade, pressão, previsão do tempo, histórico.  
**Métodos de acesso e coleta:**

* APIs públicas:  
  OpenWeather API (grátis para consultas básicas).  
  NOAA (National Oceanic and Atmospheric Administration) — dados climáticos históricos e em tempo real.  
  INMET (Instituto Nacional de Meteorologia — Brasil) — dados meteorológicos públicos

---

### **5\. Dados Históricos de Crimes e Ocorrências Policiais**

**Descrição:**  
Bases de dados públicas sobre crimes, incidentes e ocorrências relacionadas a eventos anteriores.  
**Tipo de dados:**  
Estruturados: tabelas com localização, tipo de ocorrência, data e hora.  
**Métodos de acesso e coleta:**

* Portais de dados abertos: ex.: SSP-SP (Secretaria de Segurança Pública de São Paulo), FBI Crime Data Explorer (EUA).  
* Downloads diretos: CSV, Excel ou JSON.

---

### **6\. Sensores Urbanos e Dados de Ruído** (Plataformas Open Data)

## **Descrição:** Sensores instalados em cidades inteligentes coletam dados sobre níveis de ruído, poluição e densidade de pessoas. **Tipo de dados:** Estruturados: níveis de decibéis, fluxo de pessoas. **Métodos de acesso e coleta:**

* ## Plataformas Open Data: exemplos: NYC Open Data, Dados Abertos SP.

* ## APIs de sensores urbanos: Smart Cities com sistemas de dados abertos podem oferecer esse recurso.

---

## **Fontes secundárias (não prioritárias, mas complementares):** 

**Dados de localização e mapas (OpenStreetMap):** importantes para a visualização geoespacial e roteamento, mas não essenciais para a detecção direta de tumultos.

# Os dados foram criados com ferramentas e bibliotecas generativas. 

## Justificativa do uso de dados sintéticos:

Devido à natureza sensível dos dados envolvidos neste tipo de análise — incluindo informações pessoais, geolocalização e conteúdos potencialmente identificáveis de redes sociais —, este projeto opta pela utilização de **dados sintéticos**.

Os dados sintéticos são informações geradas artificialmente que imitam características estatísticas e padrões encontrados em dados reais, mas sem representar indivíduos ou eventos reais. Esta abordagem oferece diversas vantagens:

1. Evita riscos legais e éticos, respeitando legislações como a LGPD (Lei Geral de Proteção de Dados).

2. Permite o desenvolvimento e validação de modelos analíticos em um ambiente seguro e controlado.

3. Favorece a transparência e a replicabilidade, uma vez que os dados podem ser compartilhados livremente para fins educacionais ou de pesquisa.

Assim, o uso de dados sintéticos neste projeto não compromete a validade da proposta, pois o foco está na demonstração da metodologia e no potencial da análise de dados como ferramenta para prevenção de crises em eventos de grande porte.

</details>

<details>
<summary><strong>📓 Acesso aos notebooks</strong></summary>



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
