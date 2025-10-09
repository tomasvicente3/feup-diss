# Research notes regarding read papers
## NAMP
### 3.1 "Only for FC layers"
Could we mock a FC layer from Non-FC layers, adding a connection with weigth 0?

### Backtracking algorithm - Listing 3
What are the variables in it???

### Results - 15 devices
"120 neurons is not equally divisible by 7" (possibility of asymmetric assigning or greedy heuristics?)

### Future Work
- LwM2M (Lightweight Machine-to-Machine)
- MQTT (Message Queuing Telemetry Transport)


## TinyMLaaS
### Review limitations
- Lack of standardized protocol


## TinyML-Enabled...
### advantages of TinyML
- Ver sec II

### Frameworks e modalidades
- Ver sec III


## TensorFlow Lite Micro...
### Use Cases of TinyML
- Wake word detection
- Sound anomaly detection
- Ver sec 1 (introduction)

### Dificuldades nas Frameworks TinyML, pré TFLM
- ver sec 1 (pag 2, col esq)

### Vantages do TFLM
- ver sec 1 (pag 2, col esq, 2ª enum)


## Distributed Deep Neural Networks Over...
### Decomposição da Computação
Cloud - Edge - End device


## TDMiL (2024)
### Problemas
- Sem frameworks gerais
- Limitações dos MCU e memória

### Contexto
- De Microprocessadores (RasberryPi) (potencia em W) a Microcontroladores (pot em mW)

### Feramentas
- MCUNet
- Ver outras refs, no geral

#### Web Transfer
```
Work such as [42] suggests that in scenarios with highly dynamic clients, especially
during asynchronous events, the recommendation is to utilize CoAP Pub/Sub rather than Message Queuing
Telemetry Transport-Sensor Networks (MQTT-SN), for applications handling large payloads in environments
prone to high packet loss, which matches our scenario.
```

#### Management
- LwM2M (using CoAP) > gRPC

#### Data Represantation
Concise Binary Object Representation (CBOR) >> XML/JSON