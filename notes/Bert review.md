---
title: Bert review
created: '2022-04-03T23:45:41.477Z'
modified: '2022-04-04T21:19:43.851Z'
---

# Bert review

original :

python -m set_sail.model_archive.deep_learning_sequencing.train_model --data_path "/data/rossi_data/training_data/20220112_sgko_train_data_best.csv" --experiment_name token_size_3 --num_gpus 4 --target_feature quality_score --classification --model_type transformer --token_size 3 --batch_size 16

python -m set_sail.model_archive.deep_learning_sequencing.train_model --data_path "/data/rossi_data/training_data/040322_sgko_train_data_best_regression.csv" --experiment_name token_size_3 --num_gpus 4 --target_feature quality_score --model_type transformer --token_size 3 --batch_size 16



Things are working with one GPU but not generalizeing


# this works with one GPU
python -m set_sail.model_archive.deep_learning_sequencing.train_model --data_path "/data/rossi_data/training_data/040322_sgko_train_data_best_softlabels.csv" --experiment_name token_size_3 --num_gpus 1 --target_feature quality_score --model_type transformer --token_size 3 --batch_size 16


#lets try big 
python -m set_sail.model_archive.deep_learning_sequencing.train_model --data_path "/data/rossi_data/training_data/20220112_sgko_train_data_best.csv" --experiment_name token_size_3_classification --num_gpus 1 --target_feature quality_score --classification --model_type transformer --token_size 3 --batch_size 16
