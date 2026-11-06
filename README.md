
# KURGAL 𒆳
<div align="center">
  <img src="KURGAL.png" alt="KURGAL Logo" width="300">
</div>
**The Great Mountain — A Next-Generation PHP Runtime.**

> *"From the primordial ocean of requests, order emerges."*

**KURGAL** is a proprietary, high-performance **Native PHP Runtime** developed by **KiGal**. 

It is designed to fundamentally change how PHP applications are deployed and executed—replacing the traditional, fragmented stack with a single, unified execution layer. 

**This repository contains the public integration files (Laravel worker scripts, examples, and SDK stubs) for the KURGAL runtime.**

---

## 🏔️ The Vision

Modern PHP stacks (like Nginx + PHP-FPM) carry inherent architectural overhead. They were designed for a different era of the web. 

KURGAL is built from the ground up to eliminate this overhead. It is not a cache, not a proxy, and not a wrapper. It is the **execution layer itself**—a native binary engineered for maximum stability, raw speed, and developer control.

We are currently in **active development**. 

---

## 📂 What's in this Repository?

This repository is the **public face** of KURGAL. It provides developers with the tools to prepare their applications for the future runtime. 

- **`examples/laravel-worker/`**: The official Laravel worker script (`worker.php`), bootstrap files, and a Dockerfile to understand the integration lifecycle.
- **`docs/`**: Public documentation on how to structure applications for a persistent worker environment.
- **`sdk/`**: Stub files to test your worker logic locally without the actual KURGAL binary.

**Note**: The core KURGAL engine is proprietary and closed-source. It will be available for licensing upon official release. This repository does not contain the runtime binary or its internal source code.

---

## 🚀 How It Will Work (Conceptual)

KURGAL shifts PHP from a "request-per-process" model to a **persistent worker model**. 

Instead of bootstrapping your framework on every single request, KURGAL allows your application to boot **once**, stay in memory, and handle thousands of requests in a continuous, lock-free loop.

*(See `examples/laravel-worker/worker.php` for the conceptual integration).*

---

## 🛡️ Status & Licensing

- **Status**: Active Development (Private Beta).
- **Source Code**: Closed-source (Proprietary).
- **Public Files License**: The integration scripts in this repository are licensed under the **MIT License**.
- **Trademark**: `KURGAL™` and the sigil `𒆳` are trademarks of **KiGal**. All rights reserved.

---

## 🤝 Stay Updated

We are not accepting public contributions to the core engine at this time. 
To follow the development of KURGAL, or to inquire about early access for enterprise deployments, please visit **[kigal.co](https://kigal.co)** (or contact us directly).

---

**Built with ❤️ by KiGal.**  
*The mountain stands unmoved.*

---
