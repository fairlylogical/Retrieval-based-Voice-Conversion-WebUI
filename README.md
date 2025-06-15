see https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI for the original README
# 🎹 RVC WebUI (ARM64 Docker Image)

This branch provides a Dockerized version of the [RVC Voice Conversion WebUI](https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI) — specifically built for the **ARM64 architecture** (e.g. Apple Silicon Macs, Raspberry Pi 4/5, ARM servers).

---

## 📦 Features

* ✅ ARM64-native image (no emulation needed)
* ✅ Built from official RVC WebUI repo
* ✅ Optimized for use on M1/M2 Macs, Jetson, Raspberry Pi

---

## 💋 Build Instructions (ARM64)

### 1. Clone the repo

```bash
git clone https://github.com/fairlylogical/Retrieval-based-Voice-Conversion-WebUI.git
cd Retrieval-based-Voice-Conversion-WebUI
git checkout -B arm64
```


### 2. Build the Image (locally for ARM64)

```bash
docker build -f Dockerfile.arm64 -t rvc-webui:arm64 .
```

## 📂 Running the Image

```bash
docker run --rm -p 7865:7865 rvc-webui:arm64
```

Then open [http://localhost:7865](http://localhost:7865)

---

## 📜 License

This repo builds on top of [RVC WebUI](https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI) — all credit goes to the original developers.
