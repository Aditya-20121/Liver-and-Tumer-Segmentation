# A Multi-Scale Attention Network for Liver and Tumor Segmentation


We have implemented the research paper  [MA-Net: A Multi-Scale Attention Network for Liver and Tumor Segmentation
](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9201310).


## Datasets

We use the **MICCAI 2017 Liver Tumor Segmentation (LiTS) challenge** dataset  which is available below:


 Liver tumor Segmentation Challenge (LiTS) contain 131 contrast-enhanced CT images provided by hospital around the world. For more detail about the dataset, you can check this link: [LiTs17](https://competitions.codalab.org/competitions/17094 )  dataset


 
 
## Overview of the model
![ov](https://ieeexplore.ieee.org/mediastore_new/IEEE/content/media/6287639/8948470/9201310/wang1-3025372-large.gif)

This reasearch paper proposes a novel network named Multi-scale Attention Net (MA-Net) by introducing self-attention mechanism into their method to adaptively integrate local features with their global dependencies

## Code Execution


#### Update file path in `Resnet50.ipynb, resnet34.ipynb and manet.ipynb `

Update the file path of dataset present in the **file_lists** class .ipynb files

```
file_list = []
for dirname, _, filenames in os.walk('E:/iacv_data'):
    for filename in filenames:
        file_list.append((dirname, filename)) 

for dirname, _, filenames in os.walk('E:/iacv_volume'):
    for filename in filenames:
        file_list.append((dirname, filename)) 

df_files = pd.DataFrame(file_list, columns =['dirname', 'filename']) 
df_files.sort_values(by=['filename'], ascending=True)  
```



## Software language used
* Python


## Packages used
* numpy
* pandas
* matplotlib
* sklearn
* tensorflow
* keras

## References
T. Fan, G. Wang, Y. Li, and H. Wang, "MA-Net: A Multi-Scale Attention Network for Liver and Tumor Segmentation," IEEE Access, vol. 8, pp. 155732-155743, 2020.

