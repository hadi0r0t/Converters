## Converters
# DC-DC Power Converter Simulations

A collection of MATLAB/Simulink models for simulating various DC-DC power converter circuits.

## 📁 Converters Available

| Converter | Description | Model File |
| :--- | :--- | :--- |
| **Buck** | Step-down converter. | `buck_converter.slx` |
| **Boost** | Step-up converter. | `boost_converter.slx` |
| **Buck-Boost** | Inverting converter that can step-up or step-down voltage. | `buckboostconverter.slx` |

## 🚀 How to Run

1.  Clone this repository.
    ```bash
    git clone https://github.com/your-username/your-repo-name.git
    ```
2.  Open MATLAB and navigate to the project folder.
3.  Open the desired model file (e.g., `buck_boost_model.slx`).
4.  Click the **"Run"** button in Simulink.
5.  Double-click on the **Scope** blocks to view the results.

## ⚙️ Buck Model Details

**Parameters:**
- **Input Voltage:** 24 V
- **Output Voltage:** 12 V
- **Switching Frequency:** 50 kHz
- **Duty Cycle:** 50%
- **Inductor:** 180 µH
- **Capacitor:** 22 µF
- **Load:** 5 Ω

**Expected Results:**
- A regulated **12 V** output with small ripple.
- Inductor current is a triangular wave with an avg. of **~1.2 A**.
- Output current is a DC value of **1.2 A**.

## ⚙️ Boost Model Details

**Parameters:**
- **Input Voltage:** 12 V
- **Output Voltage:** 24 V
- **Switching Frequency:** 50 kHz
- **Duty Cycle:** 50%
- **Inductor:** 180 µH
- **Capacitor:** 47 µF
- **Load:** 20 Ω

**Expected Results:**
- A regulated **24 V** output with small ripple.
- Inductor current is a triangular wave with an avg. of **~2.4 A**.
- Output current is a DC value of **1.2 A**.

## ⚙️ Buck-Boost Model Details

**Parameters:**
- **Input Voltage:** 12 V
- **Output Voltage:** -12 V
- **Switching Frequency:** 50 kHz
- **Duty Cycle:** 50%
- **Inductor:** 180 µH
- **Capacitor:** 100 µF
- **Load:** 10 Ω

**Expected Results:**
- A regulated **-12 V** output with small ripple.
- Inductor current is a triangular wave with an avg. of **~2.4 A**.
- Output current is a DC value of **-1.2 A**.

## 🔧 Solver Settings

For best results, models use variable-step solver `ode15s` with a max step size of `400e-9 s`.

## 👨‍💻 Author
**Hadi Rafat Talab**  
*GitHub:* [@hadi0r0t](https://github.com/hadi0r0t)  
*Email:* hadi0r0t@gmail.com

## 📝 License

This project is licensed under the MIT License. See the `LICENSE` file for details.
All DC-DC convrtors simulations in Matlab 
