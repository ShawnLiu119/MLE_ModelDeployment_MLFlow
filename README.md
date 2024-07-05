# MLE_ModelDeployment_MLFlow
deploy ML model on local using MLFlow 

tool - VS code

1. install MLflow in terminal <br>
![image](https://github.com/ShawnLiu119/MLE_ModelDeployment_MLFlow/assets/43327902/eee55a78-f386-4a72-8d5b-30432cfe1c79)

2. run mlflow to check whether it installed correctly <br>
came across error as below: <br>
![image](https://github.com/ShawnLiu119/MLE_ModelDeployment_MLFlow/assets/43327902/410cffd3-68b7-4cdf-a738-5f777c2a16d8)
solution<br>
run the command below<br>
![image](https://github.com/ShawnLiu119/MLE_ModelDeployment_MLFlow/assets/43327902/9eec7258-6675-4c17-8987-0e077e391385)


3. open up 2nd termnial and set up ML flow server<br>
![image](https://github.com/ShawnLiu119/MLE_ModelDeployment_MLFlow/assets/43327902/e217426f-6d96-4878-b2cc-18e72a7d4dd1)
the server listen on localhost:5000 by defualt, so when you open a browser an type in localhost:5000, it will show MLflow interface
it will create the store-folder in the vs code existing directory<br>
![image](https://github.com/ShawnLiu119/MLE_ModelDeployment_MLFlow/assets/43327902/3ff346a1-408b-4991-8de9-219d5b53130d)


4. clone the mlflow github repo <br>
![image](https://github.com/ShawnLiu119/MLE_ModelDeployment_MLFlow/assets/43327902/0bc0480f-8eef-41c4-a001-03fb07640167)

5. change the directory to one of example projects under mlflow imported
![image](https://github.com/ShawnLiu119/MLE_ModelDeployment_MLFlow/assets/43327902/ee5177f2-9adc-4334-8b26-d2994aef3115)

6. output the system variable and point to local host (let the system know that the output from model experiment is export to local<br>
in Windows use "set", whille Unix use "Export"<br>
![image](https://github.com/ShawnLiu119/MLE_ModelDeployment_MLFlow/assets/43327902/26344549-f551-4fc2-a986-183ad5ffd497)

7. prepare the files for deployment
   - MLproject(yaml file):defines all scripts ML project need to run <br>
     ![image](https://github.com/ShawnLiu119/MLE_ModelDeployment_MLFlow/assets/43327902/ad5041c5-2654-4760-9ef0-77a96389ad6c)
   - python_env.yaml: you can also define docker image here, if you need a specific environment to ensure reproducibility <br>
     ![image](https://github.com/ShawnLiu119/MLE_ModelDeployment_MLFlow/assets/43327902/e62dd61f-65ae-4cff-8d97-e14fb78fb5b7)
   - train.py <br>
     ![image](https://github.com/ShawnLiu119/MLE_ModelDeployment_MLFlow/assets/43327902/dcc2269a-1256-4014-bc66-9afe82b15448)
     this is the production-level code that you need to compile from Jupyter level code into all function-based code; <br>
     infer-signature：create signature for the model. The Model Signature in MLflow is integral to the clear and accurate operation of models. It defines the expected format for model inputs and outputs, including any additional parameters needed for inference. This 
     specification acts as a definitive guide, ensuring seamless model integration with MLflow’s tools and external services <br>
     log mdoel, and log the score

8. run mlflow experienment in terminal
   ![image](https://github.com/ShawnLiu119/MLE_ModelDeployment_MLFlow/assets/43327902/2eba48e1-cc72-4661-ab1c-3a82826e1497)
   error occurs <br>
   ![image](https://github.com/ShawnLiu119/MLE_ModelDeployment_MLFlow/assets/43327902/01c31667-54aa-42a7-954a-78be79ef8c1c)
   solution <br>
   



