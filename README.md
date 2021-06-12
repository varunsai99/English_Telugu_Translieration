The wandb report link is: https://wandb.ai/adi00510/Assignment%203%20Question%202/reports/Assignment-3--Vmlldzo2OTk5ODU

1. Question 1
    1. Here we have created a class seq2seq, in this class we have created a function "create_model" which will return a model based on different parameters which are passed to seq2seq class.
    2. We have written our code as per the requirements which is asked in the question
    3. Link for the .ipynb file: https://colab.research.google.com/drive/1PtGYeH0gD-SpFMN5LbgAYTNT-SFWIcnc?usp=sharing
2. Question 2
    1. In this question, we have setup the sweep on the above code.
    2. Here we are adding the parameters like Dropout,Batch size,Epochs,Encoder_layer_size,Decoder_layer_size,Emebdding size, Cell type, and latent dimension size.
    3. Then we have run the sweep in wandb.
    4. Link for the .ipynb file: https://colab.research.google.com/drive/1JsFpoG-7shQIafy-4HU3K4jLadoR9B5q?usp=sharing
3. Question 4
    1. Here we have run the best seq2seq model on the test data by using the best parameters we got in sweep. We got an accuracy of 41.67% accuracy on the unseen test data.
    2. The prediction_vanilla csv file is pushed in the github. It contains the predictions made by the our best vanilla seq2seq model.
    3. While creating the grid for input, actual output and predicted output we will mark predicted output as Red if actual output is not equal to predicted output. If they are equal then we will mark predicted output as Green.
    4. Generally the matplotlib can't recognize the Telugu Letters so we have used telugu.ttf in font properties. We have uploaded this file here in Github. If you are using colab then you have to load this file to colab.
    5. Link for the .ipynb file: https://colab.research.google.com/drive/1UvYNLVks2PdrcDd7Y2TTlwmkw-J5hLVT?usp=sharing
    
 4. Question 5 
    1. Here we have implemented the attention mechanism and ran sweep over the code.
    2. We got test accuracy as 46.058% with our best model.
    3. The prediction_attention csv file is pushed in the github. It contains the predictions made by the our best model with attention mechanism.
    4. We have added the attention heatmap images in 3\*3 grid to the report. 
    5. In attention plots Y axis contains Telugu letters. Generally the matplotlib can't recognize the Telugu Letters so we have used telugu.ttf in font properties. We have uploaded this file here in Github. If you are using colab then you have to load this file to colab.
    6. Link for the .ipynb file: https://colab.research.google.com/drive/10k1_9Yqhg9HiktsVMWt5aT78FirhlAIe?usp=sharing

5. Question 6  
    1. Here we use the best model which we got from sweep. Now by using the attention matrix which we got from running translate function we tried to show the visualization of connectivity from output to input.  
    2. We did this by using Intslider which is present in ipywidgets. We are using the slider value as index for the predicted output word. 
    3. We use the interact function to give the visualization in an interactive fashion. That is if we change the slider then it will automatically call get_color_code function which will give visualization. 
    4. Link for the .ipynb file: https://colab.research.google.com/drive/1DHQADAC7QkNGKgYKxIaewqxhpa-sggNN?usp=sharing 

**NOTE:** The code pushed from the system of CS20M009 is visible as "commited by username unknown".
