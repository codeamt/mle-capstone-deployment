# Fast Efficient Covidnet
Streamlit inference service deployment submodule for Udacity's Machine Learning Engineer Nanodegree program.


 
<p align="center">
<img src="https://drive.google.com/uc?export=view&id=1P1g6zNLvHTgCF6E1jnoJ6lqWIHBoCeUI" width="60%" />
</p>

**DISCLAIMER:** THIS TOOL SHOULD NOT BE USED FOR MEDICAL DIAGNOSIS/REPLACE CONSULTING FROM A MEDICAL EXPERT AND SHOULD SERVE EDUCATIONAL PURPOSES ONLY.

## Related Repos/Files: 
- [All repos](https://github.com/codeamt/FastEfficientCovidNet)
- [Data Engineering](https://github.com/codeamt/mle-capstone-data)
- [Model Training](https://github.com/codeamt/mle-capstone-modeling)
- [Technical Report](https://github.com/codeamt/FastEfficientCovidNet/blob/master/report.pdf)

## About 
This is a Chest X-Ray (CXR) classification API. Building on previous work of [[1]](https://arxiv.org/pdf/2003.09871v3.pdf), the CovNet model for this ML project utilizes a pre-trained EfficientNet-b1 to extract features and a fine-tuned Fast.ai classifier to differentiate between infection classes (Normal, Viral Pneumonia, or COVID-19) with 95% test accuracy. 
 
## Build Instructions

### Locally

#### Clone this repo:
```
git clone https://github.com/codeamt/mle-capstone-deployment FastEfficientCovidnet 
cd FastEfficientCovidnet

```

#### Install packages:
```
cd src
pip3 -r install requirements.txt 
```

### or Dockerized:

```
docker build -f Dockerfile -t app:latest .
```

## Running 

### Locally:
From the src of the repo:
```
streamlit run app.py
```
### with Docker: 

```
docker run -p 8501:8501 app:latest
```
