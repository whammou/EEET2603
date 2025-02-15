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


For the **series network** between two `nodes`, `voltage` of every `resistor` is calculated:

[^1] *Voltage Divider Rule*
[^1]:Voltage Divider Rule

$$V_{Ri} = V_s \times \left ( \frac{R_i}{R_T} \right )$$

  - $V_S$ is the `voltage` between two `nodes`
  - $R_i$ is the **resistance** of `resistor` $i$
  - $R_T$ is the total **resistance** of the *series network*


> [!NOTE]
> Polarity of $V_{Ri}$ and $V_S$ are the same


<details>
  <summary><b>Example</b></summary>
  <IMG src="./assets/LEC_04/LEC_2_1.svg" alt="voltage divider" width=80%/>
</details>


## 3. Current Divider Rule


For the **parallel network** between two `nodes`, `current` of every `resistor` is calculated as:

[^2] *Current Divider Rule*
[^2]:Current Divider Rule

$$I_{Ri} = I_S \times \left(\frac{R_T}{R_i} \right) = \left(\frac{R_i}{R_T} \right)^{-1}$$

  - $I_S$ is the total `current` going to the *parallel network*
  - $R_i$ is the **resistance** of `resistor` **i**
  - $R_T$ is the total **resistance** of the *parallel network*


  > [!NOTE]
  > Direction of $I_{Ri}$ and $_S$ are the same


<details>
  <summary><b>Example</b></summary>
  <IMG src="./assets/LEC_04/LEC_3_1.svg" alt="current divider" width=80%/>
</details>


## 4. Voltage and Current Sources


The ideal source behaviours:
- It will always produce the same current/voltage regardless of its load
- This expectation is not realistic


### 4.1 Ideal DC Voltage Source


An **ideal DC voltage source** is powerful enough to maintain constant `voltage` at its output regardless of the `current` flowing through the `source`


> [!IMPORTANT] 
> Two voltage sources of different voltage rating cannot be placed in parallel (violation of [KVL](./LEC_03.md#21-krichhoffs-voltage-law-kvl)


<p align="center">
  <IMG src="./assets/LEC_04/SCR_41_1.png" alt="ideal voltage source" width=80%/>
</p>


### 4.2 Practical DC Voltage Source


A **practical voltage source** consists of an [ideal source](#41-ideal-dc-voltage-sources) *in series with* the source `resistance` $R_S$


<p align="center">
  <IMG src="./assets/LEC_04/SCR_42_1.png" alt="practical voltage source" width=80%/>
</p>


> [!NOTE]
> For an **ideal voltage source** the value of $R_S = 0 \Omega$ 


### 4.3 Ideal DC Current Sources


An **ideal Current Source** is powerful enough to maintain constant `current` through it regardless of the `voltage` across the `source`


> [!IMPORTANT]
> Two current sources of different current rating cannot be placed in series (violation of [KCL](./LEC_03.md#22-kirchhoffs-current-law-kcl))


<p align="center">
  <IMG src="./assets/LEC_04/SCR_43_1.png" alt="ideal current source" width=80%/>
</p>

### 4.4 Practical DC Current Sources


A **practical current source** consists of an [ideal source](#43-ideal-dc-current-sources) in *parallel* with a source `resistance` $R_S$


<p align="center">
  <IMG src="./assets/LEC_04/SCR_44_1.png" alt="pratical current source" width=80%/>
</p>


> [!NOTE]
> For **ideal current source** the value of `resistance` $R_S = \infty \Omega$


## 5. Source Conversion


- Any `voltage source` $V_S$ in **series** with a `resistor` $R_S$ can be converted to an equivalent `current source` $I_S$ in **parallel** to the `resistor` $R_S$
- `Resistor` is the **same** in both cases
- $V_S$ and $I_S$ relationship: 

[^3] *Source Conversion*
[^3]:Source Conversion

$${V_S = R_{S} I_S}$$


> [!NOTE]
> **Direction** of the `current source` us from **low** potential `(-)` terminal to **high** potential `(+)` terminal of the `voltage source`


<p align="center">
  <IMG src="./assets/LEC_04/SCR_5_1.png" alt="source conversion" width=80%/>
</p>


# Footnote

