# Interactive Fourier Series Explorer

An intuitive, web-based tool for exploring the fascinating world of Fourier Series. This application allows users to visualize how complex periodic waveforms can be decomposed into a sum of simple sine and cosine waves. It's built with vanilla JavaScript, HTML, and CSS, and runs entirely in a single, self-contained file.

### [➡️ Try the Live Demo!](https://inverter3p.github.io/fourier/)


![fourier](https://github.com/user-attachments/assets/9d6355f0-de9d-42df-8db0-c0ff2ca6110c)

---

## Features

*   ✍️ **Draw Your Own Waveforms:** Use your mouse to draw any periodic function directly on the canvas.
*   🔢 **Plot from Data:** Manually enter or paste `x,y` coordinates to plot precise functions. The axes automatically scale to fit your data.
*   🚀 **Classic Presets:** Instantly generate Square, Triangle, and Sawtooth waves to see their famous Fourier series in action.
*   🎚️ **Real-time Harmonic Control:** Adjust the number of harmonics with a slider and see the reconstructed wave and frequency spectrum update instantly.
*   📊 **Frequency Spectrum Visualization:** View the magnitude of the Fourier coefficients for your signal, clearly distinguishing the DC component and the harmonic amplitudes.
*   🔍 **Unclipped Auto-Scaling:** When Gibbs phenomenon causes clipping, a dedicated modal window opens to show the waveform in its full, unclipped range.
*   ⚙️ **Interactive Modal:** The auto-scale window has its own synchronized harmonics slider, allowing for detailed analysis of ringing and convergence.

---

## How to Use

### As a User
There are two easy ways to run the explorer:
1.  **Click the [Live Demo link]([https://your-github-username.github.io/your-repo-name/](https://inverter3p.github.io/fourier/) above.**
2.  Alternatively, download the `index.html` file from this repository and open it in your favorite web browser (like Chrome, Firefox, or Edge).

### As a Developer
The project is intentionally simple to modify:
1.  Clone the repository:
    ```bash
    git clone https://github.com/your-github-username/your-repo-name.git
    ```
2.  Open the `index.html` file in a code editor.
3.  All the HTML, CSS, and JavaScript are in that single file. Make your changes, save, and refresh your browser to see them.

---

## Technical Details

*   **Frontend:** Vanilla JavaScript, HTML5, and CSS. No frameworks or libraries are used, making the code easy to read and understand.
*   **Fourier Analysis:** The application performs a Discrete Fourier Transform (DFT) to calculate the `a_n` and `b_n` coefficients of the series.
*   **Point Extraction:** The "drawing-to-text" feature uses the **Ramer-Douglas-Peucker algorithm** to simplify the drawn path into a concise set of key points, making the data more manageable.

---



---

## License

Distributed under the MIT License. See `LICENSE` for more information.
