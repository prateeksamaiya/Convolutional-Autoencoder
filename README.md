# Convolutional-Autoencoder
Convolution Encoder for compressed image representation


#Instruction
```
Open the notebook in jupyter
if you want to work with different image size just change the linear layer input just after the 5th convoltion

        self.conv5 = nn.Conv2d(128,256,3,stride=2)  #256*4*4
 ------>self.lineartohidden = nn.Linear(linear_input_size,embedding_size)
 ------>self.hiddentolinear = nn.Linear(embedding_size,linear_input_size)                            
        self.deconv5 = nn.ConvTranspose2d(256,128,3,stride=2)  

If you are unable to calculate the linear_input_size, dont worry just run the network with your input image of any size for eg 445*445 (has to be square always otherwise deconvoultion dimension might change) and when you run the train function it will throw an error giving you the correct linear_imput_size
```
