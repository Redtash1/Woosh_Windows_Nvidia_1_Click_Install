<div align="center">


# DON'T CLONE THIS REPO, IT WON'T WORK AS IT ALL DEPENDS ON THE PYTHON_EMBEDED 3.10.9 TO WORK! 


## I made this Woosh Portable 1 click install for Windows that uses Nvidia GTX 10XX, 16XX, RTX Quadro, 20XX, 30XX, 40XX, 50XX. Creates Launch Woosh & Video's, Sounds Desktop Shortcuts. 

## Click here to jump to Install 👉 [Installation](#-Installation) 👈

# ![GitHub Downloads (all assets, all releases)](https://img.shields.io/github/downloads/Redtash1/Woosh_Windows_Nvidia_1_Click_Install/total?style=for-the-badge&labelColor=orange&color=0000ff)


<img width="1528" height="497" alt="Screenshot 2026-05-03 003719" src="https://github.com/user-attachments/assets/f78a6758-ad8a-4a8b-b2e2-c0b124307788" />

----

<img width="1530" height="829" alt="Screenshot 2026-05-03 003753" src="https://github.com/user-attachments/assets/1ee8603d-ea98-4549-a81c-16460db728d5" />

</div>

----

# Woosh - Sound Effect Generative Models

This repository provides inference code and open weights for the sound effect generative models developed at Sony AI. The
current public release includes four models addressing the text-to-audio (T2A) and video-to-
audio (V2A) tasks:

- **Audio encoder/decoder (Woosh-AE)**: High-quality latent encoder/decoder providing latents
for generative modeling and decoding audio from generated latents.

- **Text conditioning (Woosh-CLAP)**: Multimodal text-audio alignment model providing token la-
tents for diffusion model conditioning.

- **T2A Generation (Woosh-Flow and Woosh-DFlow)**: Original and distilled LDMs generating au-
dio unconditionally or from given a text prompt.

- **V2A Generation (Woosh-VFlow)**: Multimodal LDM generating audio from a video sequence
with optional text prompts.


# 📦 Installation

## Nvidia GTX 10XX, 16XX, RTX Quadro, 20XX, 30XX, 40XX, 50XX  

## GTX 10XX-RTX 30XX will have torch 2.6.0+cu126 installed for compatibility. RTX 40XX & 50XX will have torch 2.8.0+cu128.

## Text to audio requires 6GB VRAM. 
## Video with audio requires 8GB VRAM or more.


1. Make sure you have Git installed as it will be needed to update Index TTS, if not download the Git Standalone Installer and click on Git for Windows/x64 Setup. 👉 [Git Standalone Installer Download](https://git-scm.com/downloads/win) 👈 To install Git, double click Git.exe and just keep clicking next until it's installed, you don't need to change anything.


2. Make sure your Nvidia graphics drivers are up-to-date. If they are not or if your not sure, please click on the following link to download Nvidia graphics drivers. 👉 [Nvidia Drivers](https://www.nvidia.com/en-us/software/nvidia-app/) 👈

3. Make sure that you have NVIDIA's [CUDA Toolkit](https://developer.nvidia.com/cuda-toolkit) version **12.8** (or newer) installed on your system.

4. Make sure you have FFMPEG Shared downloaded & on PATH. Download 👉 [ffmpeg-release-full-shared.7z](https://www.gyan.dev/ffmpeg/builds/) 👈

5.  Now after you have made sure Nvidia GPU drivers are up to date and Git is installed, download Woosh Windows Nvidia 1 Click Install
 from here 👉 [Index TTS2 Windows 1 Click Install](https://github.com/Redtash1/index_tts_Windows_1_Click_Install/releases) 👈 or from the Releases section at the top right of this page.

6. After downloading, extract Woosh Windows Nvidia 1 Click Install ZIP file and pick where you would like to extract the zip files too.

7. Then open Woosh Windows Nvidia 1 Click Install main folder, you will see this in the root
----

<img width="755" height="220" alt="Screenshot 2026-05-03 004054" src="https://github.com/user-attachments/assets/302cd4b0-2787-475a-b313-7682aba2fef3" />

----
8. Then depending on your Nvidia GPU double click on either the Install_Woosh_GTX_10XX_to_RTX_30XX.bat or Install_Woosh_RTX_40XX_&_50XX.bat to start the installation. It will install everything and download the models via Huggingface.  After installation is finished, slowly scroll back up to the top to make sure everything installed correctly.

9. To launch Woosh double click the Launch_Woosh.bat.

### If this worked for you, Please give it a Star ⭐. Thank you.

----
## API server
Woosh models can be served via our API server. Check the [API](api/) folder for usage details.

## Citation
For details about model architecture, training and evaluation, please check our tech report
available on [arxiv.org](https://arxiv.org/abs/2604.01929).

```bibtex
@misc{hadjeres2026,
      title={Woosh: A Sound Effects Foundation Model},
      author={Gaetan Hadjeres, Marc Ferras, Khaled Koutini, Benno Weck, Alexandre Bittar, Thomas Hummel, Zineb Lahrichi, Hakim Missoum, Joan Serrà and Yuki Mitsufuji},
      year={2026},
      eprint={2604.01929},
      archivePrefix={arXiv},
      primaryClass={cs.SD},
      url={https://arxiv.org/abs/2604.01929},
}
```


## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
- The majority of the code in this repository is released under the [MIT](https://choosealicense.com/licenses/mit/) license. The video-to-audio `Woosh-VFlow` and `Woosh-DVFlow` models use adapted code from [MM-AUDIO](https://github.com/hkchengrex/MMAudio) and [MotionFormer](https://github.com/facebookresearch/Motionformer/). The code for these models is made available under [Apache v2](https://www.apache.org/licenses/LICENSE-2.0) license terms.
- The open weights in the [releases](https://github.com/SonyResearch/woosh-sfx/releases) page are released under the [CC-BY-NC](https://creativecommons.org/licenses/by-nc/4.0/) license.
- The test audio and video samples in the [releases](https://github.com/SonyResearch/woosh-sfx/releases) page contain their individual license terms in the corresponding download file.
