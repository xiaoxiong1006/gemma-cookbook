# 欢迎来到Gemma Cookbook
这是一系列关于[Google Gemma](https://ai.google.dev/gemma/)的指南和示例的合集。Gemma 是一系列先进的轻量级开放模型， 采用了与打造 Gemini 模型相同的研究和技术。

## 开始使用Gemma模型
Gemma 是一系列先进的轻量级开放模型， 采用了与打造 Gemini 模型相同的研究和技术。Gemma模型系列包括：
* Gemma 基础模型
  * [Gemma](https://ai.google.dev/gemma/docs/model_card)
  * [Gemma 2](https://ai.google.dev/gemma/docs/model_card_2)
* Gemma 变体
  * [CodeGemma](https://ai.google.dev/gemma/docs/codegemma)
  * [PaliGemma](https://ai.google.dev/gemma/docs/paligemma)
  * [RecurrentGemma](https://ai.google.dev/gemma/docs/recurrentgemma)
  * [ShieldGemma](https://ai.google.dev/gemma/docs/shieldgemma)

您可以在GitHub, Hugging Face models, Kaggle, Google Cloud Vertex AI Model Garden, and [ai.nvidia.com](ai.nvidia.com)找到Gemma模型。

## 目录

| 名称                                                                                                                                          | 简介                                                                                                                                                                             |
| ------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Common_use_cases.ipynb](Common_use_cases.ipynb)                                                                                                 |  展示 Gemma、CodeGemma 和 PaliGemma 的一些常见用例。                                                                                                                  |
| **Gemma**                                                                                                                                        |
| [Keras_Gemma_2_Quickstart.ipynb](Gemma/Keras_Gemma_2_Quickstart.ipynb)                                                                           | 使用 Keras 快速入门 Gemma 2 预训练 9B 模型的教程                                                                                                                           |
| [Keras_Gemma_2_Quickstart_Chat.ipynb](Gemma/Keras_Gemma_2_Quickstart_Chat.ipynb)                                                                 |  使用 Keras 指令调优 Gemma 2 9B模型的快速入门教程，参考了这篇[博客](https://developers.googleblog.com/en/fine-tuning-gemma-2-with-keras-hugging-face-update/)。|
| [Chat_and_distributed_pirate_tuning.ipynb](Gemma/Chat_and_distributed_pirate_tuning.ipynb)                                                       | 与 Gemma 7B 聊天，并微调Gemma 7B，使其能以海盗口吻生成回答。                                                                                            |
| [gemma_inference_on_tpu.ipynb](Gemma/gemma_inference_on_tpu.ipynb)                                                                               | 在 TPU 上使用 JAX/Flax 对 Gemma 进行基础推理。                                                                                                                                      |
| [gemma_data_parallel_inference_in_jax_tpu.ipynb](Gemma/gemma_data_parallel_inference_in_jax_tpu.ipynb)                                           | 在 TPU 上使用 JAX/Flax 对 Gemma 进行并行推理。                                                                                                                                |
| [Gemma_control_vectors.ipynb](Gemma/Gemma_control_vectors.ipynb)                                                                                 | 在 I/O 2024 的[Keras talk](https://www.youtube.com/watch?v=TV7qCk1dBWA) 中，使用 Gemma 实现控制向量[control vectors](https://arxiv.org/abs/2310.01405)的示例。                                 |
| [Self_extend_Gemma.ipynb](Gemma/Self_extend_Gemma.ipynb)                                                                                         |  在 I/O 2024 的[Keras talk](https://www.youtube.com/watch?v=TV7qCk1dBWA) 中，为 Gemma 扩展自我上下文窗口的示例。                                                                       |
| [Gemma_Basics_with_HF.ipynb](Gemma/Gemma_Basics_with_HF.ipynb)                                                                                   | 使用 Hugging Face 加载、运行、微调并部署 Gemma。                                                                                                    |
| [Guess_the_word.ipynb](Gemma/Guess_the_word.ipynb)                                                                                               | 使用 Keras 与 Gemma 玩猜单词游戏。                                                                                                                                   |
| [Game_Design_Brainstorming.ipynb](Gemma/Game_Design_Brainstorming.ipynb)                                                                         | 使用 Keras 和 Gemma 在游戏设计中进行创意头脑风暴。                                                                                                                          |
| [Translator_of_Old_Korean_Literature.ipynb](Gemma/Translator_of_Old_Korean_Literature.ipynb)                                                     | KerasUse Gemma to translate old Korean literature using Keras.    使用 Keras 和 Gemma 翻译古韩语文学作品。Gemma                                                                                                                           |
| [Gemma2_on_Groq.ipynb](Gemma/Gemma2_on_Groq.ipynb)                                                                                               | 利用托管在[Groq](https://groq.com/)上的免费Gemma 2 9B IT模型（速度超快）。                                                                                           |
| [Prompt_chaining.ipynb](Gemma/Prompt_chaining.ipynb)                                                                                             | 展示在使用Gemma时如何使用提示链和迭代生成技术                                                                                                                |
| [Advanced_Prompting_Techniques.ipynb](Gemma/Advanced_Prompting_Techniques.ipynb)                                                                 | 展示在使用Gemma时如何使用提示链和迭代生成技术                                                                                                                             |
| [Run_with_Ollama.ipynb](Gemma/Run_with_Ollama.ipynb)                                                                                             | 使用 [Ollama](https://www.ollama.com/) 运行 Gemma 模型。                                                                                                                            |
| [Aligning_DPO_Gemma_2b_it.ipynb](Gemma/Aligning_DPO_Gemma_2b_it.ipynb)                                                                           | 展示如何使用 [Hugging Face TRL](https://huggingface.co/docs/trl/en/index) 中的直接偏好优化（DPO,Direct Preference Optimization）来校准 Gemma 模型。                                   |
| [Deploy_with_vLLM.ipynb](Gemma/Deploy_with_vLLM.ipynb)                                                                                           |  使用 [vLLM](https://github.com/vllm-project/vllm) 部署 Gemma 模型。                                                                                                              |
| [Deploy_Gemma_in_Vertex_AI.ipynb](Gemma/Deploy_Gemma_in_Vertex_AI.ipynb)                                                                         | 使用 [Vertex AI](https://cloud.google.com/vertex-ai) 部署 Gemma 模型。                                                                                                            |
| [RAG_with_ChromaDB.ipynb](Gemma/RAG_with_ChromaDB.ipynb)                                                                                         |  使用 [ChromaDB](https://www.trychroma.com/) 和 [Hugging Face](https://huggingface.co/) 与 Gemma 构建一个检索增强生成（RAG）系统。                               |
| [Minimal_RAG.ipynb](Gemma/Minimal_RAG.ipynb)                                                                                                     |  使用 [Google UniSim](https://github.com/google/unisim) 和 [Hugging Face](https://huggingface.co/) 与 Gemma 构建一个简单的检索增强生成（RAG）系统示例。                               |
| [RAG_PDF_Search_in_multiple_documents_on_Colab.ipynb](Gemma/RAG_PDF_Search_in_multiple_documents_on_Colab.ipynb)                                 | 在 Google Colab 上使用 Gemma 2 2B 对多个文档进行 RAG PDF 搜索。                                                                                                                 |
| [Using_Gemma_with_LangChain.ipynb](Gemma/Using_Gemma_with_LangChain.ipynb)                                                                       | 展示使用 [LangChain](https://www.langchain.com/) 与 Gemma 的示例。                                                                                                     |
| [Gemma_RAG_LlamaIndex.ipynb](Gemma/Gemma_RAG_LlamaIndex.ipynb)                                                                                   | 一个使用 Gemma 和 [LlamaIndex](https://www.llamaindex.ai/) 的 RAG 示例。                                                                                                                 |
| [Integrate_with_Mesop.ipynb](Gemma/Integrate_with_Mesop.ipynb)                                                                                   | 将 Gemma 与 [Google Mesop](https://google.github.io/mesop/) 集成                                                                                                                 |
| [Integrate_with_OneTwo.ipynb](Gemma/Integrate_with_OneTwo.ipynb)                                                                                 | 将 Gemma 与 [Google OneTwo](https://github.com/google-deepmind/onetwo) 集成。                                                                                                      |
| [Finetune_with_Axolotl.ipynb](Gemma/Finetune_with_Axolotl.ipynb)                                                                                 | 使用 [Axolotl](https://github.com/OpenAccess-AI-Collective/axolotl) 对 Gemma 进行微调。                                                                                                   |
| [Finetune_with_XTuner.ipynb](Gemma/Finetune_with_XTuner.ipynb)                                                                                   | 使用 [XTuner](https://github.com/InternLM/xtuner) 对 Gemma 进行微调。 |
| [Finetune_with_LLaMA_Factory.ipynb](Gemma/Finetune_with_LLaMA_Factory.ipynb)                                                                     | 使用 [LLaMA-Factory](https://github.com/hiyouga/LLaMA-Factory) 对 Gemma 进行微调。                                                                                                       |
| [Gemma on Android](Gemma/Gemma-on-Android)                                                                     | 一个使用 MediaPipe LLM 推理 API 部署经过微调的 Gemma-2B-it 模型的 Android 应用程序。                                                                                                       |
| **PaliGemma**                                                                                                                                    |
| [Image_captioning_using_PaliGemma.ipynb](PaliGemma/Image_captioning_using_PaliGemma.ipynb)                                                       | 使用 Keras 利用 PaliGemma 生成图像标题。                                                                                                                                  |
| [Image_captioning_using_finetuned_PaliGemma.ipynb](PaliGemma/Image_captioning_using_finetuned_PaliGemma.ipynb)                                   | 使用 [Hugging Face](https://huggingface.co/) 比较不同版本的 PaliGemma 在图像标题生成上的结果。                                                                 |
| [Finetune_PaliGemma_for_image_description.ipynb](PaliGemma/Finetune_PaliGemma_for_image_description.ipynb)                                       | 使用 [JAX](https://github.com/google/jax) 对 PaliGemma 进行图像描述的微调。                                                                                                   |
| [Integrate_PaliGemma_with_Mesop.ipynb](PaliGemma/Integrate_PaliGemma_with_Mesop.ipynb)                                                           | 将 PaliGemma 与 [Google Mesop](https://google.github.io/mesop/) 集成。                                                                                                             |
| [Zero_shot_object_detection_in_images_using_PaliGemma.ipynb](PaliGemma/Zero_shot_object_detection_in_images_using_PaliGemma.ipynb)               | 使用 PaliGemma 在图像中进行零样本目标检测。                                                                                                                                   |
| [Zero_shot_object_detection_in_videos_using_PaliGemma.ipynb](PaliGemma/Zero_shot_object_detection_in_videos_using_PaliGemma.ipynb)               | 使用 PaliGemma 在视频中进行零样本目标检测。                                                                                                                                   |
| [Referring_expression_segmentation_in_images_using_PaliGemma.ipynb](PaliGemma/Referring_expression_segmentation_in_images_using_PaliGemma.ipynb) | 使用 PaliGemma 在图像中进行指示表达分割（Referring Expression Segmentation）。                                                                                                                            |
| [Referring_expression_segmentation_in_videos_using_PaliGemma.ipynb](PaliGemma/Referring_expression_segmentation_in_videos_using_PaliGemma.ipynb) | 使用 PaliGemma 在视频中进行指示表达分割（Referring Expression Segmentation）。                                                                                                                           |

## 获取帮助
在新的[Build with Google AI Forum](https://discuss.ai.google.dev/) 论坛上提问与 Gemma Cookbook 相关的问题，或在 GitHub 上开启一个[issue](https://github.com/google-gemini/gemma-cookbook/issues)。

## 心愿单
如果您希望在 Gemma Cookbook 中实现特定功能/集成，请通过在[心愿单](https://github.com/google-gemini/gemma-cookbook/blob/main/WISHLIST.md)中添加您的功能请求来向我们发送拉取请求。

如果您想对 Gemma Cookbook 项目做出贡献，欢迎选择[心愿单](https://github.com/google-gemini/gemma-cookbook/blob/main/WISHLIST.md)中的任何一个想法并实现它。

## 贡献
我们随时欢迎贡献。请在实施之前阅读[贡献指南](https://github.com/google-gemini/gemma-cookbook/blob/main/CONTRIBUTING.md)。

感谢您与 Gemma 一起开发！我们很期待看到您创造的作品。

## 原始仓库的其他翻译版本
* [繁体中文](https://github.com/doggy8088/gemma-cookbook?tab=readme-ov-file)
