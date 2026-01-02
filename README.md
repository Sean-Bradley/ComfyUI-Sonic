# ComfyUI Sonic

Custom node that takes an audio mp3 and an image, and creates a lip synced video from them.

## Install `ComfyUI Sonic` Custom Node

Install the custom node `ComfyUI Sonic` using the manager, or you can use your command/terminal prompt.

1. Navigate to your `./ComfyUI_windows_portable/ComfyUI/custom_nodes` folder.
2. Run,
   ```bash
   git clone https://github.com/Sean-Bradley/ComfyUI-Sonic
   ```
3. Navigate to your `./ComfyUI_windows_portable` folder.
4. Run
   ```
   python_embeded\python -m pip install -r ComfyUI/custom_nodes/ComfyUI-Sonic/requirements.txt
   ```
5. Restart ComfyUI

## Install Models

We need to create this folder structure and download each model into its place.

```text
📂 ComfyUI/
├── 📂 models/
│   └── 📂 sonic/
│       ├── audio2bucket.pth
│       ├── audio2token.pth
│       ├── unet.pth
│       ├── face_yolov8m.pt
│       ├── 📂 whisper-tiny/
│       │   ├── config.json
│       │   ├── model.safetensors
│       │   └── preprocessor_config.json
│       └── 📂 RIFE/
│           └── flownet.pkl
```

Download each file and place into your `./ComfyUI/models/sonic/` folder

- [audio2bucket.pth](https://huggingface.co/Sean-Bradley/ComfyUI/tree/main/models/sonic){target=\_blank}
- [audio2token.pth](https://huggingface.co/Sean-Bradley/ComfyUI/tree/main/models/sonic){target=\_blank}
- [unet.pth](https://huggingface.co/Sean-Bradley/ComfyUI/tree/main/models/sonic){target=\_blank}
- [face_yolov8m.pt](https://huggingface.co/Sean-Bradley/ComfyUI/tree/main/models/sonic){target=\_blank}

Download each file and place into your `./ComfyUI/models/sonic/whisper-tiny/` folder

[config.json](https://huggingface.co/Sean-Bradley/ComfyUI/tree/main/models/sonic/whisper-tiny){target=\_blank}
[model.safetensors](https://huggingface.co/Sean-Bradley/ComfyUI/tree/main/models/sonic/whisper-tiny){target=\_blank}
[preprocessor_config.json](https://huggingface.co/Sean-Bradley/ComfyUI/tree/main/models/sonic/whisper-tiny){target=\_blank}

Download this file and place into your `./ComfyUI/models/sonic/RIFE/` folder

[flownet.pkl](https://huggingface.co/Sean-Bradley/ComfyUI/tree/main/models/sonic/RIFE){target=\_blank}

<!-- Download `audio2bucket.pth`,`audio2token.pth`, `unet.pth`, `yoloface_v5m.pt` and `flownet.pkl` from [https://drive.google.com/drive/folders/1oe8VTPUy0-MHHW2a_NJ1F8xL-0VN5G7W](https://drive.google.com/drive/folders/1oe8VTPUy0-MHHW2a_NJ1F8xL-0VN5G7W){target=\_blank}

Download `config.json`, `model.safetensors` and `preprocessor_config.json` from [https://huggingface.co/openai/whisper-tiny/tree/main](https://huggingface.co/openai/whisper-tiny/tree/main){target=\_blank} -->

## Sample Workflows

> [!TIP]
> For easier drag/drop of workflows into ComfyUI, visit https://sbcode.net/genai/lipsync-sonic/

Download this <a href="docs/example.mp3" download style="white-space: nowrap">Example Audio</a> and save into your `ComfyUI/input` folder.

| Initial Image                                                     | Workflow                                                        |
| ----------------------------------------------------------------- | --------------------------------------------------------------- |
| <img src="docs/sonic-1.png" style="max-height:250px"/>            | ![](docs/sonic-1-workflow.png)                                  |
| <img src="docs/sonic-2.png" style="max-height:250px"/>            | ![](docs/sonic-2-workflow.png)                                  |
| <img src="docs/girl-with-freckels.png" style="max-height:250px"/> | ![](docs/sonic-3-workflow.png)                                  |
| <img src="docs/sonic-4.png" style="max-height:250px"/>            | ![](docs/sonic-4-workflow.png)                                  |
| <img src="docs/ltxv-karate.png" style="max-height:250px"/>        | ![](docs/sonic-5-workflow.png)                                  |
| <img src="docs/ComfyUI_02591_.png" style="max-height:250px"/>     | <img src="docs/sonic-6-workflow.png" style="max-height:250px"/> |
| <img src="docs/ComfyUI_02372_.png" style="max-height:250px"/>     | <img src="docs/sonic-7-workflow.png" style="max-height:250px"/> |
| <img src="docs/sonic-8.png" style="max-height:250px"/>            | <img src="docs/sonic-8-workflow.png" style="max-height:250px"/> |
| <img src="docs/sonic-9.png" style="max-height:250px"/>            | <img src="docs/sonic-9-workflow.png" style="max-height:250px"/> |
