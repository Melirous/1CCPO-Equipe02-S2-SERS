# GreenVolt – Sistema Inteligente de Gerenciamento Energético para Eletropostos Sustentáveis

## Integrantes

* João Victor Canello Ferian – RM573295
* Gustavo Melo dos Santos – RM573562
* João Pedro Costenari Silva – RM572260

---

# Introdução

O crescimento da mobilidade elétrica tem aumentado significativamente a demanda por infraestrutura de recarga eficiente e sustentável. Nesse contexto, os eletropostos precisam gerenciar de forma inteligente os recursos energéticos disponíveis, reduzindo desperdícios e minimizando impactos ambientais.

O projeto **GreenVolt** propõe uma solução inteligente para gerenciamento energético de eletropostos, priorizando o uso de energia solar e aplicando conceitos de eficiência computacional por meio de sistemas embarcados e arquitetura RISC-V.

---

# Problema

Os eletropostos atuais enfrentam diversos desafios relacionados ao consumo e gerenciamento de energia:

* Alto consumo energético;
* Desperdício de energia durante períodos de baixa demanda;
* Sobrecarga da rede elétrica;
* Baixa integração com fontes renováveis;
* Sistemas computacionais pouco eficientes.

Esses fatores aumentam os custos operacionais e reduzem a sustentabilidade da infraestrutura de recarga.

---

# Objetivos

## Objetivo Geral

Desenvolver um sistema inteligente capaz de gerenciar o fornecimento de energia para eletropostos sustentáveis, priorizando o uso de energia renovável e otimizando o processamento computacional.

## Objetivos Específicos

* Monitorar a geração de energia solar em tempo real;
* Controlar o processo de carregamento dos veículos elétricos;
* Priorizar o uso de energia solar;
* Reduzir desperdícios energéticos;
* Simular decisões inteligentes de gerenciamento energético;
* Demonstrar a viabilidade técnica da solução através de uma prova de conceito funcional.

---

# Arquitetura da Solução

## Visão Geral

O sistema é composto por sensores responsáveis por monitorar a geração de energia solar e a demanda de carregamento dos veículos.

As informações coletadas são processadas por um controlador baseado em arquitetura RISC-V, responsável por decidir qual fonte energética será utilizada.

### Fluxo do Sistema

Painéis Solares
↓
Sensores IoT
↓
Controlador RISC-V
↓
Sistema de Decisão
↓
Carregadores de Veículos

Caso a energia solar seja insuficiente, o sistema utiliza a rede elétrica como fonte complementar.

---

# Tecnologias Utilizadas

## Hardware

* Painéis solares fotovoltaicos;
* Sensores IoT;
* Sistemas embarcados;
* Controladores baseados em arquitetura RISC-V;
* Inversores híbridos GoodWe.

## Software

* Linguagem Python (protótipo funcional);
* Programação Assembly (conceito de otimização embarcada);
* Sistemas de monitoramento energético;
* Algoritmos de tomada de decisão.

---

# Protótipo Funcional

A prova de conceito foi implementada por meio de uma simulação computacional.

O sistema recebe informações sobre:

* Energia solar disponível;
* Demanda de carregamento;
* Disponibilidade da rede elétrica.

Com base nesses dados, o algoritmo decide automaticamente a melhor forma de alimentar o eletroposto.

### Regras de Funcionamento

1. Utilizar energia solar sempre que possível.
2. Complementar com energia da rede quando necessário.
3. Evitar sobrecargas através de controle inteligente de potência.
4. Gerar relatórios operacionais.

---

# Código de Demonstração

```python
energia_solar = 35
demanda_carregamento = 25
rede_disponivel = True

print("=== SISTEMA GREENVOLT ===")

if energia_solar >= demanda_carregamento:
    print("Carregamento utilizando apenas energia solar.")
else:
    print("Energia solar insuficiente.")

    if rede_disponivel:
        complemento = demanda_carregamento - energia_solar
        print(f"Complemento da rede: {complemento} kWh")
    else:
        print("Rede indisponível.")

if demanda_carregamento > 40:
    print("Modo economia ativado.")
else:
    print("Potência normal.")
```

---

# Dados Simulados

| Horário | Energia Solar (kWh) | Demanda (kWh) |
| ------- | ------------------- | ------------- |
| 08h     | 15                  | 10            |
| 10h     | 30                  | 20            |
| 12h     | 50                  | 35            |
| 14h     | 45                  | 40            |
| 18h     | 10                  | 30            |

---

# Resultados Obtidos

A simulação demonstrou que:

* O sistema prioriza corretamente o uso de energia solar;
* Há redução da dependência da rede elétrica durante períodos de alta geração fotovoltaica;
* O gerenciamento inteligente reduz desperdícios energéticos;
* O controle de potência contribui para evitar sobrecargas.

---

# Sustentabilidade e Energias Renováveis

O GreenVolt foi desenvolvido com foco nos princípios de sustentabilidade estudados durante o semestre.

A utilização de energia solar proporciona:

* Redução da emissão de gases de efeito estufa;
* Menor dependência de fontes não renováveis;
* Redução dos custos energéticos;
* Maior eficiência operacional.

Além disso, o uso de arquitetura RISC-V e conceitos de programação Assembly contribui para:

* Menor consumo computacional;
* Maior eficiência energética dos sistemas embarcados;
* Melhor aproveitamento dos recursos de hardware.

---

# Impactos Esperados

## Impactos Ambientais

* Redução da emissão de CO₂;
* Incentivo ao uso de energia renovável;
* Menor desperdício energético.

## Impactos Tecnológicos

* Otimização computacional;
* Processamento mais eficiente;
* Melhor gerenciamento energético.

## Impactos Sociais

* Incentivo à mobilidade sustentável;
* Apoio à transição energética;
* Desenvolvimento de tecnologias sustentáveis.

# Conclusão

O GreenVolt demonstrou a viabilidade técnica de um sistema inteligente de gerenciamento energético para eletropostos sustentáveis.

A solução integra energias renováveis, sistemas embarcados e eficiência computacional para promover uma infraestrutura de recarga mais sustentável, eficiente e alinhada às necessidades da mobilidade elétrica moderna.
