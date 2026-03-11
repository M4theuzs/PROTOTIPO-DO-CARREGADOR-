# PROTOTIPO-DO-CARREGADOR-

# ⚡ Protótipo de Fonte Regulada 12V (Carregador)

## 📝 Descrição
Este projeto apresenta o desenvolvimento de um protótipo de fonte de alimentação utilizando uma ponte retificadora e o regulador de tensão **7812**. O circuito converte tensão alternada (AC) para corrente contínua (DC) regulada em **12V**.

---

## 📐 Documentação Visual

### Esquemático do Circuito
O design foca na estabilidade da tensão e filtragem de ruídos.
![Esquemático](PROJETO%20SIMPLES.jfif)

### Layout da PCB (Trilhas)
Design otimizado para placa de face simples (80mm x 40mm).
![Layout PCB](PROJETO%20FUNDO%20PRETO.jfif)

### Visualização 3D do Projeto
Representação final dos componentes montados na placa.
![Projeto 3D](PROJETO%203D.jfif)

---

## 📦 Lista de Componentes Utilizados
Conforme detalhado na lista de dispositivos do projeto:

![Lista de Dispositivos](IMAGEM%20DO%20QUE%20TENHO.jfif)

| Referência | Componente | Função |
| :--- | :--- | :--- |
| **J1** | Conector SIL-2 | Entrada AC (Transformador) |
| **BR1** | Ponte Retificadora | Retificação de onda completa |
| **C1** | Capacitor 1000uF | Filtragem de Ripple (Eletrolítico) |
| **C2 / C3** | Capacitores 100nF | Estabilização e Desacoplamento |
| **U1** | Regulador 7812 | Saída estável de 12V DC |
| **R1** | Resistor 100R | Limitador de corrente do LED |
| **D1** | LED | Indicador visual de Power ON |
| **J2** | Conector SIL-2 | Saída final da fonte |

---

## 👨‍💻 Autor
Projeto desenvolvido por **Matheus Henrique Albert**.
