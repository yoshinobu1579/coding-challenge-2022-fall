# ACM Research coding challenge (Fall 2022)

## Problem to solve

Based on the data set from cars.com, estimate if the SellerRating is greater than or equal to 4.5

## Solution

I use the following strategy.

1. Use BERT pretrained model. (BertForSequenceClassification with num_labels=2)
2. Format the input like below. Used question answering.

"[CLS]Is the car's rating above 4.5?[SEP]<Column name> is <Column value>. <Column name> is <Column value>. ..."

## Result
<img width="707" alt="スクリーンショット 2022-08-29 午後10 46 35" src="https://user-images.githubusercontent.com/70049051/187345752-95b88b1e-b763-41bd-8fb9-57c5a3957713.png">

## Citation

This code is based on the `run_glue.py` script and a blog below:
https://github.com/huggingface/transformers/blob/5bfcd0485ece086ebcbed2d008813037968a9e58/examples/run_glue.py#L128
https://mccormickml.com/2019/07/22/BERT-fine-tuning/#4-train-our-classification-model


