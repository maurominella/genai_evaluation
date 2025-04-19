# genai_evaluation README
Evaluation of generative AI applications

## Conda Environment Installation
```
conda create -n genai_evaluation python=3.12 -y
conda activate genai_evaluation
pip install -r ./common/environment.yml -y
jupyter kernelspec uninstall genai_evaluation -y
python -m ipykernel install --user --name=genai_evaluation --display-name "Generative AI evaluation"
jupyter notebook
```
