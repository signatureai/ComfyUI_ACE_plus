<p align="center">

  <h2 align="center"><img src="assets/figures/icon.png" height=16> ++: Instruction-Based Image Creation and Editing <br> via Context-Aware Content Filling </h2>

  <p align="center">
    <a href="https://arxiv.org/abs/2501.02487"><img src='https://img.shields.io/badge/arXiv-ACE++-red' alt='Paper PDF'></a>
    <a href='https://ali-vilab.github.io/ACE_plus_page/'><img src='https://img.shields.io/badge/Project_Page-ACE++-blue' alt='Project Page'></a>
    <a href='https://github.com/modelscope/scepter'><img src='https://img.shields.io/badge/Scepter-ACE++-green'></a>
    <a href='https://huggingface.co/spaces/scepter-studio/ACE-Plus'><img src='https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Space-orange'></a>
    <a href='https://huggingface.co/ali-vilab/ACE_Plus/tree/main'><img src='https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Model-orange'></a>
    <a href='https://modelscope.cn/models/iic/ACE_Plus/summary'><img src='https://img.shields.io/badge/ModelScope-Model-purple'></a>
    <br>
    <strong>Chaojie Mao</strong>
    ·
    <strong>Jingfeng Zhang</strong>
    ·
    <strong>Yulin Pan</strong>
    ·
    <strong>Zeyinzi Jiang</strong>
    ·
    <strong>Zhen Han</strong>
    <br>
    ·
    <strong>Yu Liu</strong>
    ·
    <strong>Jingren Zhou</strong>
    <br>
    Tongyi Lab, Alibaba Group
  </p>
  <table align="center">
    <tr>
    <td>
      <img src="assets/ace_method/method++.png">
    </td>
    </tr>
  </table>

## 📢 News
- [x] **[2025.01.06]** Release the code and models of ACE++.
- [] **[ToDo]** Release the demo on HuggingFace.
- [] **[ToDo]** Update Models.

##  🔥 ACE Models
ACE++ provides a comprehensive toolkit for image editing and generation to support various applications. We encourage developers to choose the appropriate model based on their own scenarios and to fine-tune their models using data from their specific scenarios to achieve more stable results.  




### ACE++ Portrait
Portrait-consistent generation to maintain the consistency of the portrait.

<table><tbody>
  <tr>
    <td>Tuning Method</td>
    <td>Input</td>
    <td>Output</td>
    <td>Instruction</td>
    <td>Models</td>
  </tr>
  <tr>
    <td>LoRA <br>+ ACE Data</td>
    <td><img src="./assets/samples/portrait/human_1.jpg" width="200"></td>
    <td><img src="./assets/samples/portrait/human_1_1.jpg" width="200"></td>
    <td style="word-wrap:break-word;word-break:break-all;" width="250px";>"Maintain the facial features. A girl is wearing a neat police uniform and sporting a badge. She is smiling with a friendly and confident demeanor. The background is blurred, featuring a cartoon logo."</td>
    <td align="center" style="word-wrap:break-word;word-break:break-all;" width="200px";><a href="https://www.modelscope.cn/models/iic/ACE_Plus/"><img src="https://img.shields.io/badge/ModelScope-Model-blue" alt="ModelScope link"> </a> <a href="https://huggingface.co/ali-vilab/ACE_Plus/tree/main/portrait/"><img src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Model-yellow" alt="HuggingFace link"> </a> </td>
  </tr>
</tbody>
</table>

Models' scepter_path: 
- **ModelScope:** ms://iic/ACE_Plus@portrait/xxxx.safetensors
- **HuggingFace:** hf://ali-vilab/ACE_Plus@portrait/xxxx.safetensors


### ACE++ Subject
Subject-driven image generation task to maintain the consistency of a specific subject in different scenes.
<table><tbody>
  <tr>
    <td>Tuning Method</td>
    <td>Input</td>
    <td>Output</td>
    <td>Instruction</td>
    <td>Models</td>
  </tr>
  <tr>
    <td>LoRA <br>+ ACE Data</td>
    <td><img src="./assets/samples/subject/subject_1.jpg" width="200"></td>
    <td><img src="./assets/samples/subject/subject_1_1.jpg" width="200"></td>
    <td style="word-wrap:break-word;word-break:break-all;" width="250px";>"Display the logo in a minimalist style printed in white on a matte black ceramic coffee mug, alongside a steaming cup of coffee on a cozy cafe table."</td>
    <td align="center" style="word-wrap:break-word;word-break:break-all;" width="200px";><a href="https://www.modelscope.cn/models/iic/ACE_Plus/"><img src="https://img.shields.io/badge/ModelScope-Model-blue" alt="ModelScope link"> </a> <a href="https://huggingface.co/ali-vilab/ACE_Plus/tree/main/subject/"><img src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Model-yellow" alt="HuggingFace link"> </a> </td>
  </tr>
</tbody>
</table>

Models' scepter_path: 
- **ModelScope:** ms://iic/ACE_Plus@subject/xxxx.safetensors
- **HuggingFace:** hf://ali-vilab/ACE_Plus@subject/xxxx.safetensors


