# Character-level RNN (GRU) – NLP Assignment

**Course:** Natural Language Processing  
**Student Name:** Tejaswini Kolluru  
**Student ID:** 700773943

---

## 🎯 Goal
Train a tiny **character-level RNN** to predict the next character in a text sequence, using **PyTorch**.

**Architecture:**  
`Embedding → GRU → Linear → Softmax`

**Training Method:**  
Teacher forcing, cross-entropy loss, Adam optimizer.

---

## 🧩 Dataset
- **Option 1:** Small toy corpus (like "hello", "help", etc.)  
- **Option 2:** Auto-download a 100–200 KB public-domain text (e.g., *Pride and Prejudice*)  
- **Option 3:** Upload your own `.txt` file  

---

## 🧠 Model & Training
- Hidden size: 64–256 (default: 128)  
- Sequence length: 50–100 (default: 100)  
- Batch size: 64  
- Trained for 5–20 epochs  
- Teacher forcing used for stable learning  

---

## 📈 Results
1. **Training and Validation Loss Curves:**  
   Plotted at the end of training.  
2. **Sample Generations:**  
   3 outputs at different temperatures (τ = 0.7, 1.0, 1.2), each 200–400 characters long.  
3. **Reflection:**  
   Discusses the effect of sequence length, hidden size, and temperature.  
   Also connects to slides on embeddings, sampling loop, teacher forcing, and model tradeoffs.

---

## 📚 Connection to Lecture Slides
- **Embedding:** Encodes characters into dense representations for learning relationships.  
- **Sampling Loop:** Generates text one character at a time using model predictions.  
- **Teacher Forcing:** Stabilizes training by feeding the real previous character.  
- **Tradeoffs:** GRUs offer efficiency and strong performance compared to LSTMs.  
- **Transformers:** Modern models like GPT extend these ideas using attention instead of recurrence.
