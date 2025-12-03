# Lyra Weather Case Study – Nîmes/Courbessac (2 December 2025)

> **Linking real-world weather to atmospheric vertical structure, with AI assistance.**  
> Radiosounding (Skew‑T) + Meteosat satellite + pressure fields + physical interpretation.

This repository documents a meteorological case study based on the **Nîmes/Courbessac** radiosonde launched on **2 December 2025 at 12:00 local time**.

The objective is **educational**:

- learning to read a **Skew‑T / emagram** rigorously,  
- cross-checking it with satellite imagery and synoptic pressure fields,  
- using an **LLM (GPT / Mistral)** to structure and deepen the analysis,  
- demonstrating how a **Human + AI workflow** accelerates learning in meteorology.

---

## 1. Repository structure

```text
.
├── README.md              # English documentation (this file)
├── README_fr.md           # French detailed version
└── graphe_images_resume/
    ├── analyse_emagramme.pdf
    ├── composition_IR_visible.png
    ├── Nimes_radiosondage.png
    ├── pressions.png
    ├── nebulosite_octas.png
    └── Visible.png
```

---

## 2. Meteorological context

- **Station:** Nîmes/Courbessac (~60 m ASL)  
- **Date / time:** Tuesday, 2 December 2025 – 12:00 LT  
- **Synoptic situation:**
  - moderate depression over northern France (1000–1004 hPa),  
  - **barometric slack** (weak gradients) over southern France (1012–1014 hPa),  
  - a large **north–south stratiform cloud band**,  
  - no deep convection (CAPE nearly zero).

Overall: a **stratiform weather regime**, with layered Sc/As clouds and weak dynamics.

---

## 3. Main results from the Skew‑T analysis

### 3.1 1000 hPa surface

The **1000 hPa** level is found around **122 m** (≈ 62 m above station elevation).

At this level:

- **T ≈ 9 °C**  
- **Tw ≈ 8 °C**  
- **RH ≈ 83 %**

### 3.2 Stratocumulus layer (~1.6–2.4 km)

Between **1585 m and 2397 m**:

- T and Td nearly identical → **saturation (RH ≈ 100 %)**  
- Temperature drops from +1.5 °C to −4.5 °C  
- Interpretation: well-defined **stratocumulus (Sc)** layer.

### 3.3 Dry layer and inversion (~2.4–2.6 km)

Between **2397 m and 2617 m**:

- temperature inversion: **+1.5 °C** over ~220 m  
- Td decreases sharply from −5 °C to −20 °C  
- Tw decreases from −5 °C to −8.5 °C  
- RH ≈ 37 %

Interpretation: **subsidence** or **advection of dry air aloft**.

### 3.4 Transition layer with near-standard lapse rate (~2.6–4.0 km)

Between **2.6 km and 4.0 km**, the temperature follows a **vertical lapse rate close to the standard atmosphere** (≈ −6 to −6.5 °C per km).

This layer shows:

- **normal atmospheric stability**,  
- no inversion or strong cooling,  
- a natural **transition** between:
  - the dry inversion layer below (~2.4–2.6 km),
  - the saturated mid-level cloud layer above (~4.0–4.3 km).

It represents a **moderately stable and dynamically neutral** portion of the profile.

### 3.5 Altostratus layer (~4.0–4.3 km)

A saturated layer appears between **4040 m and 4302 m**:

- T ≈ −10 to −11 °C  
- RH ≈ 100 %, T ≈ Td  
- Interpretation: **altostratus / thick altocumulus**.

### 3.6 Tropopause

- Tropopause height: **~11 km**  
- RH decreases to **0–5 %** → characteristic dry stratospheric air.

---

## 4. Satellite imagery and atmospheric fields

### 4.1 Meteosat 12 visible

The visible image shows:

- a **smooth, continuous north–south cloud band**,  
- stratiform texture with little convection,  
- consistent with the Sc/As layers in the radiosoundings.

### 4.2 IR / visible composite

Colors over southeastern France (grey–blue, green–yellow) indicate:

- **intermediate cloud-top temperatures**,  
- **moderate vertical extent**,  
- consistent with stratocumulus + altostratus.

### 4.3 Sea‑level pressure

- depression over northern France,  
- **weak gradients** and barometric slack over the south.

Result:  
**weak dynamics → stratiform clouds dominant**.

---

## 5. Methodology: Human + AI

### Human tasks
- precise Skew‑T reading,  
- identification of cloud layers,  
- physical interpretation.

### AI (LLM) tasks
- structuring and summarizing,  
- linking sounding ↔ satellite ↔ pressure fields,  
- improving clarity and consistency.

---

## 6. Data sources & credits

- Visualisations: **Meteociel.fr**  
- Satellite images: **EUMETSAT / Meteosat 12**  
- Radiosounding: **Météo‑France**

*Images used for educational, non‑commercial purposes.*  
