# challenge_arrhythmia-classification
환자들의 1 lead ECG(심전도)를 이용하여 AF, Normal, other rhythm , noisy 진단
Baseline model : 방법1과 같은 딥러닝 구조. 30초 데이터만 사용 (n=5,977)

## Methods 
- 기본 hyperparameter 고정 (baseline model)
max epoch =100 , early stopping (validation loss 기준)
learning rate = 1e-3

- Hyper-parameter별 성능 관찰 
LSTM layer 수
Batch normalization 적용
Label smoothing
Focal loss function 적용

## Reference
Classification of Cardiac Arrhythmias from Single Lead ECG with a Convolutional Recurrent Neural Network 
https://arxiv.org/abs/1907.01513
