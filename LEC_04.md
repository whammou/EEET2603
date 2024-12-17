# Lecture 4 - DC Circuit Analysis Methods


- **Reference:** Chapter 7,8 of the book [Introductory Circuit Analysis](/server/archive/circuits/introductory.epub)


## 0. Resistive Circuit


A circuit that contains only a pure resistance (ohms) in an AC circuit is called a Purely Resistive AC Circuit. From a technical standpoint, this circuit does not contain capacitance or inductance


## 1. Circuit Simplification for Resistive Network


- This method is normally applied for the [resistive circuit](#0-resistive-circuit) with only one electrical source
- The *series* or *parallel* network between two nodes can be represented by one equivalent resistance
- Applying [Ohm's Law](./LEC_02.md#3-ohms-law) to find the current of the series network or the voltage of parallel network


<details>
  <summary><b>Example</b></summary>
    <p align="center">
      <IMG src="./assets/LEC_04/LEC_1_1.svg" alt="cicuit simplification" width=80%/>
    </p>
</details>


## 2. Voltage Divider Rule


For the **series network** between two `nodes`, voltage of every resistor is calculated:

[^1] *Voltage Divider*
[^1]:Voltage Divider

$$V_{Ri} = V_s \times \left ( \frac{R_i}{R_T} \right )k$$

  - $V_S$ is the voltage between two nodes
  - $R_i$ is the resistance of resistor $i$
  - $R_T$ is the total resistance of the series network


> [!NOTE]
> Polarity of $V_{Ri}$ and $V_S$ are the same





# Footnote

