# Sports Crystal: 3D Elo Predictor
### Built for United Hacks V7

A stylized, interactive 3D sports outcome predictor. Using Elo rating differentials, I built the Sports Crystal to dynamically visualize match win probabilities through a 3D persistent-spin engine.

## 🚀 How it Works
The Crystal acts as a real-time data visualization engine, combining rigorous mathematical modeling with immersive 3D rendering.
* **Color-Coded Analysis:** The crystal shifts color based on the favored team (Blue for Home, Red for Away, Purple for an even Toss-up).
* **Dynamic Velocity:** The rotation speed of the 3D cube is proportional to the confidence of the prediction—the more lopsided the matchup, the faster the crystal spins.
* **True 3D Rendering:** Powered by [Three.js](https://threejs.org/), ensuring a high-performance, non-flattening 3D geometry that remains stable regardless of the prediction.

## 📜 Project History
The "Sports Crystal" was developed entirely within the **United Hacks V7 hackathon window**. 

The project began as an exploratory experiment in aesthetic data visualization, drawing inspiration from the ancient practice of **scrying**—the art of seeking insight by gazing into a reflective medium. During the early hours of the hackathon, I focused on rapid prototyping, using CSS 3D transforms to bring the "Crystal" to life. As I iterated, I encountered technical limitations with depth-flattening that threatened the visual stability of my core concept. 

Rather than abandoning the vision, I committed to an aggressive pivot midway through the competition, migrating to a robust, WebGL-based architecture using **Three.js**. This transition allowed me to resolve rendering issues and achieve the persistent, true-3D rotation I initially envisioned. The prototypes visible in this repository serve as a record of my intensive, real-time iterative process throughout the hackathon—demonstrating my technical trial-and-error and my commitment to building a high-performance engine under pressure.

## 🔮 The Art of Scrying & The Cubic Form
The concept of the "Sports Crystal" draws inspiration from the ancient practice of scrying. While traditional scrying often utilizes spheres, the **Sports Crystal** utilizes a cubic geometry. This choice is intentional: in crystal lore, the cube represents **stability, groundedness, and the structure of data.** By using a cubic form, my visualization aims to stabilize the chaotic nature of sports predictions, grounding the "visions" of the engine in firm, calculated mathematical reality.

## 📈 Prediction Logic
The core prediction logic utilizes an Elo-based ranking system. The probability of the home team ($P_{H}$) winning is calculated as follows:

$$P_{H} = \frac{1}{1 + 10^{\frac{R_{A} - R_{H}}{400}}}$$

*Where $R_{H}$ and $R_{A}$ are the Elo ratings of the Home and Away teams.*

## ⚠️ Ethical Disclaimer
This project is for educational and entertainment purposes only. The "Sports Crystal" uses historical Elo ratings to calculate probabilities based on statistical trends; it does not account for real-world variables such as player injuries or weather conditions. This tool should not be used to influence gambling or financial decisions.

## 🛠 Tech Stack
* **Frontend:** HTML5, CSS3 (Responsive Design)
* **3D Engine:** [Three.js](https://threejs.org/) (WebGL rendering)
* **Performance:** Pure client-side logic; offline-capable via caching.
