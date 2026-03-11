# PROTOTIPO-DO-CARREGADOR-

#  Protótipo de Fonte de Alimentação Linear Regulada (12V)

##  Apresentação do Projeto
Este projeto consiste no desenvolvimento completo de uma **Fonte de Alimentação Linear de 12VDC**. O objetivo principal é converter a tensão alternada (AC) proveniente de um transformador em uma tensão contínua (DC) estável e livre de ruídos, capaz de alimentar circuitos eletrônicos sensíveis, como microcontroladores e sistemas embarcados.

O projeto abrange desde o diagrama esquemático até o design da placa de circuito impresso (PCB) e a visualização tridimensional.

---

## Descrição Técnica do Circuito

O circuito é dividido em quatro estágios fundamentais:

1. **Estágio de Retificação (BR1):** Utiliza uma ponte de diodos (Full Wave Bridge Rectifier) para converter a senóide de entrada AC em uma forma de onda DC pulsante, aproveitando ambos os semiciclos da rede.
2. **Estágio de Filtragem (C1):** O capacitor eletrolítico de **1000µF** atua como filtro capacitivo. Ele armazena carga durante os picos de tensão e a libera nos vales, reduzindo o *ripple* (ondulação) e entregando uma tensão mais linear ao regulador.
3. **Estágio de Regulação (U1 - LM7812):** O circuito integrado 7812 recebe a tensão filtrada e a mantém fixada em **12V**, independente de variações na carga ou na entrada (desde que respeitado o dropout voltage de aproximadamente 2V).
4. **Estágio de Estabilização e Proteção (C2, C3, D1):** - Os capacitores cerâmicos de **100nF** filtram ruídos de alta frequência.
   - O LED **D1** associado ao resistor **R1 (100Ω)** fornece um feedback visual imediato de que a saída está energizada.

---

##  Documentação Visual e Design

### Diagrama Esquemático
O esquemático foi projetado para garantir clareza na análise do fluxo de corrente, com conexões otimizadas entre os estágios de potência e sinal.
![Esquemático](PROJETO%20SIMPLES.jfif)

###  Layout da PCB e Roteamento
A placa foi desenvolvida em **Face Simples (Bottom Layer)** com dimensões de **80mm x 40mm**. 
- **Largura das Trilhas:** Dimensionadas para suportar a corrente nominal do regulador sem aquecimento excessivo.
- **Isolamento:** Espaçamento adequado entre trilhas para evitar arcos elétricos e interferências.
![Layout PCB](PROJETO%20FUNDO%20PRETO.jfif)

###  Modelagem 3D
A visualização 3D permite validar o posicionamento físico dos componentes, garantindo que não haja interferências mecânicas e que o regulador **7812** tenha espaço para dissipação térmica.
![Projeto 3D](PROJETO%203D.jfif)

---

##  Lista de Dispositivos 
A seleção dos componentes foi feita com base na disponibilidade comercial e eficiência técnica:

![Lista de Componentes](IMAGEM%20DO%20QUE%20TENHO.jfif)

| Ref. | Componente | Especificação | Função Técnica |
| :--- | :--- | :--- | :--- |
| **J1** | Bloco Terminal | SIL-100-02 | Entrada de tensão AC (Secundário do Trafo) |
| **BR1** | Ponte Retificadora | BRIDGE | Retificação em onda completa |
| **C1** | Cap. Eletrolítico | 1000µF / 25V+ | Filtragem de ripple (baixa frequência) |
| **C2** | Cap. Cerâmico | 100nF | Desacoplamento de entrada do regulador |
| **U1** | Regulador Linear | LM7812 (TO-220) | Regulação ativa de tensão para 12V |
| **C3** | Cap. Cerâmico | 100nF | Estabilização de saída e transientes |
| **R1** | Resistor | 100Ω (1/4W) | Limitador de corrente para o LED indicador |
| **D1** | LED | 5mm (Blue) | Sinalização de funcionamento |
| **J2** | Bloco Terminal | SIL-100-02 | Saída de tensão regulada 12VDC |


##  Autor
**Matheus Henrique Albert** *Estudante de Eletrônica / Desenvolvedor de Hardware*
