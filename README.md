# Quiz-9_Group-1

## Project Title
**Dissolving Sandscape** tentative

---

## Part 1: Project Direction

### Chosen Path

Our team has chosen **Option 2: Create an original piece**.

### Team Vision

**Dissolving Sandscape** is an interactive visual work about temporary beauty, digital material, and disappearance. The piece begins as a blank dark canvas where users can pour and shape falling sand. Over time, the sand slowly forms a fragile landscape or abstract sand painting. However, the work is not meant to stay fixed. Audio changes the colour and energy of the sand, time moves the piece through stages of building and dissolving, and Perlin noise creates wind-like erosion. Our concept is inspired by Tibetan sand mandalas, where creation and destruction are both part of the artwork, and by falling-sand simulations such as The Coding Train’s **Falling Sand** and Max Bittker’s **Sandspiel**. We want the final piece to feel alive, unstable, and temporary: a sand image that the audience helps create, then watches disappear.

![Tibetan sand mandala reference](./images/1.png)

*Figure 1. Tibetan sand mandala reference. Source: Minneapolis Institute of Art, [The Tibetan Sand Mandala: A Short History](https://new.artsmia.org/hub/programming-events/tibetan-sand-mandala-history).*

![Falling sand reference](./assets/falling-sand-reference.png)

*Figure 2. Falling sand simulation reference. Source: The Coding Train, [**Coding Challenge #180: Falling Sand**](https://thecodingtrain.com/challenges/180-falling-sand/). Example code: [p5.js Web Editor](https://editor.p5js.org/codingtrain/sketches/AoH40T6fV).*

![Sandspiel reference](./assets/sandspiel-reference.png)

*Figure 3. Interactive falling-sand sandbox reference. Source: Max Bittker, [**Sandspiel**](https://sandspiel.club/). Additional project page: [Sandspiel on itch.io](https://maxbittker.itch.io/sandspiel).*

---

## Part 2: Mechanics

| Team Member | Mechanic | Script File |
|---|---|---|
| [Name 1] | User input | `user-sand-input.js` |
| [Name 2] | Audio | `audio-colour-system.js` |
| [Name 3] | Time-based | `time-phase-controller.js` |
| [Name 4] | Perlin noise and randomness | `perlin-wind-erosion.js` |

---

### Mechanic 1: User Input — Sand Pouring and Destruction

The user input mechanic allows the audience to directly shape the sand image. When the user drags the mouse across the canvas, coloured sand particles are released from the cursor and fall under simple gravity rules. This makes the mouse feel like a digital funnel or hand tool, similar to how physical sand can be poured onto a surface. The user can build piles, draw lines, or create uneven landscapes. Later in the piece, clicking on an area will disturb the settled sand and break the image apart, causing particles to collapse or scatter. This connects to our project vision because the audience is responsible for both creation and destruction. The work becomes a temporary sand painting rather than a fixed image.

![User input sketch](./assets/user-input-sketch.png)

*Figure 4. Sketch of mouse-controlled sand pouring and click-based destruction.*

---

### Mechanic 2: Audio — Colour and Energy Response

The audio mechanic uses sound level or frequency data to control the sand’s visual energy. Instead of using sound as background music only, the audio becomes part of the material behaviour. When the volume is low, the sand can appear darker, softer, and more settled. When the volume rises, the sand can become brighter, more saturated, or more active. If we use frequency analysis, low frequencies could produce warmer colours while higher frequencies could produce sharper or lighter colours. The user does not need to sing or speak perfectly; even environmental sound or music can affect the piece. This supports the project vision by making the sand feel sensitive and alive, as if the image is reacting to the atmosphere around it.

![Audio colour reference](./assets/audio-colour-reference.png)

*Figure 5. Diagram of audio amplitude controlling sand colour and brightness.*

---

### Mechanic 3: Time-Based — Building, Settling, and Dissolving Phases

The time-based mechanic controls the overall structure of the artwork. The piece will move through several stages: a building phase, a settling phase, a dissolving phase, and a final collapse or reset phase. During the building phase, the user can actively pour sand. After a certain time, the system encourages the sand to settle, making the image feel temporarily complete. Then the dissolving phase begins, where the sand slowly loses stability and starts to fade, drift, or fall away. This mechanic helps the project avoid feeling like an endless sandbox. It gives the experience a beginning, middle, and ending. Conceptually, it connects to the idea of impermanence because even a carefully built image must eventually change and disappear.

![Time phase diagram](./assets/time-phase-diagram.png)

*Figure 6. Diagram showing the planned build, settle, dissolve, and collapse phases.*

---

### Mechanic 4: Perlin Noise and Randomness — Wind Erosion

The Perlin noise and randomness mechanic creates natural-looking movement after the sand has accumulated. Instead of making every particle fall in a straight, mechanical way, this system introduces wind, drift, and erosion. Perlin noise can create smooth directional forces, so the sand appears to move like it is being pushed by an invisible current. Randomness can add small unpredictable changes, such as individual grains sliding left or right, clumping, or breaking away from the main pile. This mechanic is important because our project is about sand as a fragile material. The noise field makes the image feel organic and unstable. It also helps the final sand painting dissolve gradually, rather than simply disappearing all at once.

![Perlin wind erosion sketch](./assets/perlin-wind-erosion-sketch.png)

*Figure 7. Sketch of Perlin-noise wind pushing sand particles across the canvas.*

---

## Part 3: Putting It Together

All mechanics share one canvas and one sand-particle system. User input creates the sand, audio changes its colour and energy, time controls the artwork’s phases, and Perlin noise gradually erodes the image. The project is held together by the concept of temporary sand painting: every interaction adds material, but every material form is unstable. Visually, the work will use a dark background, bright coloured sand, and soft fading trails so the canvas feels like a glowing digital sand table. The final piece should feel interactive, fragile, and constantly changing.

---

## References and Inspiration

- Minneapolis Institute of Art. **The Tibetan Sand Mandala: A Short History**.
- The Coding Train. **Coding Challenge #180: Falling Sand**.
- Max Bittker. **Sandspiel**.
- teamLab. **Universe of Water Particles**.
- p5.js Reference. **mousePressed(), mouseDragged(), millis(), getLevel(), noise()**.
