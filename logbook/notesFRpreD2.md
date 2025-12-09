# Notes

DICA
- O SOTA é muito importante para não só estares mais dentro do teu tópico como também para perceber o que existe e se podemos utilizar alguma coisa que alguém já fez no nosso contexto. Apesar disso, é muito fácil perder demasiado tempo no SOTA e a ler coisas novas e interessantes mas, quando tiveres o problema em específico que vais atacar e a solução definida/pensada, vais precisar de tempo para implementar as coisas :D
  - Tenta controlar o tempo que dispendes e focar no problema :) 


## Research Questions

### RQ1: Is it feasible to integrate edge devices into far-edge devices’ inference networks without compromising performance?

- Integrar edge no far-edge pode não ser verdade, existe algumas pessoas que definem o far-edge como um subset da edge. O que nós queremos é mais algo como: 'Is it feasible to have collaborative ML inferences using edge and far-edge devices without compromising performance?'

### RQ2: What is the most efficient method to enable reliable communication between edge and far-edge devices partaking in an inference network?

- O que é que estavas a pensar com "reliable communication"?
- Eu diria que o principal nisto será a otimização na comunicação entre os dispositivos na quantidade de dados que são transmitidos durante as inferências. Esta otimização faz-se quando orquestramos e distribuimos as partes do modelo.

### RQ3: How efficiently can the resources of edge and far-edge devices be utilized towards collaborative inference tasks?

- Acho que a resposta a esta pergunta é o grande foco da tua tese
- Perceber como é que podemos usar os vários tipos de dispositivos tendo em conta as suas peculiaridades e os requisitos da aplicação (neste caso um modelo AI)

### RQ4: Is there a feasible method to fragment more complex DNN models (e.g., Recurrent Neural Networks (RNNs)) in the context of edge and far-edge computing?

- Pode ser giro ver o que existe no State of the Art mas diria que a implementação de algoritmos de partição não será o foco

## Queries

### 2b - Model Partitioning & Split Inference

( "split inference" OR "distributed inference" OR "split computing" OR "collaborative inference" OR "layer partitioning" OR "DNN partitioning" ) AND ( "Edge" OR "Far-Edge" OR "TinyML" OR "microcontroller" OR "resource-constrained" )	

- OK!
- Dado que este tópico será perceber o que existe no SOTA e não de implementação, aconselhava a não perderes muito tempo nestes artigos, só se vires que realmente vale a pena.

### 3b - ML Workload Orchestration / Scheduling

( ("resource-aware" OR "network-aware" OR "adaptive" OR "heterogeneous") NEAR/5 ("schedul*" OR "orchestrat*" OR "placement" OR "allocation") ) AND ( "inference" OR "ML model*" OR "DNN" ) AND ( "Edge" OR "Fog" OR "IoT" OR "Far-Edge" )

- OK! Alterava ML model para só ML
- Provavelmente vais perder mais tempo nos resultados desta query que deve haver cenas engraçadas

### 4c - Computation Offloading

( "inference" NEAR/3 ("offload*" OR "decision*") OR "inference offloading" ) AND ( "resource-aware" OR "latency-aware" OR "energy-aware" OR "adaptive" OR "resource-constrained" OR "decision model" ) AND ( "Edge" OR "Far-Edge" OR "IoT" OR "TinyML" OR "MCU" )	

- OK!
- Aqui podem aparecer coisas fixes mas imagino que vás apanhar muitos artigos muito low level, e.g., soluções ao nível do HW e coisas assim. Tens que filtrar bem os resultados quando fores ler o abstract para ver se encontramos alguma coisa a nível de distribuição de modelos na rede/clusters de dispositivos

### 5c - Heterogeneous Resource Management 

("device heterogeneity" OR "hardware heterogeneity" OR "heterogeneous computing" OR "heterogeneous resources" OR "heterogeneous cluster") AND ("schedul*" OR "orchestrat*" OR "allocation") AND ("inference" OR "DNN" OR "ML workload*") AND ("Edge" OR "IoT" OR "Far-Edge")	

- Acaba por ser bastante parecida à 3b. O que achas de tentar dar merge?
- E claramente tens resultados suficientes para ler com as outras :P
