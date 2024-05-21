## python info 조회하기


1. python 버전 
```
# cmd에서 확인
python -v
python --version

# python에서 확인
import sys
sys.version

# 라이브러리 버전 확인
import pandas as pd
pd.__version__

# 파이썬 경로 확인(mac versino)
which python
```

  
2. torch 버전
```
import torch
torch.__version__
```

  
3. torch.gpu 사용 가능
```
import torch
print(torch.cuda.is_available())  # True/False
print(torch.cuda.device_count())  # 사용 가능한 gpu 개수
print(torch.cuda.get_device_name(torch.cuda.current_device()))  # 사용 가능한 gpu list

# tensorflow 버전
import tensorflow as tf
print("Num GPUs Available: ", len(tf.config.experimental.list_physical_devices('GPU')))  # 사용 가능한 gpu list

# mac 버전
print(f"MPS 장치를 지원하도록 build가 되었는가? {torch.backends.mps.is_built()}")
print(f"MPS 장치가 사용 가능한가? {torch.backends.mps.is_available()}")
device = torch.device("mps")

# windows 버전
device = torch.device('cuda') if torch.cuda.is_available() else torch.device('cpu')
```

  
