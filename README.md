# The 10-Floor Tower of Judgment

> *"A 10-tier cyber-brutalist spatial puzzle game built entirely in a single HTML file—featuring zero external dependencies, CSS 3D perspective projection, procedural Web Audio, and voice-synthesized psychological damage."*

---

## 👁️ Overview

**The 10-Floor Tower of Judgment** (also titled **The Tower of Justice**) is a first-person 3D browser escape-room satire. Players find themselves trapped in a minimalist, neon-etched testing complex where every floor personifies a classic developer or academic nightmare: procrastination, corporate sycophancy, CSS centering agony, tutorial hell, imposter syndrome, and burnout.

Unlike standard escape rooms that rely on point-and-click pixel hunting, **The Tower of Judgment** evaluates behavioral and spatial input: ramming walls with your head, spinning in an executive office chair, freezing in pure panic, or frantically scrolling into the void.

---

## ✨ Features & Architecture

- **Zero-Library 3D Spatial Engine**:
  - Rendered entirely with native CSS3 transforms (`preserve-3d`, `perspective: 900px`, `rotateX`, `rotateY`, and `translate3d`).
  - Smooth camera yaw and position interpolation implemented via an internal `requestAnimationFrame` loop.
- **Procedural Web Audio Engine**:
  - Uses native browser `AudioContext` and dynamic `OscillatorNode` synthesis.
  - Generates custom sounds for physical collisions ("bonks"), decrypting plaques, elevator transitions, and timeline glitch sirens without loading any external `.mp3` or `.wav` files.
- **Live Text-to-Speech (TTS) Curator**:
  - Integrated via the browser's `SpeechSynthesis` API to deliver spoken roasts and condescending remarks when you fail, beg, or progress.
- **Evasive Micro-Mechanics**:
  - **The Roaming Curator Button**: A "Beg for Hint" button that senses cursor velocity ($\Delta d / \Delta t$) and teleports away if approached too quickly. Players must sneak up on it slowly to interact.
- **Hidden Passphrase Buffer**:
  - Listens globally to keystrokes in real-time, streaming your input into the HUD's secret buffer.
- **Timeline Mutation Trap**:
  - Making common spelling blunders on Floor 7 triggers a complete reality collapse, resetting the tower to Floor 0 with mutated puzzle mechanics, altered clues, and new passphrases.

---

## 🎮 Controls

| Input | Action |
| :--- | :--- |
| <kbd>W</kbd> <kbd>A</kbd> <kbd>S</kbd> <kbd>D</kbd> / <kbd>Arrows</kbd> | Move forward, backward, and strafe |
| <kbd>Q</kbd> / <kbd>E</kbd> | Continuous 3D rotation / swivel (Hold down) |
| <kbd>Mouse Move</kbd> | Look around chamber angles / pitch |
| <kbd>Mouse Wheel</kbd> | Rapid camera zoom / movement translation |
| <kbd>Keyboard Keys</kbd> | Type the floor's passphrase anywhere at any time |
| <kbd>Esc</kbd> / <kbd>Enter</kbd> | Dismiss active dossiers, menus, and modals |

---

## 🏢 Tower Blueprint & Floor Directory

To decrypt the clues on any floor, you must first obtain Curator clearance (by stealthily approaching and clicking the roaming **"Beg Curator for Hint"** button) and perform the floor's specific behavior:

| Tier | Floor Name | Decryption Mechanism |
| :---: | :--- | :--- | :---: |
| **0** | **Ground Zero: Procrastination** | Repeatedly ram into walls until structural integrity cracks |
| **1** | **Corporate Sycophant Suite** | Hold <kbd>Q</kbd> or <kbd>E</kbd> to complete a 360° executive swivel
| **2** | **Overleaf & Academic Hell** | Stop all input and freeze in dead silence for 3.5 seconds
| **3** | **CSS Centering Purgatory** | Stand dead in the exact center ($X \approx 0, Z \approx 0$) for 2 seconds
| **4** | **Tutorial Hell Wasteland** | Rapidly hammer movement inputs like an ape copying code
| **5** | **Impostor Syndrome Labyrinth** | Vigorously shake your mouse back and forth in panic
| **6** | **Protocol 67 Matrix Anomaly** | Spin your mouse wheel continuously to crack the buffer
| **7** | **Burnout & Palpitations** | Execute choreographed rebound wall sequences
| **8** | **Antechamber of Revelation** | Walk into and register all 4 chamber corners
| **9** | **The Summit Vault of Truth** | All plaques open; inspect the South Wall memorandum

---

## ⚠️ The Caffeine Hazard & Mutated Timeline

On **Floor 7**, entering common misspellings of the word `caffeine` (such as `caffiene`, `caffein`, `cafiene`, etc.) will trigger an alarm:
1. Progress is wiped back down to Floor 0.
2. Floors 0 through 6 mutate into alternate variations:
   - **FL 0**: Reverse traction (walk backward into walls).
   - **FL 1**: Strafe oscillation (alternate <kbd>A</kbd> and <kbd>D</kbd>).
   - **FL 2**: High-velocity panic tremor keystrokes.
   - **FL 3**: Peripheral grid slide (slide into outer room corners).
   - **FL 4**: Rapid mouse-clicking spam.
   - **FL 5**: Alternating head-shake turns (<kbd>Q</kbd> / <kbd>E</kbd> switching).
   - **FL 6**: Reboot diagnostic circuit (touch North $\rightarrow$ East $\rightarrow$ South).

---

## 🚀 Running the Project

Because the entire application is contained in a single standalone file, no compilation, bundler, or server environment is required.

1. Clone or download the repository.
2. Open `index.html` directly in any modern desktop browser (Chrome, Firefox, Edge, Safari, Brave).
3. Click anywhere on the canvas or press <kbd>Enter</kbd> to allow browser audio permissions and start ascending.
