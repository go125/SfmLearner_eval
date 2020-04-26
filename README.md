# Sfm Learner
Abs Rel Error Calculation

# How to use

## 1 Make npy file from model

```shell
python test_kitti_depth.py --dataset_dir='/home/ubuntu/data/raw_data_KITTI/' --output_dir='/home/ubuntu/data/SfMLearner_result_20200413' --ckpt_file='/home/ubuntu/data/models_SfMLearner/model-190532'
```

If you want use checkpoint of struct2depth or depth from video, use the code [here](https://github.com/go125/TestCheckpointFromDFV).

## 2 Calculate Abs Rel Error


### For checkpoint from SfMLearner

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/SfMLearner_result_20200413/model-190532.npy
```

### For checkpoint from stuct2depth

```shell
python kitti_eval/eval_depth.py --kitti_dir=/home/ubuntu/data/raw_data_KITTI/ --pred_file=/home/ubuntu/data/dfv_KITTI_depth_result_20200414/result.npy
```
