# uavs3d-cuda
A high-performance AVS3 video decoder with NVIDIA CUDA hardware acceleration, based on the [uavs3d](https://github.com/uavs3/uavs3d) open-source project.

## Features

- AVS3-P2 Baseline Profile full support
- 8K-10-bit video decoding
- CUDA-accelerated Reconstruction (Luma & Chroma)
- CUDA-accelerated SAO (Sample Adaptive Offset) filter
- CUDA-accelerated ALF (Adaptive Loop Filter)
- CUDA-accelerated MC average pixel for large blocks (64/128)
- SSE4/AVX2 optimizations retained on CPU side
- Automatic CUDA detection with CPU fallback

## Source Code

The CUDA acceleration source code is pending release. I have reached out to the original author of uavs3d for permission and am currently awaiting their response. The source code will be published here once I receive confirmation.

In the meantime, the demo videos above showcase the decoder's capability in real-time 8K AVS3 playback.

## Requirements

| Component | Version |
|-----------|---------|
| CMake | >= 3.10 |
| CUDA Toolkit | >= 10.0 (11.0+ recommended) |
| GCC / MSVC | C99 / C++11 |
| FFmpeg (player) | >= 4.0 |
| SDL2 (player) | >= 2.0.10 |

**GPU**: NVIDIA GPU with CUDA

## 120Mbps-AVS3-CCTV8K-Play demo
Capture the display by Nvidia DXGI and Nvenc. And the relevant video is attached.

https://github.com/user-attachments/assets/f75a132a-aa4f-4ef3-aa00-1382ae068a1f

https://github.com/user-attachments/assets/8caa76c1-41f9-4668-8f24-03365c9ede23

https://github.com/user-attachments/assets/a83a46fe-b729-4bc6-a070-3fe05dacb7fc

https://github.com/user-attachments/assets/1cfab9ca-f66a-4805-84fe-9b14eee95446



## 120Mbps-AVS3-CCTV8K-demo
The codes can be running at VS2019 with CUDA compile. And AVS3 video decoder with NVIDIA CUDA hardware acceleration is shown in CPU-13900KF and GTX1060.

<img width="3440" height="1440" alt="无标题" src="https://github.com/user-attachments/assets/28e33971-7669-4606-ae71-37f2f77cd57b" />
<img width="3440" height="1440" alt="无标题2" src="https://github.com/user-attachments/assets/0826cb33-febe-41b9-b9d6-7efbc3274f3f" />
<img width="3440" height="1440" alt="无标题3" src="https://github.com/user-attachments/assets/0949e75f-b789-4083-975f-98d3c33c679b" />


## License
BSD 3-Clause License. See COPYING for details.

## Acknowledgements
uavs3d - High-performance AVS3 software decoder
Copyright: Peking University Shenzhen Graduate School, Peng Cheng Laboratory, Guangdong Bohua UHD Innovation Corporation

