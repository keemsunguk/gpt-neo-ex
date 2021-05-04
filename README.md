# GPT-NEO in FreeWheel

## GPT Neo

### Model Description
GPT-Neo 1.3B is a transformer model designed using EleutherAI's replication of the GPT-3 architecture. GPT-Neo refers to the class of models, while 1.3B represents the number of parameters of this particular pre-trained model.

### Training data
GPT-Neo 1.3B was trained on the Pile, a large scale curated dataset created by EleutherAI for the purpose of training this model.

[Project Landing Page](https://huggingface.co/EleutherAI)

## Models
* [1.3B](https://huggingface.co/EleutherAI/gpt-neo-1.3B)
* [2.7B](https://huggingface.co/EleutherAI/gpt-neo-2.7B)


## Installation

1. Clone [this](https://github.com/keemsunguk/gpt-neo-ex.git) repo
```buildoutcfg
git clone https://github.com/keemsunguk/gpt-neo-ex.git
```
2. Create the environment
   (Just copy and paste the commands from the code block.)
   1. "nlp_env" is a name that I used.  Feel free to use your own env name
   1. In the requirements, the latest transformer was installed from 
      its [repo](git+https://github.com/huggingface/transformers), not from Pypi.
   Transformer from Pypi will not recognize gpt-neo, at least for now.
   1. Transformer requires torch package (pytorch, already in the requirements.txt)
   1. To run with Jupyter, ipywidgets is required
   1. I put everything in the requirements.txt
```buildoutcfg
cd gpt-neo-ex
python3 -m venv nlp_env
source nlp_env/bin/activate
pip install -r requirements.txt
```
3. Set up a kernel
```buildoutcfg
python -m ipykernel install --user --name nlp_env --display-name nlp_env
```

4. Run this example [notebook](https://github.com/keemsunguk/gpt-neo-ex.git/blob/master/notebooks/gpt-neo-try1.ipynb)
    * GPT-Neo was trained on the Pile, a dataset known to contain profanity, lewd, and otherwise abrasive language. Depending on your usecase GPT-Neo may produce socially unacceptable text.