### ACE++ LocalEditing
Redrawing the mask area of images while maintaining the original structural information of the edited area.
<table><tbody>
  <tr>
    <td>Tuning Method</td>
    <td>Input</td>
    <td>Output</td>
    <td>Instruction</td>
    <td>Models</td>
  </tr>
  <tr>
    <td>LoRA <br>+ ACE Data</td>
    <td><img src="./assets/samples/local/local_1.webp" width="200"><br><img src="./assets/samples/local/local_1_m.webp" width="200"></td>
    <td><img src="./assets/samples/local/local_1_1.jpg" width="200"></td>
    <td style="word-wrap:break-word;word-break:break-all;" width="250px";>"By referencing the mask, restore a partial image from the doodle {image} that aligns with the textual explanation: "1 white old owl"."</td>
    <td align="center" style="word-wrap:break-word;word-break:break-all;" width="200px";><a href="https://www.modelscope.cn/models/iic/ACE_Plus/"><img src="https://img.shields.io/badge/ModelScope-Model-blue" alt="ModelScope link"> </a> <a href="https://huggingface.co/ali-vilab/ACE_Plus/tree/main/local_editing/"><img src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Model-yellow" alt="HuggingFace link"> </a> </td>
  </tr>
</tbody>
</table>

Models' scepter_path: 
- **ModelScope:** ms://iic/ACE_Plus@local_editing/xxxx.safetensors
- **HuggingFace:** hf://ali-vilab/ACE_Plus@local_editing/xxxx.safetensors

### ACE++ Fully [Coming soon] 
Fully finetuning a composite model with ACE’s data to support various editing and reference generation tasks through an instructive approach.

##  🔥 Applications
The ACE++ model supports a wide range of downstream tasks through simple adaptations. Here are some examples, and we look forward to seeing the community explore even more exciting applications utilizing the ACE++ model.

<table><tbody>
  <tr>
    <th align="center" colspan="1">Application</th>
    <th align="center" colspan="1">ACE++ Model</th>
    <th align="center" colspan="5">Examples</th>
  </tr>
  <tr>
    <td>Try On</td>
    <td>ACE++ Subject</td>
    <td><img src="./assets/samples/application/try_on/1_ref.png" width="200"></td>
    <td><img src="./assets/samples/application/try_on/1_1_edit.png" width="200"></td>
    <td><img src="./assets/samples/application/try_on/1_1_m.png" width="200"></td>
    <td><img src="./assets/samples/application/try_on/1_1_res.png" width="200"></td>
    <td style="word-wrap:break-word;word-break:break-all;" width="100px";>"The woman dresses this skirt."</td>
  </tr>
  <tr>
    <td>Logo Paste</td>
    <td>ACE++ Subject</td>
    <td><img src="./assets/samples/application/logo_paste/1_ref.png" width="200"></td>
    <td><img src="./assets/samples/application/logo_paste/1_1_edit.png" width="200"></td>
    <td><img src="./assets/samples/application/logo_paste/1_1_m.png" width="200"></td>
    <td><img src="./assets/samples/application/logo_paste/1_1_res.webp" width="200"></td>
    <td style="word-wrap:break-word;word-break:break-all;" width="100px";>"The logo is printed on the headphones."</td>
  </tr>
  <tr>
    <td>Photo Editing</td>
    <td>ACE++ Subject</td>
    <td><img src="./assets/samples/application/photo_editing/1_ref.png" width="200"></td>
    <td><img src="./assets/samples/application/photo_editing/1_1_edit.png" width="200"></td>
    <td><img src="./assets/samples/application/photo_editing/1_1_m.png" width="200"></td>
    <td><img src="./assets/samples/application/photo_editing/1_1_res.jpg" width="200"></td>
    <td style="word-wrap:break-word;word-break:break-all;" width="100px";>"The item is put on the ground."</td>
  </tr>
  <tr>
    <td>Movie Poster Editor</td>
    <td>ACE++ Portrait</td>
    <td><img src="./assets/samples/application/movie_poster/1_ref.png" width="200"></td>
    <td><img src="./assets/samples/application/movie_poster/1_1_edit.png" width="200"></td>
    <td><img src="./assets/samples/application/movie_poster/1_1_m.png" width="200"></td>
    <td><img src="./assets/samples/application/movie_poster/1_1_res.webp" width="200"></td>
    <td style="word-wrap:break-word;word-break:break-all;" width="100px";>"The man is facing the camera and is smiling."</td>
  </tr>
</tbody>
</table>

## ⚙️️ Installation
Download the code using the following command:
```bash
git clone https://github.com/ali-vilab/ACE_plus.git
```

