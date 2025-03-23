# [SAKSRNet for NTIRE 2025 Challenge on Image Super-Resolution (x4)](https://cvlai.net/ntire/2025/) @ [CVPR 2025](https://cvpr.thecvf.com/)

## How to test the baseline model?

1. `git clone https://github.com/sander-ali/SAKSRNet.git`
2. Run the code using the following command
    ```
    python test.py --test_dir testset --model_id 21
    ```

### Weighted score for Perception Quality Track

We use the following equation to calculate the final weight score: 

$$
\text{Score} = \left(1 - \text{LPIPS}\right) + \left(1 - \text{DISTS}\right) + \text{CLIPIQA} + \text{MANIQA} + \frac{\text{MUSIQ}}{100} + \max\left(0, \frac{10 - \text{NIQE}}{10}\right). 
$$

The score is calculated on the averaged IQA scores. 

## License and Acknowledgement
This code repository is release under [MIT License](LICENSE). 

## The proposed workflow of SAKSRNet is shown below

![network_diagram](https://github.com/user-attachments/assets/605cbf21-6067-4915-9979-63e4bd111d78)

## Some visual results are also shown below.

![results1](https://github.com/user-attachments/assets/fb13abfc-0a57-4b05-9376-579a2bf1dc03)


![results2](https://github.com/user-attachments/assets/0ad5fd12-5960-4372-8074-b39ec82d9287)

