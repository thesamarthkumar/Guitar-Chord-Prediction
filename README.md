# Guitar Chord Prediction via Multilayer Perceptron

A PyTorch project that predicts guitar chord roots based on finger positions and chord structures.
Compares a nn.Linear–based MLP with NdLinear–based MLP.

---

## Features

- Loads and preprocesses the dataset.  
- Encodes chord roots, structures, and string‐by‐string finger positions.  
- Trains two MLP classifiers:
  1. One model using standard nn.Linear layers.  
  2. One Model using the custom NdLinear layer.  
- Evaluates both models (accuracy, classification reports, confusion matrices).

---

## Python Version and Libraries

- **Python** 3.11+  
- **PyTorch**  
- **NumPy** & **Pandas**  
- **scikit‑learn**  
- **NdLinear** 


---

## Dataset

This project uses the [Guitar Chords Finger Positions dataset](https://archive.ics.uci.edu/dataset/575/guitar+chords+finger+positions) from the UCI Machine Learning Repository:

- **CHORD_ROOT**: root note of the chord <- Target Variable
- **CHORD_TYPE**: major, minor, 7th, etc.
- **CHORD_STRUCTURE**: intervals of the chord (e.g. '1;3;5;b7').  
- **FINGER_POSITIONS**: finger placements on the 6 strings ('x,1,0,2,3,4').  
- **NOTE_NAMES**: names of each note forming the chord ('A#,C##,G#,B#,F##').

CSV file is also included.

---

## Installation

1. **Clone** this repository:
   ```bash
   git clone https://github.com/thesamarthkumar/Guitar-Chord-Prediction.git
   cd Guitar-Chord-Prediction
  
