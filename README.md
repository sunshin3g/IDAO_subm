### Sigma Chad Machines team solution for the first stage of IDAO 2022, first section.
### Solution description
Our solution is a simple blend of five instances of the SOTA model.  
The initial code of the model was taken from here: [deeperGATGNN github](https://github.com/usccolumbia/deeperGATGNN)

We made a couple of engineering modification to the initial code.  
It was required simply to make it work on Google Colab. It doesn't include any changes related to the model architecture or other scientific stuff.   
We also converted material data to .cif format. However, we did not conduct any other manual preprocessing of the material data.

Finally, we trained five NN with deeperGATGNN architecture. There's only a little variability in the hyperparameters of the models except random seeds.
We averaged predictions of the models in order to make a prediction for the final submission. 

### How to reproduce final submission
1. Actually, the only required thing is to open final_submission notebook on Colab and run all cells consequently. It should only take about 15 minutes to get predictions.
2. If you don't want to use Colab, you may face some issues with CUDA version and other GPU stuff. If it is the case, you may look for a proper installation guide in [the deeperGATGNN repository's README.](https://github.com/usccolumbia/deeperGATGNN) 
