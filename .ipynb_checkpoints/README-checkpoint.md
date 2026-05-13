# Mauro Minella repository for storing samples about<br/>
# `Evaluation of generative AI applications`

## Environment preparation
Evaluation of generative AI applications

### 1. Install Git from its [WEB site](https://git-scm.com/downloads), choosing your operating system

### 2. Open a git/bash command prompt, or make sure that git executable is in the path

### 3. ***CD*** into the base folder for your git repositories
If you do not have one, you may create a folder called `git_repos`

### 4. Use `git` to clone this repo locally
```git clone https://github.com/maurominella/genai_evaluation.git```

### 5. Create a sub-folder of the base `git_repos` called `config` if it does not exist yet
**Before** moving into this folder, just copy the file `credentials_my(template).env` of the cloned repo into it:<br/>
- ```cp "./genai_evaluation/credentials_my(template).env" ./config```

The file `./config/credentials_my.env` -without the final `(template)` in the name- will have to be updated with your own credentials in order to be shared among all repositories.

### 6. ***CD*** into `genai_evaluation` folder of the cloned repository
```cd genai_evaluation```

### 7. Install Miniconda from its [WEB site](https://www.anaconda.com/docs/getting-started/miniconda/install), choosing your operating system

### 8. Open Miniconda bash / prompt, or make sure that conda executable is in the path

### 9. Environment provisioning for Azure AI Agent Service (`genai_evaluation`)

#### 9.1 Remove the pre-existing conda `genai_evaluation_conda` environment (if exists)
```conda env remove -n genai_evaluation_conda -y```

#### 9.2 Create new Conda Environment `genai_evaluation_conda` with Python 3.11
```conda create -n genai_evaluation_conda python=3.11 -y```

#### 9.3 Activate the `genai_evaluation_conda` environment
```conda activate genai_evaluation_conda```

#### 9.4 Install libraries and dependencies
```pip install -r ./common/requirements.txt```

#### 9.5 Remove `genai_evaluation_conda` kernel (if exists)
```jupyter kernelspec uninstall genai_evaluation_conda -y```

#### 9.6 Create `genai_evaluation_conda` kernel 
```python -m ipykernel install --name genai_evaluation_conda --user```

#### 9.7 Check kernels list to make sure that `genai_evaluation_conda` exists
```jupyter kernelspec list```



enjoy ;-)
