The implementation of fine tuning Gemma-2 model on image captioning datasets. The implementation is based on LLaVA papers (https://arxiv.org/abs/2304.08485) that project image representation into token for LLMs. In the demo we uses CLIP (https://arxiv.org/abs/2103.00020) to obtain the image representations, and project it using simple MLP model into the same size of LLM token embeddings. We then train the model using FLICKR-8k dataset. We train the model to perform captioning, but it show generalization to other tasks after trained on captioning task. Some example of this generalization is that the model able to create a poem based on an image. However, as the dataset and computation resourcce is very limited, the results still have lot of limitations.
