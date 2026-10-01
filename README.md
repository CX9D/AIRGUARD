# AIRGUARD v2.0: Automated Vehicle Exhaust Monitoring Platform

An open-source, zero-budget computer vision framework engineered to process local traffic camera ingress fields for real-time smoke opacity metrics and localized vehicle filtering.

## 🛠️ System Architecture Pipeline

The framework is divided into two decoupled layers to run 100% free with unlimited compute thresholds:

1. **Frontend Interface UI (GitHub Pages):** A lightweight, static dark-themed analytical dashboard designed for immediate user data delivery.
2. **AI Processing Brain (Google Colab Edge Node):** A remote cloud server accelerated by free T4 GPU allocations running background inference.

## ⚙️ Core Processing Steps

*   **Phase 1: Video Collection (Ingress):** Real-world traffic streams are captured at 30-60 FPS via a smartphone node overlooking high-density road bottlenecks (e.g., NHCE Footover Bridge, Outer Ring Road).
*   **Phase 2: Object Tracking & Segmentation:** The system utilizes a lightweight **YOLOv8** convolutional neural network to isolate moving vehicles (cars, buses, trucks) and project an automated bounding zone directly over the tailpipe trajectory.
*   **Phase 3: Software-Defined Sensor Layer:** Rather than deploying expensive physical sensors, an **OpenCV processing loop** isolates volatile smoke plumes via Background Subtraction and computes dynamic light attenuation against the road surface matrix using pixel darkness metrics.

## 📈 System Benchmark Targets
*   **Vehicle Bounding Precision:** ~93.5%
*   **Processing Latency Rate:** <45ms per frame execution
*   **Infrastructure Overhead Cost:** ₹0.00 (Pure Cloud Free-Tier Framework)
