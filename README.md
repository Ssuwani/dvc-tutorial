# DVC Tutorial

Data Version Control의 사용법을 간단히 작성해보았습니다.

- `upload_data.ipynb`
- `load_from_dvc.ipynb`

두개의 파일을 확인하면 됩니다.

`tf.keras.datasets.mnist.load_data()` 를 통해 60000개의 학습용 데이터를 얻을 수 있습니다. 이를 10000개씩 분할하여 DVC로 관리하였습니다. 실제로 버져닝된 데이터가 저장되는 경로는 GCS입니다. 따라서 이 레포를 클론해서 실행하려면 `upload_data.ipynb` 내 `gsutil mb` 를 적절한 이름으로 변경해야 합니다. 그리고 업로드 된 데이터를 불러와 확인하기 위한 `load_from_dvc.ipynb` 는 제 버킷의 권한을 모두에게 허용하지 않았기 때문에 권한 에러가 발생합니다. 각자의 리모트 폴더를 만드셔서 따라해보시기 바랍니다.



현 레포지토리 내 tag로 버전을 관리하였습니다.

- Version 1 : 10000 / 60000
- Version 2 : 20000 / 60000
- Version 3 : 30000 / 60000
- Version 4 : 40000 / 60000
- Version 5 : 50000 / 60000
- Version 6 : 60000 / 60000

