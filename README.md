# Sfm Learner_eval
Abs Rel Error Calculation

[Original Code](https://github.com/tinghuiz/SfMLearner)

# How to use

## 1 Make npy file from model

### Input Example

```shell
python test_kitti_depth.py --dataset_dir='/home/ubuntu/data/raw_data_KITTI/' --output_dir='/home/ubuntu/data/SfMLearner_result_20200413' --ckpt_file='/home/ubuntu/data/models_SfMLearner/model-190532'
```

If you want use checkpoint of struct2depth or depth from video, use the code [here](https://github.com/go125/TestCheckpointFromDFV).

## 2 Calculate Abs Rel Error


### Input Example for checkpoint from SfMLearner

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/SfMLearner_result_20200413/model-190532.npy
```

### Input Example for checkpoint from stuct2depth

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200430/result.npy
```

### Input Example for checkpoint from Depth from Video in the Wild

#### kitti_learned_intrinsics

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200501/result.npy
```

#### cityscapes_kitti_learned_intrinsics

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200501_2/result.npy
```

# Sekilab AWS Result
 
## 61468 steps (983488 images)

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/result_20200518_61468/result.npy
```


    abs_rel,     sq_rel,        rms,    log_rms,     d1_all,         a1,         a2,         a3,     scalor

    0.1504,     1.0985,     5.6942,     0.2312,     0.0000,     0.7938,     0.9295,     0.9724 ,   15.1749 
    

# Training Experiment

```
python data/prepare_train_data.py --dataset_dir=/home/ubuntu/data/raw_data_KITTI/ --dataset_name='kitti_raw_eigen' --dump_root=/home/ubuntu/SfMLearner_data/ --seq_length=3 --img_width=416 --img_height=128 --num_threads=4
```


