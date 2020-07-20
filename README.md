# Sfm Learner_eval
Abs Rel Error Calculation

[Original Code](https://github.com/tinghuiz/SfMLearner)

# How to use

## 1 Make npy file from model

## Input Example

```shell
python test_kitti_depth.py --dataset_dir='/home/ubuntu/data/raw_data_KITTI/' --output_dir='/home/ubuntu/data/SfMLearner_result_20200413' --ckpt_file='/home/ubuntu/data/models_SfMLearner/model-190532'
```

If you want use checkpoint of struct2depth or depth from video, use the code [here](https://github.com/go125/TestCheckpointFromDFV).

## 2 Calculate Abs Rel Error


## Input Example for checkpoint from SfMLearner

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/SfMLearner_result_20200413/model-190532.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3,     scalor 

0.1826,     1.5948,     6.7088,     0.2700,     0.0000,     0.7339,     0.9016,     0.9593 ,    3.0119 

## Input Example for checkpoint from stuct2depth

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200430/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3,     scalor 

0.1452,     1.1166,     5.3778,     0.2183,     0.0000,     0.8127,     0.9429,     0.9779 ,   22.2982 
    
    

## Input Example for checkpoint from Depth from Video in the Wild

## kitti_learned_intrinsics

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200501/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3,     scalor 

0.1262,     0.9462,     5.2214,     0.2086,     0.0000,     0.8470,     0.9475,     0.9774 ,   28.4933


## cityscapes_kitti_learned_intrinsics

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200501_2/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3,     scalor 

0.1231,     0.8915,     5.1707,     0.2069,     0.0000,     0.8497,     0.9493,     0.9778 ,   12.4957 


## cityscapes_kitti_learned_intrinsics_gray


## 14394 steps

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/result_20200717_14394/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3,     scalor 

0.1772,     1.2595,     6.0586,     0.2490,     0.0000,     0.7409,     0.9153,     0.9710 ,   10.4929 

## 28788 steps

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/result_20200717_28788/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3,     scalor 

0.1603,     1.1314,     5.8094,     0.2339,     0.0000,     0.7773,     0.9277,     0.9742 ,    9.9255 

## 43182 steps

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/result_20200717_43182/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3,     scalor 
   
0.1492,     1.0899,     5.5213,     0.2216,     0.0000,     0.8025,     0.9363,     0.9765 ,   11.3448 

## 57576 steps

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/result_20200717_57576/result.npy
```

abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3,     scalor 

0.1465,     1.0935,     5.8459,     0.2291,     0.0000,     0.7982,     0.9323,     0.9733 ,   12.4209 

## 71970 steps

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/result_20200717_71970/result.npy
```

## 86364 steps

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/result_20200717_86364/result.npy
```



# Training Experiment

```
python data/prepare_train_data.py --dataset_dir=/home/ubuntu/data/raw_data_KITTI/ --dataset_name='kitti_raw_eigen' --dump_root=/home/ubuntu/SfMLearner_data/ --seq_length=3 --img_width=416 --img_height=128 --num_threads=4
```


