# DDoS-Simulation-Mitigation-Report
# 🛡️ Cloud DDoS Simulation & Mitigation Report

This repository contains a security assessment report focused on simulating a controlled **DDoS (Distributed Denial of Service)** attack against a cloud-hosted web application and evaluating the effectiveness of cloud-native protection tools (e.g., AWS Shield).

---

## 📋 Report Overview

The report includes:
- ✅ A basic web application deployed on an AWS EC2 instance
- ✅ Low-impact DDoS simulation using `hping3`
- ✅ Monitoring via AWS CloudWatch
- ✅ Analysis of AWS Shield's response
- ✅ Recommendations for layered mitigation strategies

---

## 🔍 Simulation Details

- **Target**: Static HTML page hosted via Apache on AWS EC2
- **Attack Tool**: `hping3` (SYN flood, 5-minute duration)
- **Monitoring**: AWS CloudWatch (CPU, network metrics, response time)
- **Cloud Protection**: AWS Shield Standard

---

## 🧪 Key Observations

- Increased CPU & network metrics during attack
- Slight latency (60–80ms) without service crash
- No alerts triggered due to low-scale simulation
- AWS Shield absorbed traffic automatically

---

## 🔐 Recommended Mitigations

- 🔸 **AWS WAF** – Rule-based filtering of suspicious traffic
- 🔸 **Rate Limiting** – Restrict request frequency per IP
- 🔸 **Geo-blocking** – Limit access to necessary regions
- 🔸 **CloudFront CDN** – Distribute traffic & absorb load spikes
- 🔸 **Auto Scaling** – Add capacity under stress

---

## 📥 Download the Report

[📄 Click here to download the full PDF](https://github.com/your-username/your-repo-name/blob/main/DDoS_Simulation_Report.pdf)

> Replace the link above with your actual GitHub username and repo name.

---

## ⚠️ Disclaimer

This simulation was performed in a controlled and ethical manner, strictly for educational and defensive security testing purposes.  
Always consult your cloud provider’s acceptable use policies before performing simulations.

---

## 📌 License

This repository is for academic and non-commercial use only.
