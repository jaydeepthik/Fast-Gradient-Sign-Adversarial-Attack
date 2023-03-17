# Fast-Gradient-Sign-Adversarial-Attack

Fast Gradient Sign Adversarial Attack(FGSM) examples creation using FashionMnist dataset. <br>
inspiration: https://pytorch.org/tutorials/beginner/fgsm_tutorial.html

## About Adversarial Attacks:

# Fast Gradient Sign Attack:

`General goal`: Add the least amount of pertubations to the input that causes desired misclassification.<br>

`Assumptions on attacker's knowledge`: <br>

1.   White-Box: Attacker has full knowledge and access to the model, architecture, inputs, outputs and weights.
2.   Black-Box: Attacher has knowledge only about the inputs and outputs of the model and no information about the underlynig model architecture or weights.<br>

`Goals`:<br>
1. misclassification: Attacker only wants the output classification to be wrong and does not care about what the new classification is.
1. Source/Target misclassification: pertubations to the input that belongs to a specific source class so that it is classified as a specific target class.<br>

FGSM : `White-box` attack with the goal of `misclassification`.<br>

`Fast Gradient Sign Attack`: Use gradient of the loss w.r.t input data, then adjust the inputs to maximize the loss
