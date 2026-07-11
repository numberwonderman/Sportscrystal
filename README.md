# Sports Crystal: 3D Elo Predictor
### Built for United Hacks V7

A stylized, interactive 3D sports outcome predictor. Using Elo rating differentials, the Sports Crystal dynamically visualizes match win probabilities through a 3D persistent-spin engine.

## 🚀 How it Works
The Crystal acts as a real-time data visualization engine, combining rigorous mathematical modeling with immersive 3D rendering.
* **Color-Coded Analysis:** The crystal shifts color based on the favored team (Blue for Home, Red for Away, Purple for an even Toss-up).
* **Dynamic Velocity:** The rotation speed of the 3D cube is proportional to the confidence of the prediction—the more lopsided the matchup, the faster the crystal spins.
* **True 3D Rendering:** Powered by [Three.js](https://threejs.org/), ensuring a high-performance, non-flattening 3D geometry that remains stable regardless of the prediction.

## 📜 Project History
The "Sports Crystal" began as an experiment in aesthetic data visualization, drawing inspiration from the **long history of scrying**—the practice of gazing into a reflective object to seek insight. We wanted our project to modernize this practice, using sports data as the "influence" and the 3D cube as the reflective surface.

We transitioned to a **cube** for its structural integrity and geometric clarity; while spheres are traditional, the cube represents the **stability and groundedness** of calculated data. This version of the project represents our final pivot to a WebGL-based architecture using Three.js, resolving previous CSS-based rendering limitations. You may find similar conceptual prototypes in this repository; they serve as a record of the technical trial-and-error process that led to this final engine.

## 📈 Prediction Logic
The core prediction logic utilizes an Elo-based ranking system. The probability of the home team ($P_H$) winning is calculated as follows:

$$P_{H} = \frac{1}{1 + 10^{\frac{R_{A} - R_{H}}{400}}}$$

*Where $R_{H}$ and $R_{A}$ are the Elo ratings of the Home and Away teams.*

## ⚠️ Ethical Disclaimer
This project is for educational and entertainment purposes only. The "Sports Crystal" uses historical Elo ratings to calculate probabilities based on statistical trends; it does not account for real-world variables such as player injuries or weather conditions. This tool should not be used to influence gambling or financial decisions.

## 🛠 Tech Stack
* **Frontend:** HTML5, CSS3 (Responsive Design)
* **3D Engine:** [Three.js](https://threejs.org/) (WebGL rendering)
* **Performance:** Pure client-side logic; offline-capable via caching.
