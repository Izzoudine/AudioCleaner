Sure! Here's the English version for your `README.md` file:

---

### 🎯 Model Evaluation Metrics

To assess the performance of the noise reduction model, we selected metrics specifically suited for signal enhancement tasks, combining both objective and perceptual evaluations.

#### 📶 Signal-to-Noise Ratio (SNR)
**SNR** measures the proportion of **signal power** relative to **noise power** in the audio.  
A higher SNR indicates that the model has effectively reduced the noise while preserving the original signal.  
> 🔍 **Interpretation**: The higher the SNR after processing, the better the quality of the cleaned signal.

#### 🗣️ Perceptual Evaluation of Speech Quality (PESQ)
**PESQ** is a standardized metric for evaluating the **perceived quality of speech** after processing, based on the **intelligibility** and **fidelity** of the signal.  
It provides a score that closely reflects how a human would perceive the audio quality.
> 🎧 **Use case**: Widely used in telecommunications and speech enhancement applications.

#### 🧠 Short-Time Objective Intelligibility (STOI)
**STOI** measures the **intelligibility of speech** in processed audio signals.  
It ensures that speech remains understandable after noise has been removed.
> 🎯 **Best for**: Applications where speech clarity is crucial, such as voice assistants, transcription, and communication systems.

---

### 🧠 Learning Approach

The model uses a **Transfer Learning** strategy, leveraging powerful pre-trained models such as **Demucs**, **DeepFilterNet**, and **RNNoise**.  
This approach allows us to:
- Avoid the need for large labeled datasets
- Benefit from strong baseline performance
- Accelerate training with high starting accuracy

---

Let me know if you’d like a matching section about the model architecture or use case description!
