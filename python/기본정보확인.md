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
```

  