Install the necessary packages with `pip`: 
```bash
cd ACE_plus
pip install -r requirements.txt
```
ACE++ depends on FLUX.1-Fill-dev as its base model, which you can download from [![HuggingFace link](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Model-yellow)](https://huggingface.co/black-forest-labs/FLUX.1-Fill-dev). 
In order to run the inference code or Gradio demo normally, we have defined the relevant environment variables to specify the location of the model. 
For model preparation, we provide three methods for downloading the model. The summary of relevant settings is as follows.

|   Model Downloading Method    | Clone to Local Path                                                                                                                                                                                                                                         | Automatic Downloading during Runtime<br>(Setting the Environment Variables using scepter_path in [ACE Models](#-ace-models))                                                                                                       |
|:-----------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Environment Variables Setting | <pre><code>export FLUX_FILL_PATH="path/to/FLUX.1-Fill-dev"<br>export PORTRAIT_MODEL_PATH="path/to/ACE++ PORTRAIT PATH"<br>export SUBJECT_MODEL_PATH="path/to/ACE++ SUBJECT PATH"<br>export LOCAL_MODEL_PATH="path/to/ACE++ LOCAL EDITING PATH"</code></pre> | <pre><code>export FLUX_FILL_PATH="hf://black-forest-labs/FLUX.1-Fill-dev"<br>export PORTRAIT_MODEL_PATH="${scepter_path}"<br>export SUBJECT_MODEL_PATH="${scepter_path}"<br>export LOCAL_MODEL_PATH="${scepter_path}"</code></pre> |

## 🚀 Inference
Under the condition that the environment variables defined in [Installation](#-installation), users can run examples and test your own samples by executing infer.py. 
The relevant commands are as follows:
```bash
export FLUX_FILL_PATH="hf://black-forest-labs/FLUX.1-Fill-dev"
export PORTRAIT_MODEL_PATH="ms://iic/ACE_Plus@portrait/comfyui_portrait_lora64.safetensors"                                                                                                                                      
export SUBJECT_MODEL_PATH="ms://iic/ACE_Plus@subject/comfyui_subject_lora16.safetensors"                                                                                                                                         
export LOCAL_MODEL_PATH="ms://iic/ACE_Plus@local_editing/comfyui_local_lora16.safetensors" 
# Use the model from huggingface
# export PORTRAIT_MODEL_PATH="hf://ali-vilab/ACE_Plus@portrait/comfyui_portrait_lora64.safetensors"        
# export SUBJECT_MODEL_PATH="hf://ali-vilab/ACE_Plus@subject/comfyui_subject_lora16.safetensors"        
# export LOCAL_MODEL_PATH="hf://ali-vilab/ACE_Plus@local_editing/comfyui_local_lora16.safetensors" 
python infer.py
```

## 💻 Demo
We have built a GUI demo based on Gradio to help users better utilize the ACE++ model. Just execute the following command.
```bash
export FLUX_FILL_PATH="hf://black-forest-labs/FLUX.1-Fill-dev"
export PORTRAIT_MODEL_PATH="ms://iic/ACE_Plus@portrait/comfyui_portrait_lora64.safetensors"                                                                                                                                      
export SUBJECT_MODEL_PATH="ms://iic/ACE_Plus@subject/comfyui_subject_lora16.safetensors"                                                                                                                                         
export LOCAL_MODEL_PATH="ms://iic/ACE_Plus@local_editing/comfyui_local_lora16.safetensors" 
# Use the model from huggingface
# export PORTRAIT_MODEL_PATH="hf://ali-vilab/ACE_Plus@portrait/comfyui_portrait_lora64.safetensors"        
# export SUBJECT_MODEL_PATH="hf://ali-vilab/ACE_Plus@subject/comfyui_subject_lora16.safetensors"        
# export LOCAL_MODEL_PATH="hf://ali-vilab/ACE_Plus@local_editing/comfyui_local_lora16.safetensors" 
python demo.py
```

## 📚 Limitations
* For certain tasks, such as deleting and adding objects, there are flaws in instruction following. For adding and replacing objects, we recommend trying the repainting method of the local editing model to achieve this.
* The generated results may contain artifacts, especially when it comes to the generation of hands, which still exhibit distortions.
* The current version of ACE++ is still in the development stage. We are working on improving the model's performance and adding more features.

## 📝 Citation
ACE++ is a post-training model based on the FLUX.1-dev series from black-forest-labs. Please adhere to its open-source license. The test materials used in ACE++ come from the internet and are intended for academic research and communication purposes. If the original creators feel uncomfortable, please contact us to have them removed. 

If you use this model in your research, please cite the works of FLUX.1-dev and the following papers:
```bibtex
@article{mao2025ace++,
  title={ACE++: Instruction-Based Image Creation and Editing via Context-Aware Content Filling},
  author={Mao, Chaojie and Zhang, Jingfeng and Pan, Yulin and Jiang, Zeyinzi and Han, Zhen and Liu, Yu and Zhou, Jingren},
  journal={arXiv preprint arXiv:2501.02487},
  year={2025}
}
```
```bibtex
@article{han2024ace,
  title={ACE: All-round Creator and Editor Following Instructions via Diffusion Transformer},
  author={Han, Zhen and Jiang, Zeyinzi and Pan, Yulin and Zhang, Jingfeng and Mao, Chaojie and Xie, Chenwei and Liu, Yu and Zhou, Jingren},
  journal={arXiv preprint arXiv:2410.00086},
  year={2024}
}
```
