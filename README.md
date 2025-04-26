# data_science_dashboard
dynamic data science dashboard with Taipy Scenarios

## Requirements
- `taipy >= 4.0.0` (previous versions do no have `tp.Orchestrator()` but use `tp.Core()` instead)
- `plotly == 5.24.1`
- `tensorflow == 2.18.0`
- `scikit-learn == 1.5.2`

### Recommended Environment Setup - No GPU
```
>> conda create -n your_name python=3.11
>> conda activate your_name
>> pip install taipy
>> pip install plotly
>> pip install tensorflow
>> pip install scikit-learn
```

### Recommended Environment Setup - with GPU
This enviropnment will result in obtaining predictions faster. How faster depends on your CPU and GPU model.
<br>
On my end, it results in approx. 20% speed up from switching to RTX 4080 GPU over 12th Gen Intel i9-12900k CPU.
<br>
<br>
*Please replace the first command with one that <b>matches your system requirements and CUDA version</b> from <a href="https://docs.rapids.ai/install/" target="_blank">the official RAPIDS installation guide</a>. 
```
>> conda create -n your_name -c rapidsai -c conda-forge -c nvidia cudf=24.10 python=3.12 'cuda-version>=12.0,<=12.5'
>> conda activate your_name
>> pip install taipy
>> pip install plotly
>> pip install tensorflow
>> pip install scikit-learn
```

## Dataset
S&P 500 Stocks (daily updated) by Larxel
<br>
https://www.kaggle.com/datasets/andrewmvd/sp-500-stocks

## Further Learning
Please checkout Taipy's <a href="https://links.taipy.io/Mariya" target="_blank">Official Github Repo</a> for more details and contribution guidelines.