# OnGansAndGMMs

The project is based on the paper: https://arxiv.org/abs/1805.12462

The proposal for the project may be found here: https://www.overleaf.com/read/xgkqshgyqngd (Richardson  and  Weiss2018)

## Proposal summary

For convinience main milestones and list of experiments to be conducted is listed below (note that this list maybe changed in future):

Here we will briefly describe the goals of the project as well as important milestones.

At first, we want to reproduce the key experiments of Richardson  and  Weiss2018:
- Implement Voronoi cells based statistic test
- Implement Mixture of Factor Analysers (MFA) for data distribution modeling
- Compare MFA and GANS using statistic test proposed in paper, IS and FID on CelebA dataset.

There is also a number of interesting experiments, which can be conducted:
- Reproduce visual insights into the mode collapse problem
- Compare the ability of latent variables of GANs and GMMs to describe data manifold.
- Replace Mixture of FA with Mixture of PPCAs and compare the difference

## Team members
- Konstantin Pakulev
- Alisa Alenicheva
- Olga Tsimboy

## MFA
### Training
To train MFA from scratch you need to specify ```dataset_root``` parameter in [mfa_train.sh](mfa_train.sh). The root folder should contain folder with aligned and cropped images and train/val/test partitioning. Refer [dataset page](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html) for more info.

### Evaluation
Download the [pre-trained MFA model](https://drive.google.com/open?id=1CdSbcTV-zK55vVi3tZ-tXy0zGynZkIwp) or train it yourself.<br>
Edit ```path_to_model``` parameter in the thrid cell of [mfa_eval.ipynb](mfa_eval.ipynb) and run it.

