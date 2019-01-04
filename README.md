# IDRiD_Challenge_Mask-RCNN

### The Challenge in (https://idrid.grand-challenge.org/)

the the data can be download [here](https://ieee-dataport.org/open-access/indian-diabetic-retinopathy-image-dataset-idrid)

The Mask RCNN's application in IDRiD(only for challenge 1)


#### 原始的数据结构
* Original:

    --traiing
    
       ---IDRiD_01.jpg
       
       ---IDRiD_02.jpg
       ...
       
     --testing
       ---IDRiD_01.jpg
       
       ---IDRiD_02.jpg
       ...
* Groundtruths:

     --training
     
        ---Haemorrhages
          
          IDRiD_01.jpg
          
          IDRiD_02.jpg
          ...
        ---HardExudates
        
        ---Microaneurysms
        
        ---OpticDisc
        
        ---SoftExudates
        
      --testing
        ---Haemorrhages
          
          IDRiD_01.jpg
          
          IDRiD_02.jpg
          ...
        ---HardExudates
        
        ---Microaneurysms
        
        ---OpticDisc
        
        ---SoftExudates
        
        
    
        

*  Step 1 : Create Dataset

First,create directory **data**
```bash
mkdir data
```
And create data
```python
python dataset.py
```
The data will store in data,they are too big,so I do not show that.

*  Step 2: Train the Model
```python 
python main.py
```
the checkpoint will be stored in directory **checkpoint**,you can download the pretrained model in [here](https://github.com/yejg2017/IDRiD_Challenge_Mask-RCNN/releases/download/v1.0/checkpoint.zip)


*  Step 3: [Demo](./demo.ipynb)
Show the Mask and model evaluation


![Diabetes](./example.jpg)
