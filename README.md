# Sensor-de-enchentes
`Linguagem: C++` - `Problemas: Não identificados` - `Colaboradores: 3` - `Status: Concluído`

![Imagem do WhatsApp de 2025-06-06 à(s) 09 24 05_1152bc0e](https://github.com/user-attachments/assets/2be228fa-7faa-4c79-9771-92175b6f4f97)

> Projeto de Edge Computing & Iot : sistema físico de monitoramento


### Contextualização
➡️ Nas últimas décadas, o Brasil tem enfrentado enchentes recorrentes, principalmente em áreas urbanas com infraestrutura precária e planejamento inadequado. Cerca de um terço dos municípios apresenta um alto risco de desastres por inundações, os quais são agravados pela ocupação irregular e por eventos climáticos extremos. Além de danos materiais e econômicos, o fenômeno impacta no bem-estar populacional, com doenças transmitidas por água contaminada, proliferação de vetores e colapso de serviços essenciais, afetando sobretudo populações vulneráveis. A falta de políticas eficientes de prevenção agrava a situação, exigindo ações urgentes e integradas entre setores público e privado.

## Introdução
➡️  Diante desse cenário, soluções tecnológicas acessíveis e eficientes são essenciais para mitigar os riscos e alertar a população sobre situações críticas. Este projeto propõe um sistema de monitoramento e alerta de enchentes baseado em um sensor ultrassônico, capaz de medir o nível da água em bueiros e vias urbanas.  

## 📃Descrição
➡️ Ao detectar uma elevação perigosa no nível da água, o dispositivo aciona indicadores visuais (LEDs) e sonoros (buzzer), garantindo que tanto pessoas com deficiência visual quanto auditiva sejam devidamente alertadas. Os dados são exibidos em um display LCD e transmitidos via comunicação serial, permitindo acompanhamento em tempo real. Dessa forma, o sistema visa prevenir acidentes, reduzir os danos causados por inundações e contribuir para a segurança da população, especialmente em regiões com infraestrutura precária e maior vulnerabilidade a desastres.  

## ⚙️Componentes utilizados 
Para realizar a montagem do equipamento, foram necessários:

- [x] Sensor de distância ultrassônico HC-SR04
- [x] Buzzer piezoelétrico
- [x] LDC com 2 linhas, 16 caracteres por linha
- [x] Protoboard
- [x] Led's (vermelho, amarelo e verde)
- [x] 3 Resistores (220 Ohms)

## 🛠️Principais funcionalidade
- Medição em tempo real do nível da pagua utilizando sensor HC-SR04
- Sistemas de Alerta visual utilizando led's verde, amarelo e vermelho, os quais indicam diferentes níveis de risco (inclusão de indivíduos com deficiência auditiva)
- Alerta sonoro com buzzer (inclusão de indivíduos com deficiência visual)
- Exibição de dados em um display LDC e no Serial Monitor

>❗Níveis de Risco:
  Led verde: distância segura (>66% da distância máxima) -
  Led amarelo: nível intermediário (entre 33% e 66% da distância máxima) -
  Led vermelho (+buzzer): Nível crítico (<33% da distância máxima).

```
Trata-se de um prjeto acessível e de baixo custo, utilizando componentes eletrônicos simples
```


## 💻Simulação
```
Simulação realizada através do Wokwi.
```
![image](https://github.com/user-attachments/assets/63f0530b-4139-45ff-bbfd-d386ef8c4a00)
>Alternativa de simulação: Tinkercad

## Guia de Simulação
1. Acesse o Wokwi (https://wokwi.com), ou Tinkercad (https://tinkercad.com),  e crie um novo projeto.
2. Adicione os componetes (aqueles identificados na sessão "⚙️Componetes utilizados").
3. Conecte os componentes conforme o esquema:
- HC-SR04 (sensor de distância:
   - ```Trig```: Pino 13
   - ```Echo```: Pino 12
- Buzzer: Pino 10
- Led's:
   - Verde: Pino 10
   - Amarelo: Pino 9
   - Vermelho: Pino 8
- LDC I2C: Conecte via barramento I2C (SDA: A$ - SCL: A5)
4. Copie e cole o código fornecido neste repositório.
5. Execute a simulação e observe:
   - O LDC exibindo a distância em cm.
   - Os led's acendendo condorme o nível da água (é possível alterar a sitância do sensor dentro do simulador)
   - O buzzer tocando quando o led vermelho é ativado.
   - 
> Link direto para o projeto no Wokwi: [https://wokwi.com/projects/432199183495312385](https://wokwi.com/projects/433021166159651841)

> Link do vídeo de simulação do projeto montado com os materiais: https://youtube.com/shorts/aaJSPbpZQcY?si=xv7V4EAsl86TR_oH



### 🤝Colaboradores
Os contribuidores para este projeto foram:
`Laura Dantas`
`Felipe Catto`
`Raphael Aaron`
