# DM0011 · Video SFT Samples / 视频 SFT 样例

**Dataset card / 数据集卡片** · Zovda sample dataset. This repository is the GitHub mirror of the card; the data files are hosted on Hugging Face — **[download the dataset / 下载数据集](https://huggingface.co/datasets/Zovda/dm0011-video-sft-samples)**.

本仓库是数据集卡片的 GitHub 镜像，数据文件托管在 Hugging Face，**[点击下载 / download](https://huggingface.co/datasets/Zovda/dm0011-video-sft-samples)**。

| Item / 项目 | Value / 值 |
|---|---|
| Dataset ID / 数据集编号 | DM0011 |
| Files / 数据文件 | 3 |
| Size / 数据体积 | 343.41 MB |
| Language / 语言 | zh |
| Tasks / 任务类别 | video-classification, visual-question-answering |
| Hugging Face / 数据地址 | [dm0011-video-sft-samples](https://huggingface.co/datasets/Zovda/dm0011-video-sft-samples) |
| Provided by / 提供方 | Zovda |
| Contact / 联系邮箱 | lucas@zovda.com |

## Overview / 简介

High-resolution video samples spanning outdoor, industrial, animal, sports and visual-effects scenes for video SFT data construction and scene-understanding evaluation.

覆盖户外、工业、动物、运动与视觉特效等场景的高分辨率视频理解样例，可用于视频 SFT 数据构造与场景理解评测。

## What's inside / 数据内容

- 8 videos covering: a girl running to the sea (outdoor), machine-tool circuitry (industrial), refinery water flow (industrial), purple-pigment VFX (visual effects), ski follow-cam (sports), a grazing goat (animal), mountain biking (sports) and FPV park flight (sports/camera movement).
- 8 条视频，场景包括：女孩跑向海边（户外）、机床电路（工业）、炼厂水流（工业）、紫色颜料 VFX（视觉特效）、滑雪跟拍（运动）、山羊吃草（动物）、山地自行车（运动）、FPV 穿越公园（运动/运镜）。

> This repository ships 3 representative clips (one each for outdoor, industrial and VFX); the full 8-clip scene pack is delivered on request.
>
> 本仓库提供 3 条代表性视频（户外、工业、视觉特效各 1 条），完整 8 条场景包按需交付。

## Specifications / 规格

- Format: MP4 (H.264)
- 格式：MP4（H.264）
- Footage: high-resolution live action
- 画面：高分辨率实拍素材
- Organisation: file names follow `asset-id_scene-name`, usable as weak labels
- 组织：文件名为「素材编号_场景中文名」，场景可直接作为弱标签

## Suitable tasks / 适用任务

- Video instruction-tuning (SFT) data construction
- 视频指令微调（SFT）数据构造
- Scene classification and video understanding
- 场景分类与视频内容理解
- Visual reference and benchmarking for video generation
- 视频生成模型的画面参考与评测

## Files / 文件清单

Paths below are relative to the Hugging Face repository root. 下表路径相对于 Hugging Face 仓库根目录。

| # | File | Size |
|---|---|---|
| 1 | `stock-video-samples/a7082646505_女孩跑向海边.mp4` | 105.98 MB |
| 2 | `stock-video-samples/a8051309735_机床电路.mp4` | 81.06 MB |
| 3 | `stock-video-samples/a9168587977_紫色颜料VFX.mp4` | 156.36 MB |

## Download / 下载

The files are not stored in this repository. 数据文件不在本仓库内，请从 Hugging Face 获取。

- Dataset page / 数据集页面: https://huggingface.co/datasets/Zovda/dm0011-video-sft-samples
- Direct file URL / 单文件直链: `https://huggingface.co/datasets/Zovda/dm0011-video-sft-samples/resolve/main/<path from MANIFEST.csv>`

```python
from huggingface_hub import snapshot_download

snapshot_download(
    repo_id="Zovda/dm0011-video-sft-samples",
    repo_type="dataset",
    local_dir="./dm0011-video-sft-samples",
)
```

```python
from huggingface_hub import hf_hub_download

hf_hub_download(
    repo_id="Zovda/dm0011-video-sft-samples",
    repo_type="dataset",
    filename="<path from MANIFEST.csv>",
    local_dir="./dm0011-video-sft-samples",
)
```

## Rights and disclaimer / 授权与声明

Supplied by Zovda; samples demonstrate scene coverage and specification. Contact us for commercial licensing.

素材由 Zovda 供应，样例仅用于展示场景覆盖与规格。商用授权请联系我们。

This dataset is shared to demonstrate data organisation, technical specifications and delivery structure. For formal licensing, large-scale access or custom production, contact lucas@zovda.com.

本数据集仅用于展示数据组织方式、技术规格与交付结构。正式授权、规模化取数与定制生产请联系 lucas@zovda.com。

## About Zovda / 关于 Zovda

Zovda builds, cleans, annotates and packages training data across video, audio, images, e-commerce image-text pairs, exam question banks, embodied AI and coding-agent corpora.

Zovda 提供多模态与文本训练语料的数据采集、清洗、标注与结构化交付服务，覆盖视频、音频、图像、电商图文、K12 与职业题库、具身智能、代码智能体等方向。

**Contact / 联系方式:** lucas@zovda.com
