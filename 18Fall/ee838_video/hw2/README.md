## Dependencies

- Tensorflow 1.4
- You can install other python packages by running following command
  `pip install -r requirements.txt` 
  (sk image, numpy ...)



## Usage

- Training

    ```shell
    CUDA_VISIBLE_DEVICES=1 python -i training.py \
    --data_path=/home/siit/navi/data/input_data/ee838_hw2/ \
    --im_size=320 --batch_size=16 --ratio=1 \
    --mode=training --checkpoint_path=./01checkpoints \
    ```

    You can find the log file from `./log`, output sample from `./sample`, and check point from `./checkpoints`

     

- Testing 

    ```shell
    CUDA_VISIBLE_DEVICES=1 python -i testing.py \
    --data_path=/home/siit/navi/data/input_data/ee838_hw2/ \
    --batch_size=16 --ratio=1 \
    --mode=testing --checkpoint_path=./checkpoint \
    ```

    In order to run this, you need to put the checkpoint file in `./checkpoint`

    You can find the result file from `./log`, output images from `./sample`

