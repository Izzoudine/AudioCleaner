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

# Audio Noise Reduction Models Comparison

## Demucs
- **Focus:** Originally for music source separation, excellent for general noise reduction
- **Strengths:** Highest quality separation, handles complex noise, MIT license
- **Limitations:** Computationally intensive, larger model size
- **Best for:** Projects where quality is the top priority

## DeepFilterNet
- **Focus:** Speech enhancement and noise suppression
- **Strengths:** Natural sound preservation, good balance of quality/efficiency
- **Limitations:** Less effective on non-speech audio
- **Best for:** Voice recordings, podcasts, and interviews

## RNNoise
- **Focus:** Real-time voice noise reduction
- **Strengths:** Extremely lightweight, low latency, runs on minimal hardware
- **Limitations:** Lower quality than larger models, voice-specific
- **Best for:** Real-time applications, mobile devices, live communication

Choose **Demucs** for highest quality, **DeepFilterNet** for balanced performance, or **RNNoise** for efficiency and real-time use.

| Feature | Demucs | DeepFilterNet | RNNoise |
|---------|--------|---------------|---------|
| **Primary Focus** | Music/general audio separation | Speech enhancement | Voice communication |
| **Quality** | ★★★★★ | ★★★★☆ | ★★★☆☆ |
| **Efficiency** | ★★☆☆☆ | ★★★★☆ | ★★★★★ |
| **Real-time Capability** | Limited | Good | Excellent |
| **Model Size** | Large | Medium | Small |
| **Implementation Complexity** | Medium | Medium | Low |
| **Best Use Case** | High-quality offline processing | Balanced quality/performance | Real-time applications |

