## Projeto Milk Temperature

### Problem:
Milk Temperature on the Farm: Ensuring Quality and Safety
The temperature of milk on the farm is a crucial factor in ensuring the quality, safety and shelf life of the product. From milking to storage, temperature control is essential to prevent the proliferation of bacteria and maintain the nutritional properties of milk.

Temperatura do Leite na Fazenda: Garantindo Qualidade e Segurança
A temperatura do leite na fazenda é um fator crucial para garantir a qualidade, segurança e vida útil do produto. Desde a ordenha até o armazenamento, o controle da temperatura é essencial para evitar a proliferação de bactérias e manter as propriedades nutricionais do leite.

### Motivation:
Proper Storage
Chilled milk must be stored in cooling tanks, keeping the temperature below 4°C. It is important to ensure that refrigeration equipment is working properly and that the temperature is monitored regularly.

Armazenamento Adequado
O leite resfriado deve ser armazenado em tanques de resfriamento, mantendo a temperatura abaixo de 4°C. É importante garantir que o equipamento de refrigeração esteja funcionando corretamente e que a temperatura seja monitorada regularmente.

### Solution:
By transferring the temperature data through the Milk_Diagnostic equipment (device for collecting and sending milk data on the farm via SMS), we will analyze this data and use deep reinforcement learning to predict the temperature of the milk in the next few minutes, being able to alert the collecting company about a possible increase and for the producer to take action before the event happens. This guarantees the quality of the milk.

Transferindo os dados de temperatura através do equipamento Milk_Diagnostic (aparelho de coleta e envio de dados do leite na fazenda via sms) vamos analisar esses dados e utilizar aprendizado profundo por reforço para predizer a temperatura do leite nos próximos minutos podendo alertar sobre um possível aumento da mesma para a empresa captadora e para o produtor tomar as providências antes que o evento aconteça. Garantindo assim a qualidade do leite.

### Objective:
- In this project we are going to the investigative phase of Milk_Diagnostic (a device for collecting and sending milk data on the farm via SMS), we are going to carry out a survey of the variation in milk temperature over a given period. Here we will make a prediction of these temperatures, using reinforcement learning for the next few minutes to alert both the producer and the collecting company about a possible spike in the temperature of the milk stored on the farm, before the event happens.

- Nesse projeto vamos para a fase investigatória do Milk_Diagnostic (aparelho de coleta e envio de dados do leite na fazenda via sms), vamos fazer um levantamento da variação da temperatura do leite em determinado período. Aqui vamos fazer uma predição dessas temperaturas, utilizando aprendizado por reforço para os próximos minutos para alertar tanto o produtor quanto a empresa captadora sobre um possível pico da temperatura do leite armazenado na fazenda, antes que o evento aconteça.

### Data Origin:
- Dataset: MILK_temperature.TXT

- Through the Milk_Diagnostic equipment (device for collecting and sending milk data on the farm via SMS) data on milk temperature, ambient temperature, date, time, humidity, geographic coordinates, are transferred daily from the farm's milk reservoir every 10 minutes (configurable), 24 hours a day, 7 days a week.

- Através do equipamento Milk_Diagnostic (aparelho de coleta e envio de dados do leite na fazenda via sms)os dados de temperatura do leite, temperatura ambiente, data, hora, umidade, coordenadas geográficas, são transferidos diariamente do reservatório de leite da fazenda a cada 10 minutos (configurável), 24 horas por dia durante os 7 dias da semana.

- Aqui está o que as colunas representam:

    local: identificador da fazendo origem do leite
    data: data da coleta da temperatura
    hora: hora, minutos e segundos da coleta da temperatura
    lat: latitude do local da fazenda
    long: longitude do local da fazenda
    umidade: umidade ambiente do local do tanque de leite
    t_ex: temperatura ambiente do local do tanque de leite
    t1, t2, t3, t4, t5, t6, t7, t8: 
        temperaturas coletadas dentro do intervalo configurado para envio (10 minutos para esse trabalho)
