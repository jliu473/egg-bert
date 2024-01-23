# EGG-BERT: Essay GradinG BERT

EGG-BERT is a cost-effective transformer-based model for the Automatic Essay Scoring (AES) task.

(Final Project for 6.8611 Quantitative Methods for Natural Language Processing)

### Instructions for use:

1. Run the following code to install the required packages:

```bash
pip install transformers
pip install logging
pip install pytorch_lightning
pip install torchmetrics
```

2. Place the code and data files as follows:
   `me_aesdata` in the same directory as the .ipynb files

3. Change the prefix path in the first cell to the prefix path of the data files

4. Run all the code up to and including the `train()` cell.

5. After `train()` is done, model is saved to `lightning_logs/version_{latest_version}/checkpoints/epoch={latest_epoch}.ckpt`, copy this to the `saved_model_path` inside of `test()`.

6. Run the rest of the code, and the kappas will be output to the last cell.
