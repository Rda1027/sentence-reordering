# sentence-reordering
Sentence Reordering task completed through the implementation of a Transformer.

## Project Description
This project simply aim to build a model able to take as input shuffled sentences and respond as an output with the sentence ordered.
In order to accomplish such an objective it has been used a Transformer, very popular neural network structure used for NLP applications.

## Implementation Details

### DUMP_ENABLE

Simple Boolean variable helpful in understanding which portion of code need to be executed.

    DUMP_ENABLE = False

Following this option, I included only cells where dataset is downloaded, tokenized (and eventually detokenized) from scratch. 

    DUMP_ENABLE = True

Following this option, I manage to avoid downloading the dataset and adapting the tokenizer to such text from scratch, while I simply use pkl files in the Resources directory. 

### Weights

The model can be retrained again or it can be updated to last found best weights, reading them from the my_weights3.h5 file in the Resources directory.

## Credits

The overall structure of the Transformer is based on the one proposed in the [Tensorflow](https://www.tensorflow.org/text/tutorials/transformer) documentation.

I also took inspiration from a new structure template based on a [reaserch](https://arxiv.org/abs/2002.04745), called "On Layer Normalization in the Transformer Architecture" by Ruibin Xiong, Yunchang Yang, Di He, Kai Zheng, Shuxin Zheng, Chen Xing, Huishuai Zhang, Yanyan Lan, Liwei Wang, Tie-Yan Liu.