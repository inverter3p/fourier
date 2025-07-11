# Interactive Fourier Series Explorer

An intuitive, web-based tool for exploring the fascinating world of Fourier Series. This application allows users to visualize how complex periodic waveforms can be decomposed into a sum of simple sine and cosine waves. It's built with vanilla JavaScript, HTML, and CSS, and runs entirely in a single, self-contained file.

### [➡️ Try the Live Demo!](https://inverter3p.github.io/fourier/)


![fourier](https://github.com/user-attachments/assets/9d6355f0-de9d-42df-8db0-c0ff2ca6110c)

---

## How to Use

This tool provides three primary ways to define a waveform. The core concept is that the **X-Max** value defines the fundamental period (T) of your signal.

### 1. Draw a Waveform with Your Mouse

This is the most intuitive way to get started.
-   Simply click and drag your mouse across the **"Your Waveform"** canvas on the left.
-   As you draw, the application instantly calculates the Fourier series and displays the reconstructed wave and its frequency spectrum.
-   Once you release the mouse, the coordinates of your drawing are automatically extracted into the text area below.

### 2. Plot Precise Points from the Text Area

For creating precise or complex waveforms, you can input `x,y` coordinates directly.
-   Enter coordinates in the text area, with each point on a new line (e.g., `0, 100` then `1, -50`).
-   When you click **"Plot from Points"**, the application reads your data and:
    -   **Automatically scales the axes:** If your points go beyond the current `X-Max` or `Y-Max` values, the fields will update to fit all of your data.
    -   Draws the resulting waveform by connecting your points.
-   This is perfect for plotting data from a spreadsheet or another program.

### 3. Use a Preset Waveform

Quickly explore classic examples of Fourier series.
-   First, set the **X-Max** and **Y-Max** to define the period and amplitude you want. For example, to create a square wave with a period of 2π and an amplitude of 1, set `X-Max` to `6.28` and `Y-Max` to `1`.
-   Click **"Square"**, **"Triangle"**, or **"Sawtooth"**.
-   The tool will generate the necessary points in the text area and plot the waveform according to your specified scales.

---

## Key Features

*   **Real-time Interaction:** All plots update instantly as you draw or change the number of harmonics with the slider.
*   **Harmonic Analysis:** Use the **"Harmonics"** slider to see how adding more sine/cosine terms improves the accuracy of the reconstructed wave.
*   **Frequency Spectrum:** The bottom chart shows the amplitude of each harmonic, giving you insight into the signal's frequency content.
*   **Auto-Scale for Clipping:** If the reconstructed wave (especially for square waves) exceeds the plot boundaries due to Gibbs phenomenon, an **"Auto-scale"** button appears. Click it to open a modal window showing the true, unclipped waveform.
*   **Zero-Dependency:** Just download the `index.html` file and open it in any modern web browser.

---

## Technical Details

*   **Frontend:** Vanilla JavaScript, HTML5, and CSS.
*   **Fourier Analysis:** Performs a Discrete Fourier Transform (DFT) to calculate the series coefficients.
*   **Path Simplification:** Uses the Ramer-Douglas-Peucker algorithm to convert freehand drawings into a manageable set of points.

---

## Contributing

Contributions are welcome! Please feel free to fork the repository, make improvements, and submit a pull request.

## License

Distributed under the MIT License. See `LICENSE` for more information.
