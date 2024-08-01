# marian_en_to_it_finetune
This readMe file contains a summary of the jupyter notebook. For more detailed recount of the processes we took to pre-train the marian model, please go through the jupyter notebook (click on marian_finetune.ipynb).

This repository contains a jupyter notebook file which showcases the steps we took to fine the Helsinki-NLP english to Italian Marian model. The model we used was a pretrained model by the University of Helsinki which we obtained through Hugging Face. The dataset we used was also obtained from Hugging Face called opus books. We split the data using 80% of it for training, 10% for testing and 10% for validation. We used a SacreBlue metric to determine the accuracy of the translation.

We tested training the marian model with different learning rates and batch sizes. We achieved the highest sacre-bleu score with learning rate of 1e-5 and batch size of 8.

There are many improvements that can be made.  Improvements that can be made are using a bigger dataset and using a bigger pre-trained transformer model. Expanding the dataset could potentially lead to substantial performance gains, as translation models heavily rely on the volume and diversity of training data. Given more time and resources, incorporating a larger dataset could be a promising avenue for enhancing the model’s accuracy and fluency. Using a bigger transformer model as a pretrained model might have yielded better results due to having more parameters.

However, due to hardware and time constraints, we were unable to adopt such a model or dataset in the current project. In future endeavors, investing in more powerful hardware and allocating time for training with larger transformer models could offer significant performance improvements.
