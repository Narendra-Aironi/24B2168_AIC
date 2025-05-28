# 24B2168_AIC
Submission for IIT Bombay's AI community assignment 2025

---
## Setup instructions
* Setup instructions for each technical question is given at the beginning of the corresponding `.ipynb` file.
* Since the Fashion-MNIST dataset is quite large, I have not included it in the T_Q2 folder. You can download it from https://drive.google.com/drive/folders/1qZNwYOW53GZYZjpmsSpZMBNh1PEQumnb. Create a folder under T_Q2 named Fashion-MNIST and add all the downloaded files to it. This is needed only if you want to run the notebook yourself.
* I am using a M3 Macbook Pro. GPU acceleration is done using MPS framework for Apple Silicon chips. For CUDA systems, use CTRL + F and replace all instances of `"mps"` with `"cuda"`.
* In T_Q3, you will need to enter your google API key to run the code successfully.

> Documentation of analysis, experiments and final comments are scattered through the jupyter notebooks. They illustrate how certain hyper-parameters were chosen, reasoning behind the specific model chosen, interpretation of validation metrics etc.

---
## Error Handling and troubleshooting
* In case of error, first ensure the latest version of Python (at least >3.10), and its libraries. Preferably, use a virtual environment to avoid version mismatch.
* Next fix is to see if all mps instances are replaced with cuda. Case-specific instructions may also be present in the markdown of `ipynb` files. Do read it carefully.
* MPS doesn't support certain functions and arguments in PyTorch yet. When porting to CUDA, you can enable those arguments to speed up training. Eg. in BERT training, `fp16=True`, `use_mps_device=False` etc.
* Ensure your API key is properly configured in your Google AI studio. It is used in T_Q3. Free LLM models are only used, having high rate limits, so API problems should be rare.

---
## References

I haven't used AI or Copilot for writing **any** technical code. I used it only sparingly to plot validation metrics like confusion matrix and graphs. 
For debugging, I have used multiple forums like StackOverflow, Reddit and respective forums of PyTorch, HuggingFace, Gemini and LlamaIndex. However, I don't have references to those threads.
I have referred extensively, and majorly to the documentations/github repos of the libraries I used. I haven't included links to those either. 
Finally, I referred briefly to the research paper on transformers "Attention is all you need" and the paper that introduced BERT.

### T_Q1
https://huggingface.co/blog/bert-101
https://medium.com/huggingface/distilbert-8cf3380435b5
https://medium.com/@heyamit10/fine-tuning-bert-for-classification-a-practical-guide-b8c1c56f252c
https://www.kaggle.com/code/deekoul/custom-dataset-dataloader-to-load-bert-tokenizer

### T_Q2
https://colab.research.google.com/github/kjamithash/Pytorch_DeepLearning_Experiments/blob/master/FashionMNIST_ResNet_TransferLearning.ipynb
https://www.learnpytorch.io/06_pytorch_transfer_learning/
https://www.kaggle.com/code/girishgupta/fashion-mnist-using-resnet

### T_Q3
https://medium.com/@roya90/building-a-pdf-question-answering-system-with-retrieval-augmented-generation-rag-in-python-1f14770efdb9
https://karpathy.github.io/2019/04/25/recipe/
https://docs.llamaindex.ai/en/stable/examples/low_level/oss_ingestion_retrieval/
https://medium.com/@anuragmishra_27746/five-levels-of-chunking-strategies-in-rag-notes-from-gregs-video-7b735895694d
https://www.modular.com/ai-resources/scaling-llm-inference-leveraging-kv-caches-for-faster-response-times#:~:text=Key%2DValue%20caching%20is%20a,optimizes%20the%20overall%20inference%20workflow.
https://medium.com/biased-algorithms/gradient-accumulation-in-pytorch-36962825fa44
