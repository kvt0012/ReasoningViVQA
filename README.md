# ReasoningViVQA: A Comprehensive Dataset and Multimodal Reasoning Framework for Enhancing Real-World Visual Reasoning in Low-Resource Vietnamese

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) 	![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)

- This repository is a implementation of the framework PhoViT for a Vietnamese visual question answering.

- In this work, we are also releasing a dataset for visual reasoning. The dataset is provided in folder [data/ViCLEVR](hhttps://github.com/kvt0012/ViCLEVR/tree/main/data/ViCLEVR) in this repository. More details about dataset are provided below.

# News

- Sep 2023: Finish paper

<!-- <!-- *Paper*: []() -->
#### Citation 
```
@Article{Tran2024ReasoningViVQA,
  title= {ReasoningViVQA: A Comprehensive Dataset and Multimodal Reasoning Framework for Enhancing Real-World Visual Reasoning in Low-Resource Vietnamese},
  author= {Khiem Vinh Tran, Hao Phu Phan, Kiet Van Nguyen,Ngan Luu Thuy Nguyen},
  journal= {},
  number= {},
	pages= {},
  doi= {},
  year={2024}
}
```

# Framework

## Dataset format

<!-- ```json
{
  "id":"6",
  "question":[ {
         "language":"en",
         "string":"Where is the first case in Vietnam?  ",
         "keywords":"first case, COVID-19, Vietnam "
      }, {
         "language":"vi",
         "string":"Truong hop ca nhiem COVID-19 dau tien cua Viet Nam la o dau?",
         "keywords":"Ca nhiem dau tien, COVID-19, Viet Nam"
      }],
  "query":{
      "sparql":"SELECT DISTINCT ?uri WHERE { <http://dbpedia.org/resource/COVID-19_pandemic_in_Vietnam> <http://dbpedia.org/property/firstCase> ?uri }"
  },
  "answers":[{"head":{"vars":["uri"]},
         "results":{"bindings":[{"uri":{
                     "type":"uri",
                     "value":"http://dbpedia.org/resource/Ho_Chi_Minh_City"
                  }}]}}
  ]
}
``` -->

## Enviroment
` pip install -r requirement.txt` 
## Preprocess data


`python main.py --inp in/ --output out/ `

`--data` : Data input configuration

`--output` : Data output

##  Usage

`python main.py --data --output`
- ```Training:``` python main.py 

- ```Validate:``` python main.py --task validate

- ```Test:``` python main.py --task test

## Support 
Please raise potential bugs on github. If you have a research related question, please send it to this email(vinhkhiemt135@gmail.com)


