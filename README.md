# Optical Character Recognition for Receipt

## Sample Results
Input Image             |  Output
:----------------------:|:----------------------:
<img src="./data/tes.jpg" width="300" title="sample-input">  |  <img src="./data/sample_output.jpg" width="300" title="sample-output">

## Requirements

```
pip install -r requirements.txt
```
or
```
conda env create -f environment.yaml
```

## Container
```
docker build -t receipt-ocr .
docker run -d --name receipt-ocr-service -p 80:80 receipt-ocr
docker start receipt-ocr-service
docker stop receipt-ocr-service
```