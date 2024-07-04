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



