**Analog to Digital Quantization in Python**

An algorithm to compute a quantized value of a given analog voltage input, built in Python. The project optionally includes a GUI interface to visualize the input and output in real-time.

_**Features**_

🧮 Converts analog voltage values to quantized digital outputs

⚙️ Configurable parameters (reference voltage, resolution, etc.)

🖥️ Optional graphical user interface (GUI) for visualization

💡 Clean, modular, and easy-to-understand Python code


_**How It Works**_

The algorithm simulates an Analog-to-Digital Converter (ADC):

1. Input: Analog voltage (floating-point value)

2. Process:

* Set resolution (e.g., 8-bit, 10-bit)

* Define reference voltage (e.g., 5V)

* Compute digital equivalent using:

Quantized Value=⌊Vref​Analog Voltage​×(2n−1)⌋

3. Output: Integer value between 0 and 2^(n) - 1, where = 𝑛 is the resolution


**GUI Preview**

If using the GUI version (Tkinter or PyQt based), you’ll see:

Input field for analog voltage

Dropdown for resolution

Real-time quantized result display

**Installation**
_git clone https://github.com/yourusername/analog-quantizer.git
cd analog-quantizer
pip install -r requirements.txt_

**Usage**

**_CLI Version:___**

_python quantizer.py --voltage 2.5 --resolution 10 --vref 5.0_

_**GUI Version:**___

_python gui_quantizer.py_


**Contributing**

Pull requests are welcome! Please open an issue first to discuss your ideas.
