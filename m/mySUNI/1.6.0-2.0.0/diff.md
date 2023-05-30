# Comparing `tmp/mySUNI-1.6.0-py3-none-any.whl.zip` & `tmp/mySUNI-2.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 22213 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat       22 b- defN 22-Nov-02 05:50 mySUNI/__init__.py
--rw-rw-rw-  2.0 fat    15396 b- defN 22-Nov-02 05:49 mySUNI/cds.py
--rw-rw-rw-  2.0 fat    16768 b- defN 22-Aug-25 04:40 mySUNI/utils.py
--rw-rw-rw-  2.0 fat    34523 b- defN 22-Nov-02 05:50 mySUNI-1.6.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      503 b- defN 22-Nov-02 05:50 mySUNI-1.6.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Nov-02 05:50 mySUNI-1.6.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 22-Nov-02 05:50 mySUNI-1.6.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      597 b- defN 22-Nov-02 05:50 mySUNI-1.6.0.dist-info/RECORD
-8 files, 67908 bytes uncompressed, 21183 bytes compressed:  68.8%
+Zip file size: 22525 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat       23 b- defN 23-May-30 00:27 mySUNI/__init__.py
+-rw-rw-rw-  2.0 fat    16136 b- defN 23-May-30 00:26 mySUNI/cds.py
+-rw-rw-rw-  2.0 fat    17226 b- defN 23-May-30 00:26 mySUNI/utils.py
+-rw-rw-rw-  2.0 fat    35184 b- defN 23-May-30 00:28 mySUNI-2.0.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      547 b- defN 23-May-30 00:28 mySUNI-2.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 00:28 mySUNI-2.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-May-30 00:28 mySUNI-2.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      597 b- defN 23-May-30 00:28 mySUNI-2.0.0.dist-info/RECORD
+8 files, 69812 bytes uncompressed, 21495 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: mySUNI/cds.py
 Comment: 
 
 Filename: mySUNI/utils.py
 Comment: 
 
-Filename: mySUNI-1.6.0.dist-info/LICENSE
+Filename: mySUNI-2.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: mySUNI-1.6.0.dist-info/METADATA
+Filename: mySUNI-2.0.0.dist-info/METADATA
 Comment: 
 
-Filename: mySUNI-1.6.0.dist-info/WHEEL
+Filename: mySUNI-2.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: mySUNI-1.6.0.dist-info/top_level.txt
+Filename: mySUNI-2.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: mySUNI-1.6.0.dist-info/RECORD
+Filename: mySUNI-2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mySUNI/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '1.6.0'
+__version__ = '2.0.0'
```

## mySUNI/cds.py

```diff
@@ -1,371 +1,374 @@
-import json
-import datetime
-import requests
-import urllib
-import pandas as pd
-import seaborn as sns
-import requests
-from requests.auth import HTTPBasicAuth
-import os
-import time
-import datetime
-from tqdm.notebook import tqdm
-import zipfile
-from IPython.display import clear_output
-
-# 데이터셋 JSON 파일 경로
-DATASET_DATA_PATH = 'dataset.json'
-DATASET_DOWNLOAD_URL = 'https://raw.githubusercontent.com/braincrew/cds/main/mySUNI/data/dataset.json'
-
-# 프로젝트 관련 파일 JSON 파일 경로
-PROJECT_DATA_PATH = 'project.json'
-PROJECT_DOWNLOAD_URL = 'https://raw.githubusercontent.com/braincrew/cds/main/mySUNI/data/project.json'
-
-# 워크샵 관련 파일 JSON 파일 경로
-WORKSHOP_DATA_PATH = 'workshop.json'
-WORKSHOP_DOWNLOAD_URL = 'https://raw.githubusercontent.com/braincrew/cds/main/mySUNI/data/workshop.json'
-
-
-####### 데이터셋 관련 모듈 #######
-
-class Dataset:
-
-    def __init__(self, data_dir='data'):
-        self.data_dir = data_dir
-        # data 폴더 생성
-        if not os.path.exists(data_dir):
-            os.makedirs(data_dir)
-
-        r = requests.get(DATASET_DOWNLOAD_URL)
-        open(DATASET_DATA_PATH, 'wb').write(r.content)
-
-        with open(DATASET_DATA_PATH) as f:
-            datasets = json.load(f)
-
-
-        titles = []
-        infos = []
-        datas = []
-        filenames = []
-
-        for name_ in datasets:
-            titles.append(name_)
-            infos.append(datasets[name_]['info'])
-            datas.append(datasets[name_]['data'])
-            filenames.append(datasets[name_]['filename'])
-
-        self.dataset = pd.DataFrame({
-            'name': titles,
-            'info': infos,
-            'data': datas,
-            'filename': filenames,
-        })
-
-
-    def info(self):
-        display(self.dataset[['name', 'info', 'filename']])
-
-
-    def load(self, dataset_names):
-        global datasets
-        username = 'mysuni'
-        password = 'mysuni1!'
-
-        if type(dataset_names) == str:
-            df = self.dataset.loc[self.dataset['name'] == dataset_names]
-            if df.shape[0] > 0:
-                fileurl = df['data']
-                filename = df['filename']
-                for f_name, f_url in zip(filename.iloc[0], fileurl.iloc[0]):
-                    r = requests.get(f_url, auth=HTTPBasicAuth(username, password))
-                    filepath = os.path.join(self.data_dir, f_name)
-                    open(filepath, 'wb').write(r.content)
-                    print(f'파일 다운로드 완료\n====================\n\n데이터셋: {dataset_names}\n파일경로: {filepath}\n\n====================')
-                return
-            else:
-                raise Exception('데이터셋 정보가 없습니다.')
-
-        elif type(dataset_names) == list or type(dataset_names) == tuple:
-            for dataset_name in dataset_names:
-                df = self.dataset.loc[self.dataset['name'] == dataset_name]
-                if df.shape[0] > 0:
-                    fileurls = df['data'].iloc[0]
-                    filenames = df['filename'].iloc[0]
-                    for fileurl, filename in zip(fileurls, filenames):
-                        r = requests.get(fileurl, auth=HTTPBasicAuth(username, password))
-                        filepath = os.path.join(self.data_dir, filename)
-                        open(filepath, 'wb').write(r.content)
-                        print(f'파일 다운로드 완료\n====================\n\n데이터셋: {dataset_name}\n파일경로: {filepath}\n\n====================')
-                else:
-                    raise Exception('데이터셋 정보가 없습니다.')
-            return
-        else:
-            raise Exception('잘못된 정보입니다.')
-
-
-dataset = Dataset()
-
-
-def list_data():
-    global dataset
-    dataset.info()
-
-
-def download_data(dataset_name):
-    global dataset
-    return dataset.load(dataset_name)
-
-####### 워크샵 관련 모듈 #######
-
-# q = {'mySUNI-WorkShop-00-Python':['mySUNI-WorkShop-00-Python-실습.ipynb'],
-#  'mySUNI-WorkShop-01-StepWalk':['mySUNI-WorkShop-01-StepWalk-실습.ipynb'],
-#  'mySUNI-WorkShop-02-Pandas':['mySUNI-WorkShop-02-Pandas-실습.ipynb'],
-#  'mySUNI-WorkShop-03-타이타닉 생존자 분석':['mySUNI-WorkShop-03-타이타닉 생존자 분석-실습.ipynb'],
-#  'mySUNI-WorkShop-04-타이타닉 생존자 예측':['mySUNI-WorkShop-04-타이타닉 생존자 예측-실습.ipynb'],
-# 'mySUNi-WorkShop-05-데이터 전처리 및 분석':['mySUNI-WorkShop-CCTV 데이터 분석(실습).ipynb',
-#  'mySUNI-WorkShop-국민연금 데이터 분석(실습).ipynb',
-#  'mySUNI-WorkShop-민간 아파트 가격동향 분석(실습).ipynb',
-#  'mySUNI-WorkShop-아파트 실거래가 분석 I(실습).ipynb',
-#  'mySUNI-WorkShop-아파트 실거래가 분석 II(실습).ipynb',
-#  'mySUNI-WorkShop-유가 가격 분석 (실습).ipynb',
-#  'mySUNI-WorkShop-중고차 판매 정보 분석 (실습).ipynb'],
-#  'mySUNI-WorkShop-06-웨이퍼 불량 유형 분류':['mySUNI-WorkShop-06-웨이퍼 불량 유형 분류-실습(코드추가).ipynb',
-#   'mySUNI-WorkShop-06-웨이퍼 불량 유형 분류-실습.ipynb'],
-#  'mySUNI-WorkShop-07-따릉이 대여량 예측':['mySUNI-WorkShop-07-따릉이 대여량 예측-실습(코드추가).ipynb',
-#   'mySUNI-WorkShop-07-따릉이 대여량 예측-실습.ipynb'],
-#  'mySUNI-WorkShop-08-집 값 예측':['mySUNI-WorkShop-08-집 값 예측-실습(코드추가).ipynb',
-#   'mySUNI-WorkShop-08-집 값 예측-실습.ipynb'],
-#  'mySUNI-WorkShop-09-머신러닝 연습':['mySUNI-WorkShop-빌딩 전력 소모량 예측 (실습).ipynb',
-#   'mySUNI-WorkShop-사용자 이탈 예측 (실습).ipynb',
-#   'mySUNI-WorkShop-에너지 효율 예측 (실습).ipynb',
-#   'mySUNI-WorkShop-와인 유형 분류 (실습).ipynb']}
-
-# s = {'mySUNI-WorkShop-00-Python':['mySUNI-WorkShop-00-Python-해설.ipynb'],
-#  'mySUNI-WorkShop-01-StepWalk':['mySUNI-WorkShop-01-StepWalk-해설.ipynb'],
-#  'mySUNI-WorkShop-02-Pandas':['mySUNI-WorkShop-02-Pandas-해설.ipynb'],
-#  'mySUNI-WorkShop-03-타이타닉 생존자 분석':['mySUNI-WorkShop-03-타이타닉 생존자 분석-해설.ipynb'],
-#  'mySUNI-WorkShop-04-타이타닉 생존자 예측':['mySUNI-WorkShop-04-타이타닉 생존자 예측-해설.ipynb'],
-# 'mySUNi-WorkShop-05-데이터 전처리 및 분석':['mySUNI-WorkShop-CCTV 데이터 분석(해설).ipynb',
-#  'mySUNI-WorkShop-국민연금 데이터 분석(해설).ipynb',
-#  'mySUNI-WorkShop-민간 아파트 가격동향 분석(해설).ipynb',
-#  'mySUNI-WorkShop-아파트 실거래가 분석 I(해설).ipynb',
-#  'mySUNI-WorkShop-아파트 실거래가 분석 II(해설).ipynb',
-#  'mySUNI-WorkShop-유가 가격 분석 (해설).ipynb',
-#  'mySUNI-WorkShop-중고차 판매 정보 분석 (해설).ipynb'],
-#  'mySUNI-WorkShop-06-웨이퍼 불량 유형 분류':['mySUNI-WorkShop-06-웨이퍼 불량 유형 분류-해설.ipynb'],
-#  'mySUNI-WorkShop-07-따릉이 대여량 예측':['mySUNI-WorkShop-07-따릉이 대여량 예측-해설.ipynb'],
-#  'mySUNI-WorkShop-08-집 값 예측':['mySUNI-WorkShop-08-집 값 예측-해설.ipynb'],
-#  'mySUNI-WorkShop-09-머신러닝 연습':['mySUNI-WorkShop-빌딩 전력 소모량 예측 (해설).ipynb',
-#   'mySUNI-WorkShop-사용자 이탈 예측 (해설).ipynb',
-#   'mySUNI-WorkShop-에너지 효율 예측 (해설).ipynb',
-#   'mySUNI-WorkShop-와인 유형 분류 (해설).ipynb']}
-
-r = requests.get(WORKSHOP_DOWNLOAD_URL)
-open(WORKSHOP_DATA_PATH, 'wb').write(r.content)
-
-with open(WORKSHOP_DATA_PATH) as f:
-    workshops = json.load(f)
-    
-q = workshops['q']
-s = workshops['s']
-
-def list_workshop():
-    workshop = pd.DataFrame({
-        '워크샵':q.keys(),
-    })
-    display(workshop.sort_values('워크샵'))
-
-def download_workshop(workshop_name, sol=False, local=False):
-    # auth
-    username = 'mysuni'
-    password = 'mysuni1!'
-
-    if local:
-        if not os.path.exists(os.path.join('workshop', f'{workshop_name}')):
-            os.makedirs(os.path.join('workshop', f'{workshop_name}'))
-
-    else:
-        if not os.path.exists(os.path.join('/mnt/elice', 'workshop', f'{workshop_name}')):
-            os.makedirs(os.path.join('/mnt/elice', 'workshop', f'{workshop_name}'))
-
-    if sol:
-        workshop_files = s[workshop_name]
-    else:
-        workshop_files = q[workshop_name]
-
-    print(f'워크샵: {workshop_files}\n==============================\n파일 정보\n')
-    for workshop_file in workshop_files:
-        fileurl = "http://sk.jaen.kr:8080/workshop/" + workshop_file
-        r = requests.get(fileurl, auth=HTTPBasicAuth(username, password))
-        if local:
-            filepath = os.path.join('workshop', f'{workshop_name}', workshop_file)
-        else:
-            filepath = os.path.join('/mnt/elice','workshop', f'{workshop_name}', workshop_file)
-
-        if os.path.exists(filepath):
-            file = filepath.split('.')
-            now = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
-            file[0] = file[0] + now
-            filepath = ".".join(file)
-        open(filepath, 'wb').write(r.content)
-        print(f'저장 위치:\t {filepath}')
-    print(f'\n==============================')
-
-
-####### 프로젝트 관련 모듈 #######
-
-project = None
-
-
-class Project:
-    def __init__(self, project_name, class_info, email, server='manage'):
-        self.project_name = project_name
-        self.edu_name = "mySUNI"
-        self.edu_rnd = class_info.split()[0]
-        self.edu_class = class_info.split()[1]
-        self.email = email
-        self.server = server
-
-        r = requests.get(PROJECT_DOWNLOAD_URL)
-        open(PROJECT_DATA_PATH, 'wb').write(r.content)
-
-    def __make_submission(self, submission):
-        timestring = datetime.datetime.now().strftime('%H-%M-%S')
-        filename = 'submission-{}.csv'.format(timestring)
-        submission.to_csv(filename, index=False)
-        print('파일을 저장하였습니다. 파일명: {}'.format(filename))
-        return filename
-
-    def __project_submission(self, file_name):
-        file_path = './'
-        url = f'http://{self.server}.jaen.kr/api/studentProject/apiScoring?edu_name={self.edu_name}\
-        &edu_rnd={self.edu_rnd}&edu_class={self.edu_class}&mail={self.email}&project_name={self.project_name}&file_name={file_name}'
-        files = {'file': (file_name, open(file_path + file_name, 'rb'), 'text/csv')}
-        r = requests.post(url, files=files)
-        r.encoding = 'utf-8'
-        message = ''
-        try:
-            data = json.loads(r.text) # json 변환 실패시 원본 메세지 사용
-            if 'trial' in data.keys():
-                message = '제출 여부 :{}\n오늘 제출 횟수 : {}\n제출 결과:{}'.format(data['msg'], data['trial'], data['score'])
-            else:
-                message = '제출 실패 : {}'.format(data['msg'])
-        except:
-            message = '변환 에러 발생 : {}'.format(r.text)
-        return message
-
-    def project_final_submission(self, name, ipynb_file_path=None):
-        url = "http://sk.jaen.kr/submission_final"
-        files = []
-        if ipynb_file_path is None:
-            raise Exception('노트북(ipynb) 파일의 경로를 입력해 주세요.') 
-        files.append(('file', open(ipynb_file_path, 'rb')))
-        data = {'name': name, 'rnd':self.edu_rnd, 'class':self.edu_class}
-        res = requests.post(url, data=data, files=files)
-        print(res.text)
-
-    def submit(self, submission):
-        filename = self.__make_submission(submission)
-        print(self.__project_submission(filename))
-
-
-def download_project(project_name, class_info, email, use_path=None, skip_download=False, server='manage'):
-    '''
-    use_path: 지정 폴더에 다운로드
-    skip_download: 폴더에 데이터가 존재할 시 SKIP. 단 CHECKSUM 비교는 안함.
-    '''
-    global project, files
-    try:
-        project = Project(project_name, class_info=class_info, email=email, server=server)
-
-        # data 폴더 경로 지정
-        DATA_DIR = 'data'
-        if use_path is not None:
-            DATA_DIR = use_path
-
-        with open(PROJECT_DATA_PATH) as f:
-            datasets = json.load(f)
-
-        # data 폴더 생성
-        if not os.path.exists(os.path.join(DATA_DIR, project_name)):
-            os.makedirs(os.path.join(DATA_DIR, project_name))
-
-        project_files = datasets[project_name]
-
-        # skip download 체크
-        file_to_remove = []
-        if skip_download:
-            for filename, _ in project_files.items():
-                filepath = os.path.join(DATA_DIR, project_name, filename)
-                if os.path.exists(filepath):
-                    file_to_remove.append(filename)
-                    print(f'{filename} 파일이 {filepath} 이미 존재하여 다운로드를 SKIP 합니다..')
-
-        print(f'카운트 다운!')
-        time_cnt = 1
-        while time_cnt <= 3:
-            print(f'{time_cnt}', end=' ')
-            time.sleep(1)
-            time_cnt += 1
-        clear_output(wait=True)
-
-        for k in file_to_remove:
-            project_files.pop(k)
-
-        # auth
-        username = 'mysuni'
-        password = 'mysuni1!'
-
-        print(f'프로젝트: {project_name}\n==============================\n파일 다운로드\n')
-        for filename, fileurl in project_files.items():
-            r = requests.get(fileurl, auth=HTTPBasicAuth(username, password), stream=True)
-
-            filepath = os.path.join(DATA_DIR, project_name, filename)
-            print(f'{filename}', end=' ')
-
-            ## 다운로드 progress bar 추가 ##
-            total_size_in_bytes = int(r.headers.get('content-length', 0))
-            block_size = 1024
-
-            progress_bar = tqdm(total=total_size_in_bytes, unit='B', unit_scale=True)
-            with open(filepath, 'wb') as file:
-                for data in r.iter_content(block_size):
-                    progress_bar.update(len(data))
-                    file.write(data)
-            progress_bar.close()
-            if total_size_in_bytes != 0 and progress_bar.n != total_size_in_bytes:
-                print("ERROR: 다운로드 도중 에러가 발생하였습니다.")
-            else:
-                if filepath.endswith('.zip'):
-                    print(f'압축 해제 및 프로젝트 파일 구성중...')
-                    zipfile.ZipFile(filepath).extractall(os.path.join(DATA_DIR, project_name))
-            ## 다운로드 progress bar 추가 ##
-        clear_output(wait=True)
-        print(f'\n==============================')
-        print(f'프로젝트: {project_name}\n==============================\n파일 목록\n')
-        for f in [fs for fs in os.listdir(os.path.join('data', project_name)) if 'csv' in fs]:
-            print(f'{f}\n- {os.path.join(DATA_DIR, project_name, f)}\n')
-        print(f'==============================')
-    except Exception as err:
-        print(err)
-        raise Exception('잘못된 정보입니다.')
-
-
-def submit(submission_file):
-    global project
-    project.submit(submission_file)
-
-
-def end_project(name, ipynb_file_path):
-    global project
-    project.project_final_submission(name, ipynb_file_path)
-
-def update_project(project_name=None, class_info=None, email=None):
-    global project
-    if project_name:
-        project.project_name = project_name
-    if project.class_info:
-        project.class_info = class_info
-    if project.email:
-        project.email = email
-    print('정보 업데이트 완료')
+import json
+import datetime
+import requests
+import urllib
+import pandas as pd
+import seaborn as sns
+import requests
+from requests.auth import HTTPBasicAuth
+import os
+import time
+import datetime
+from tqdm.notebook import tqdm
+import zipfile
+from IPython.display import clear_output
+
+# 데이터셋 JSON 파일 경로
+DATASET_DATA_PATH = 'dataset.json'
+# DATASET_DOWNLOAD_URL = 'https://raw.githubusercontent.com/braincrew/cds/main/mySUNI/data/dataset.json'
+DATASET_DOWNLOAD_URL = 'http://data.jaen.kr/download?download_path=%2Fdata%2Ffiles%2FmySUNI%2Fdatasets%2Fdataset.json'
+
+# 프로젝트 관련 파일 JSON 파일 경로
+PROJECT_DATA_PATH = 'project.json'
+# PROJECT_DOWNLOAD_URL = 'https://raw.githubusercontent.com/braincrew/cds/main/mySUNI/data/project.json'
+PROJECT_DOWNLOAD_URL = 'http://data.jaen.kr/download?download_path=%2Fdata%2Ffiles%2FmySUNI%2Fdatasets%2Fproject.json'
+
+# 워크샵 관련 파일 JSON 파일 경로
+WORKSHOP_DATA_PATH = 'workshop.json'
+# WORKSHOP_DOWNLOAD_URL = 'https://raw.githubusercontent.com/braincrew/cds/main/mySUNI/data/workshop.json'
+WORKSHOP_DOWNLOAD_URL = 'http://data.jaen.kr/download?download_path=%2Fdata%2Ffiles%2FmySUNI%2Fdatasets%2Fworkshop.json'
+
+
+####### 데이터셋 관련 모듈 #######
+
+class Dataset:
+
+    def __init__(self, data_dir='data'):
+        self.data_dir = data_dir
+        # data 폴더 생성
+        if not os.path.exists(data_dir):
+            os.makedirs(data_dir)
+
+        r = requests.get(DATASET_DOWNLOAD_URL)
+        open(DATASET_DATA_PATH, 'wb').write(r.content)
+
+        with open(DATASET_DATA_PATH) as f:
+            datasets = json.load(f)
+
+
+        titles = []
+        infos = []
+        datas = []
+        filenames = []
+
+        for name_ in datasets:
+            titles.append(name_)
+            infos.append(datasets[name_]['info'])
+            datas.append(datasets[name_]['data'])
+            filenames.append(datasets[name_]['filename'])
+
+        self.dataset = pd.DataFrame({
+            'name': titles,
+            'info': infos,
+            'data': datas,
+            'filename': filenames,
+        })
+
+
+    def info(self):
+        display(self.dataset[['name', 'info', 'filename']])
+
+
+    def load(self, dataset_names):
+        global datasets
+        username = 'mysuni'
+        password = 'mysuni1!'
+
+        if type(dataset_names) == str:
+            df = self.dataset.loc[self.dataset['name'] == dataset_names]
+            if df.shape[0] > 0:
+                fileurl = df['data']
+                filename = df['filename']
+                for f_name, f_url in zip(filename.iloc[0], fileurl.iloc[0]):
+                    r = requests.get(f_url, auth=HTTPBasicAuth(username, password))
+                    filepath = os.path.join(self.data_dir, f_name)
+                    open(filepath, 'wb').write(r.content)
+                    print(f'파일 다운로드 완료\n====================\n\n데이터셋: {dataset_names}\n파일경로: {filepath}\n\n====================')
+                return
+            else:
+                raise Exception('데이터셋 정보가 없습니다.')
+
+        elif type(dataset_names) == list or type(dataset_names) == tuple:
+            for dataset_name in dataset_names:
+                df = self.dataset.loc[self.dataset['name'] == dataset_name]
+                if df.shape[0] > 0:
+                    fileurls = df['data'].iloc[0]
+                    filenames = df['filename'].iloc[0]
+                    for fileurl, filename in zip(fileurls, filenames):
+                        r = requests.get(fileurl, auth=HTTPBasicAuth(username, password))
+                        filepath = os.path.join(self.data_dir, filename)
+                        open(filepath, 'wb').write(r.content)
+                        print(f'파일 다운로드 완료\n====================\n\n데이터셋: {dataset_name}\n파일경로: {filepath}\n\n====================')
+                else:
+                    raise Exception('데이터셋 정보가 없습니다.')
+            return
+        else:
+            raise Exception('잘못된 정보입니다.')
+
+
+dataset = Dataset()
+
+
+def list_data():
+    global dataset
+    dataset.info()
+
+
+def download_data(dataset_name):
+    global dataset
+    return dataset.load(dataset_name)
+
+####### 워크샵 관련 모듈 #######
+
+# q = {'mySUNI-WorkShop-00-Python':['mySUNI-WorkShop-00-Python-실습.ipynb'],
+#  'mySUNI-WorkShop-01-StepWalk':['mySUNI-WorkShop-01-StepWalk-실습.ipynb'],
+#  'mySUNI-WorkShop-02-Pandas':['mySUNI-WorkShop-02-Pandas-실습.ipynb'],
+#  'mySUNI-WorkShop-03-타이타닉 생존자 분석':['mySUNI-WorkShop-03-타이타닉 생존자 분석-실습.ipynb'],
+#  'mySUNI-WorkShop-04-타이타닉 생존자 예측':['mySUNI-WorkShop-04-타이타닉 생존자 예측-실습.ipynb'],
+# 'mySUNi-WorkShop-05-데이터 전처리 및 분석':['mySUNI-WorkShop-CCTV 데이터 분석(실습).ipynb',
+#  'mySUNI-WorkShop-국민연금 데이터 분석(실습).ipynb',
+#  'mySUNI-WorkShop-민간 아파트 가격동향 분석(실습).ipynb',
+#  'mySUNI-WorkShop-아파트 실거래가 분석 I(실습).ipynb',
+#  'mySUNI-WorkShop-아파트 실거래가 분석 II(실습).ipynb',
+#  'mySUNI-WorkShop-유가 가격 분석 (실습).ipynb',
+#  'mySUNI-WorkShop-중고차 판매 정보 분석 (실습).ipynb'],
+#  'mySUNI-WorkShop-06-웨이퍼 불량 유형 분류':['mySUNI-WorkShop-06-웨이퍼 불량 유형 분류-실습(코드추가).ipynb',
+#   'mySUNI-WorkShop-06-웨이퍼 불량 유형 분류-실습.ipynb'],
+#  'mySUNI-WorkShop-07-따릉이 대여량 예측':['mySUNI-WorkShop-07-따릉이 대여량 예측-실습(코드추가).ipynb',
+#   'mySUNI-WorkShop-07-따릉이 대여량 예측-실습.ipynb'],
+#  'mySUNI-WorkShop-08-집 값 예측':['mySUNI-WorkShop-08-집 값 예측-실습(코드추가).ipynb',
+#   'mySUNI-WorkShop-08-집 값 예측-실습.ipynb'],
+#  'mySUNI-WorkShop-09-머신러닝 연습':['mySUNI-WorkShop-빌딩 전력 소모량 예측 (실습).ipynb',
+#   'mySUNI-WorkShop-사용자 이탈 예측 (실습).ipynb',
+#   'mySUNI-WorkShop-에너지 효율 예측 (실습).ipynb',
+#   'mySUNI-WorkShop-와인 유형 분류 (실습).ipynb']}
+
+# s = {'mySUNI-WorkShop-00-Python':['mySUNI-WorkShop-00-Python-해설.ipynb'],
+#  'mySUNI-WorkShop-01-StepWalk':['mySUNI-WorkShop-01-StepWalk-해설.ipynb'],
+#  'mySUNI-WorkShop-02-Pandas':['mySUNI-WorkShop-02-Pandas-해설.ipynb'],
+#  'mySUNI-WorkShop-03-타이타닉 생존자 분석':['mySUNI-WorkShop-03-타이타닉 생존자 분석-해설.ipynb'],
+#  'mySUNI-WorkShop-04-타이타닉 생존자 예측':['mySUNI-WorkShop-04-타이타닉 생존자 예측-해설.ipynb'],
+# 'mySUNi-WorkShop-05-데이터 전처리 및 분석':['mySUNI-WorkShop-CCTV 데이터 분석(해설).ipynb',
+#  'mySUNI-WorkShop-국민연금 데이터 분석(해설).ipynb',
+#  'mySUNI-WorkShop-민간 아파트 가격동향 분석(해설).ipynb',
+#  'mySUNI-WorkShop-아파트 실거래가 분석 I(해설).ipynb',
+#  'mySUNI-WorkShop-아파트 실거래가 분석 II(해설).ipynb',
+#  'mySUNI-WorkShop-유가 가격 분석 (해설).ipynb',
+#  'mySUNI-WorkShop-중고차 판매 정보 분석 (해설).ipynb'],
+#  'mySUNI-WorkShop-06-웨이퍼 불량 유형 분류':['mySUNI-WorkShop-06-웨이퍼 불량 유형 분류-해설.ipynb'],
+#  'mySUNI-WorkShop-07-따릉이 대여량 예측':['mySUNI-WorkShop-07-따릉이 대여량 예측-해설.ipynb'],
+#  'mySUNI-WorkShop-08-집 값 예측':['mySUNI-WorkShop-08-집 값 예측-해설.ipynb'],
+#  'mySUNI-WorkShop-09-머신러닝 연습':['mySUNI-WorkShop-빌딩 전력 소모량 예측 (해설).ipynb',
+#   'mySUNI-WorkShop-사용자 이탈 예측 (해설).ipynb',
+#   'mySUNI-WorkShop-에너지 효율 예측 (해설).ipynb',
+#   'mySUNI-WorkShop-와인 유형 분류 (해설).ipynb']}
+
+r = requests.get(WORKSHOP_DOWNLOAD_URL)
+open(WORKSHOP_DATA_PATH, 'wb').write(r.content)
+
+with open(WORKSHOP_DATA_PATH) as f:
+    workshops = json.load(f)
+    
+q = workshops['q']
+s = workshops['s']
+
+def list_workshop():
+    workshop = pd.DataFrame({
+        '워크샵':q.keys(),
+    })
+    display(workshop.sort_values('워크샵'))
+
+def download_workshop(workshop_name, sol=False, local=False):
+    # auth
+    username = 'mysuni'
+    password = 'mysuni1!'
+
+    if local:
+        if not os.path.exists(os.path.join('workshop', f'{workshop_name}')):
+            os.makedirs(os.path.join('workshop', f'{workshop_name}'))
+
+    else:
+        if not os.path.exists(os.path.join('/mnt/elice', 'workshop', f'{workshop_name}')):
+            os.makedirs(os.path.join('/mnt/elice', 'workshop', f'{workshop_name}'))
+
+    if sol:
+        workshop_files = s[workshop_name]
+    else:
+        workshop_files = q[workshop_name]
+
+    print(f'워크샵: {workshop_files}\n==============================\n파일 정보\n')
+    for workshop_file in workshop_files:
+        fileurl = "http://sk.jaen.kr:8080/workshop/" + workshop_file
+        r = requests.get(fileurl, auth=HTTPBasicAuth(username, password))
+        if local:
+            filepath = os.path.join('workshop', f'{workshop_name}', workshop_file)
+        else:
+            filepath = os.path.join('/mnt/elice','workshop', f'{workshop_name}', workshop_file)
+
+        if os.path.exists(filepath):
+            file = filepath.split('.')
+            now = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
+            file[0] = file[0] + now
+            filepath = ".".join(file)
+        open(filepath, 'wb').write(r.content)
+        print(f'저장 위치:\t {filepath}')
+    print(f'\n==============================')
+
+
+####### 프로젝트 관련 모듈 #######
+
+project = None
+
+
+class Project:
+    def __init__(self, project_name, class_info, email, server='manage'):
+        self.project_name = project_name
+        self.edu_name = "mySUNI"
+        self.edu_rnd = class_info.split()[0]
+        self.edu_class = class_info.split()[1]
+        self.email = email
+        self.server = server
+
+        r = requests.get(PROJECT_DOWNLOAD_URL)
+        open(PROJECT_DATA_PATH, 'wb').write(r.content)
+
+    def __make_submission(self, submission):
+        timestring = datetime.datetime.now().strftime('%H-%M-%S')
+        filename = 'submission-{}.csv'.format(timestring)
+        submission.to_csv(filename, index=False)
+        print('파일을 저장하였습니다. 파일명: {}'.format(filename))
+        return filename
+
+    def __project_submission(self, file_name):
+        file_path = './'
+        url = f'http://{self.server}.jaen.kr/api/studentProject/apiScoring?edu_name={self.edu_name}\
+        &edu_rnd={self.edu_rnd}&edu_class={self.edu_class}&mail={self.email}&project_name={self.project_name}&file_name={file_name}'
+        files = {'file': (file_name, open(file_path + file_name, 'rb'), 'text/csv')}
+        r = requests.post(url, files=files)
+        r.encoding = 'utf-8'
+        message = ''
+        try:
+            data = json.loads(r.text) # json 변환 실패시 원본 메세지 사용
+            if 'trial' in data.keys():
+                message = '제출 여부 :{}\n오늘 제출 횟수 : {}\n제출 결과:{}'.format(data['msg'], data['trial'], data['score'])
+            else:
+                message = '제출 실패 : {}'.format(data['msg'])
+        except:
+            message = '변환 에러 발생 : {}'.format(r.text)
+        return message
+
+    def project_final_submission(self, name, ipynb_file_path=None):
+        url = "http://sk.jaen.kr/submission_final"
+        files = []
+        if ipynb_file_path is None:
+            raise Exception('노트북(ipynb) 파일의 경로를 입력해 주세요.') 
+        files.append(('file', open(ipynb_file_path, 'rb')))
+        data = {'name': name, 'rnd':self.edu_rnd, 'class':self.edu_class}
+        res = requests.post(url, data=data, files=files)
+        print(res.text)
+
+    def submit(self, submission):
+        filename = self.__make_submission(submission)
+        print(self.__project_submission(filename))
+
+
+def download_project(project_name, class_info, email, use_path=None, skip_download=False, server='manage'):
+    '''
+    use_path: 지정 폴더에 다운로드
+    skip_download: 폴더에 데이터가 존재할 시 SKIP. 단 CHECKSUM 비교는 안함.
+    '''
+    global project, files
+    try:
+        project = Project(project_name, class_info=class_info, email=email, server=server)
+
+        # data 폴더 경로 지정
+        DATA_DIR = 'data'
+        if use_path is not None:
+            DATA_DIR = use_path
+
+        with open(PROJECT_DATA_PATH) as f:
+            datasets = json.load(f)
+
+        # data 폴더 생성
+        if not os.path.exists(os.path.join(DATA_DIR, project_name)):
+            os.makedirs(os.path.join(DATA_DIR, project_name))
+
+        project_files = datasets[project_name]
+
+        # skip download 체크
+        file_to_remove = []
+        if skip_download:
+            for filename, _ in project_files.items():
+                filepath = os.path.join(DATA_DIR, project_name, filename)
+                if os.path.exists(filepath):
+                    file_to_remove.append(filename)
+                    print(f'{filename} 파일이 {filepath} 이미 존재하여 다운로드를 SKIP 합니다..')
+
+        print(f'카운트 다운!')
+        time_cnt = 1
+        while time_cnt <= 3:
+            print(f'{time_cnt}', end=' ')
+            time.sleep(1)
+            time_cnt += 1
+        clear_output(wait=True)
+
+        for k in file_to_remove:
+            project_files.pop(k)
+
+        # auth
+        username = 'mysuni'
+        password = 'mysuni1!'
+
+        print(f'프로젝트: {project_name}\n==============================\n파일 다운로드\n')
+        for filename, fileurl in project_files.items():
+            r = requests.get(fileurl, auth=HTTPBasicAuth(username, password), stream=True)
+
+            filepath = os.path.join(DATA_DIR, project_name, filename)
+            print(f'{filename}', end=' ')
+
+            ## 다운로드 progress bar 추가 ##
+            total_size_in_bytes = int(r.headers.get('content-length', 0))
+            block_size = 1024
+
+            progress_bar = tqdm(total=total_size_in_bytes, unit='B', unit_scale=True)
+            with open(filepath, 'wb') as file:
+                for data in r.iter_content(block_size):
+                    progress_bar.update(len(data))
+                    file.write(data)
+            progress_bar.close()
+            if total_size_in_bytes != 0 and progress_bar.n != total_size_in_bytes:
+                print("ERROR: 다운로드 도중 에러가 발생하였습니다.")
+            else:
+                if filepath.endswith('.zip'):
+                    print(f'압축 해제 및 프로젝트 파일 구성중...')
+                    zipfile.ZipFile(filepath).extractall(os.path.join(DATA_DIR, project_name))
+            ## 다운로드 progress bar 추가 ##
+        clear_output(wait=True)
+        print(f'\n==============================')
+        print(f'프로젝트: {project_name}\n==============================\n파일 목록\n')
+        for f in [fs for fs in os.listdir(os.path.join('data', project_name)) if 'csv' in fs]:
+            print(f'{f}\n- {os.path.join(DATA_DIR, project_name, f)}\n')
+        print(f'==============================')
+    except Exception as err:
+        print(err)
+        raise Exception('잘못된 정보입니다.')
+
+
+def submit(submission_file):
+    global project
+    project.submit(submission_file)
+
+
+def end_project(name, ipynb_file_path):
+    global project
+    project.project_final_submission(name, ipynb_file_path)
+
+def update_project(project_name=None, class_info=None, email=None):
+    global project
+    if project_name:
+        project.project_name = project_name
+    if project.class_info:
+        project.class_info = class_info
+    if project.email:
+        project.email = email
+    print('정보 업데이트 완료')
```

## mySUNI/utils.py

 * *Ordering differences only*

```diff
@@ -1,458 +1,458 @@
-import codecs
-import json
-import os
-
-# 코드 입력 문구 (코드를 삭제하고 출력을 박제하는 Cell)
-code_input_msgs = [
-    '# 코드입력',
-    '# 코드를 입력하세요.',
-    '# 코드를 입력해 주세요',
-]
-
-# 검증코드 (출력 값을 삭제하지 않음)
-validation_msgs =  [
-    '# 검증코드',
-    '# 코드 검증',
-    '# 코드검증',
-]
-
-
-def convert_ipynb(from_file, to_file=None, folder_path=None, post_fix='-변환.ipynb'):
-    """
-    from_file: 읽어 올 해설 파일 이름
-    to_file: 변환 후 내보낼 파일 명, None
-    folder_path: 기본 값 None. None이 아니면 해당 폴더경로에 생성
-    post_fix: 파일 뒤에 붙혀줌. 그대로 두면 -변환 이라고 postfix 가 붙어서 자동 생성
-    
-    (예시)
-    - 폴더 지정 안하는 경우, 같은 경로에 생성
-    convert_ipynb(filename)
-    - 폴더 지정시 해당 경로의 폴더에 생성
-    convert_ipynb(filename, folder_path='00-Workshop/변환')
-    - 아무 post_fix 없이 생성
-    convert_ipynb(filename, folder_path='00-Workshop/변환', post_fix='.ipynb')
-    """
-    try:
-        f = codecs.open(from_file, 'r')
-        source = f.read()
-    except UnicodeDecodeError:
-        f = codecs.open(from_file, 'r', encoding='utf-8')
-        source = f.read()
-    except Exception as e:
-        raise Exception("파일 변환에 실패 했습니다. 에러 메세지:" + e)
-
-    y = json.loads(source)
-
-    idx = []
-    sources = []
-
-    for i, x in enumerate(y['cells']):
-        flag = False
-        valid_flag = False
-        for x2 in x['source']:
-            for msg in code_input_msgs:
-                if msg in x2:
-                    flag = True
-                    break
-
-            for valid_msg in validation_msgs:
-                if valid_msg in x2:
-                    valid_flag = True
-                    break
-
-        if flag:
-            new_text = []
-            for x2 in x['source']:
-                if x2.startswith('#'):
-                    new_text.append(x2)
-            x['source'] = new_text
-
-        if 'outputs' in x.keys():
-            if not flag and not valid_flag:
-                x['outputs'] = []  
-            elif len(x['outputs']) > 0:
-                for outputs in x['outputs']:
-                    if 'data' in outputs.keys():
-                        clear_flag = False
-                        for key, value in outputs.items():
-                            if type(value) == dict and len(value) > 0:
-                                add_cnt = 0
-                                for key2 in value.keys():
-                                    if 'text/html' == key2:
-                                        idx.append(i + add_cnt)
-                                        html_text = value['text/html']
-                                        html_text.insert(0, '<p><strong>[출력 결과]</strong></p>')
-                                        sources.append(html_text)
-                                        clear_flag = True
-                                        break
-                                    elif 'text/plain' == key2:
-                                        idx.append(i + add_cnt)
-                                        plain_text = value['text/plain']
-                                        plain_text[0] = '<pre>' + plain_text[0]
-                                        plain_text[len(plain_text)-1] = plain_text[len(plain_text)-1] + '</pre>'
-                                        plain_text.insert(0, '<p><strong>[출력 결과]</strong></p>')
-                                        sources.append(plain_text)
-                                        clear_flag = True
-                                        add_cnt += 1
-                                    elif 'image/png' == key2:
-                                        idx.append(i + add_cnt)
-                                        plain_image = value['image/png']
-                                        plain_image = '<img src="data:image/png;base64,' + plain_image.replace('\n','') + '"/>'
-                                        sources.append(plain_image)
-                                        clear_flag = True
-                                        add_cnt += 1
-                        if clear_flag:
-                            x['outputs'] = []
-
-                if len(x['outputs']) > 0 and 'text' in x['outputs'][0].keys():
-                    idx.append(i)
-                    text = x['outputs'][0]['text']
-                    
-                    if len(text) > 0:
-                        text[0] = '<pre>' + text[0]
-                        text[len(text) - 1] = text[len(text) - 1] + '</pre>'
-                        text.insert(0, '<p><strong>[출력 결과]</strong></p>')
-                    sources.append(text)
-                    x['outputs'][0]['text'] = []
-
-        if 'execution_count' in x.keys():
-            x['execution_count'] = None
-
-    cnt = 0
-    tmp = []
-    for i, s in zip(idx, sources):
-        v = {'cell_type': 'markdown',
-             'metadata': {},
-             'source': s}
-        tmp.append((i + 1 + cnt, v))
-        cnt += 1
-
-    for i in range(len(tmp)):
-        y['cells'].insert(tmp[i][0], tmp[i][1])
-
-    if to_file is None:
-        if '해설' in from_file:
-            to_file = from_file.replace('해설', '실습')
-            to_file = to_file[:-6] + post_fix
-        else:
-            to_file = from_file[:-6] + post_fix
-
-    if folder_path is not None:
-        # 폴더 경로 없으면 생성
-        if not os.path.isdir(folder_path):
-            os.mkdir(folder_path)
-        # 폴더 경로를 포함한 파일 경로 생성
-        to_file = os.path.join(folder_path, os.path.basename(to_file))
-
-    with open(to_file, "w") as json_file:
-        json.dump(y, json_file)
-    print('생성완료')
-    print(f'파일명: {to_file}')
-    
-
-# folder_path: 변환할 폴더 경로
-# new_folder_name: 기본값은 /자동변환. 새로 생성할 폴더명
-def convert_ipynb_folder(folder_path, new_folder_name='변환', post_fix='-변환.ipynb'):
-    """
-    folder_path: 변환할 폴더 경로
-    new_folder_name: 기본값은 /자동변환. 새로 생성할 폴더명
-    
-    (예시)
-    convert_ipynb_folder(folder_path, new_folder_name='실습폴더', post_fix='.ipynb')
-    
-    변환 (post_fix 적용)
-    convert_ipynb_folder(folder_path, post_fix='-자동변환.ipynb')
-    """
-    new_folder_path = os.path.join(folder_path, new_folder_name)
-    
-    if not os.path.isdir(new_folder_path):
-        os.mkdir(new_folder_path)
-
-    ipynb_list = [os.path.join(folder_path, f) for f in os.listdir(folder_path) if f.endswith('ipynb')]
-
-    for file in ipynb_list:
-        convert_ipynb(file, folder_path=new_folder_path, post_fix=post_fix)
-
-### Util 함수
-import matplotlib.pyplot as plt
-import seaborn as sns
-import numpy as np
-import pandas as pd
-from sklearn.metrics import mean_squared_error, mean_squared_log_error, mean_absolute_error
-
-
-class ModelPlot():
-    def __init__(self, error='mse', figsize=(15, 10)):
-        self.my_predictions = {}
-
-        self.figsize = figsize
-        self.font_big = 15
-        self.font_small = 12
-        self.graph_width = 10
-        self.round = 5
-        self.error_name, self.error = self.set_error(error)
-
-        self.colors = ['r', 'c', 'm', 'y', 'k', 'khaki', 'teal', 'orchid', 'sandybrown',
-                       'greenyellow', 'dodgerblue', 'deepskyblue', 'rosybrown', 'firebrick',
-                       'deeppink', 'crimson', 'salmon', 'darkred', 'olivedrab', 'olive',
-                       'forestgreen', 'royalblue', 'indigo', 'navy', 'mediumpurple', 'chocolate',
-                       'gold', 'darkorange', 'seagreen', 'turquoise', 'steelblue', 'slategray',
-                       'peru', 'midnightblue', 'slateblue', 'dimgray', 'cadetblue', 'tomato'
-                       ]
-
-    def set_plot_options(self, figsize=(15, 10), font_big=15, font_small=12, graph_width=10, round=5):
-        self.figsize = figsize
-        self.font_big = font_big
-        self.font_small = font_small
-        self.graph_width = graph_width
-        self.round = round
-
-    def set_error(self, error='mse'):
-        if error == 'mse':
-            self.error = mean_squared_error
-            self.error_name = 'mse'
-            return error, self.error
-        elif error == 'rmse':
-            def rmse(y_true, y_pred):
-                return np.sqrt(mean_squared_error(y_true, y_pred))
-            self.error = rmse
-            self.error_name = 'rmse'
-            return error, self.error
-
-        elif error == 'rmsle':
-            def rmsle(y_true, y_pred):
-                return np.sqrt(mean_squared_log_error(y_true, y_pred))
-            self.error = rmsle
-            self.error_name = 'rmsle'
-            return error, self.error
-        elif error == 'mae':
-            self.error = mean_absolute_error
-            self.error_name = 'mae'
-            return error, self.error
-        else:
-            self.error = mean_squared_error
-            self.error_name = 'mse'
-            return 'mse', mean_squared_error
-
-    def plot_predictions(self, name_, actual, pred):
-        df = pd.DataFrame({'prediction': pred, 'actual': actual})
-        df = df.sort_values(by='actual').reset_index(drop=True)
-
-        plt.figure(figsize=self.figsize)
-        plt.scatter(df.index, df['prediction'], marker='x', color='r')
-        plt.scatter(df.index, df['actual'], alpha=0.7, marker='o', color='black')
-        plt.title(name_, fontsize=self.font_big)
-        plt.legend(['prediction', 'actual'], fontsize=self.font_small)
-        plt.show()
-
-    def plot_error(self, name_, actual, pred):
-        pred = np.asarray(pred).reshape(-1)
-        actual = np.asarray(actual).reshape(-1)
-
-        self.plot_predictions(name_, actual, pred)
-
-        err = self.error(actual, pred)
-        self.my_predictions[name_] = err
-
-        y_value = sorted(self.my_predictions.items(), key=lambda x: x[1], reverse=True)
-
-        df = pd.DataFrame(y_value, columns=['model', 'error'])
-
-        print(df)
-
-        min_ = max(df['error'].min() - 10, 0)
-        max_ = df['error'].max()
-        diff = (max_ - min_)
-        max_ += diff * 0.25
-        offset = diff * 0.05
-
-        length = len(df) / 2
-
-        fig, ax = plt.subplots(1, 1)
-        fig.set_size_inches(self.graph_width, length)
-        ax.set_yticks(np.arange(len(df)))
-        ax.set_yticklabels(df['model'], fontsize=self.font_small)
-
-        bars = ax.barh(np.arange(len(df)), df['error'], height=0.3)
-
-        for i, v in enumerate(df['error']):
-            idx = np.random.choice(len(self.colors))
-            bars[i].set_color(self.colors[idx])
-            ax.text(v + offset, i, str(round(v, self.round)), color='k', fontsize=self.font_small, fontweight='bold',
-                    verticalalignment='center')
-
-        ax.set_title(f'{self.error_name.upper()} Error', fontsize=self.font_big)
-        ax.set_xlim(min_, max_)
-
-        plt.show()
-
-    def plot_all(self):
-        y_value = sorted(self.my_predictions.items(), key=lambda x: x[1], reverse=True)
-
-        df = pd.DataFrame(y_value, columns=['model', 'error'])
-
-        print(df)
-
-        min_ = max(df['error'].min() - 10, 0)
-        max_ = df['error'].max()
-        diff = (max_ - min_)
-        max_ += diff * 0.25
-        offset = diff * 0.05
-
-        length = len(df) / 2
-
-        fig, ax = plt.subplots(1, 1)
-        fig.set_size_inches(self.graph_width, length)
-        ax.set_yticks(np.arange(len(df)))
-        ax.set_yticklabels(df['model'], fontsize=self.font_small)
-
-        bars = ax.barh(np.arange(len(df)), df['error'], height=0.3)
-
-        for i, v in enumerate(df['error']):
-            idx = np.random.choice(len(self.colors))
-            bars[i].set_color(self.colors[idx])
-            ax.text(v + offset, i, str(round(v, self.round)), color='k', fontsize=self.font_small, fontweight='bold',
-                    verticalalignment='center')
-
-        ax.set_title(f'{self.error_name.upper()} Error', fontsize=self.font_big)
-        ax.set_xlim(min_, max_)
-
-        plt.show()
-
-    def add_model(self, name_, actual, pred):
-        err = self.error(actual, pred)
-        self.my_predictions[name_] = err
-
-    def remove_model(self, name_):
-        if name_ in self.my_predictions:
-            self.my_predictions.pop(name_)
-        else:
-            print('(에러) 지정한 키 값으로 등록된 모델이 없습니다.')
-
-    def clear_error(self):
-        self.my_predictions.clear()
-
-
-plot = ModelPlot(error='mse')
-
-
-def set_plot_error(error='mse'):
-    global plot
-    '''
-    error: 'mse', 'rmse', 'rmsle', 'mae'
-    '''
-    plot.set_error(error)
-
-
-def plot_error(name_, actual, prediction):
-    global plot
-    plot.plot_error(name_, actual, prediction)
-
-
-def plot_all():
-    global plot
-    plot.plot_all()
-
-
-def remove_error(name_):
-    global plot
-    plot.remove_model(name_)
-
-
-def add_error(name_, actual, prediction):
-    global plot
-    plot.add_model(name_, actual, prediction)
-
-
-def clear_error():
-    global plot
-    plot.clear_error()
-
-
-def set_plot_options(figsize=(15, 10), font_big=15, font_small=12, graph_width=10, round=5):
-    global plot
-    plot.set_plot_options(figsize=figsize, font_big=font_big, font_small=font_small, graph_width=graph_width, round=round)
-
-def summary(df):
-    print(f'데이터 프레임 형태(shape) : {df.shape}')
-    s = pd.DataFrame(df.dtypes, columns=['데이터 타입'])
-    s['최소값'] = df.min()
-    s['최대값'] = df.max()
-    s = s.reset_index()
-    s = s.rename(columns={'index':'특성명'})
-    s['결측치 개수'] = df.isna().sum().values
-    s['고유값 개수'] = df.nunique().values
-    s['고유값'] = [df[col_name].unique() for col_name in df.columns]
-    return s
-
-
-from sklearn.metrics import mean_squared_log_error
-def rmsle(true, pred):
-    return np.sqrt(mean_squared_log_error(true, pred)) 
-
-def gini(y_true, y_pred):
-    # 실제값과 예측값의 크기가 같은지 확인 (값이 다르면 오류 발생)
-    if y_true.shape != y_pred.shape:
-        raise Exception('Shape Error : 실제값과 예측값의 개수가 일치하지 않습니다.')
-
-    n_samples = y_true.shape[0]                      # 데이터 개수
-    L_mid = np.linspace(1 / n_samples, 1, n_samples) # 대각선 값
-
-    # 1) 예측값에 대한 지니계수
-    pred_order = y_true[y_pred.argsort()] # y_pred 크기순으로 y_true 값 정렬
-    L_pred = np.cumsum(pred_order) / np.sum(pred_order) # 로렌츠 곡선
-    G_pred = np.sum(L_mid - L_pred)       # 예측 값에 대한 지니계수
-
-    # 2) 예측이 완벽할 때 지니계수
-    true_order = y_true[y_true.argsort()] # y_true 크기순으로 y_true 값 정렬
-    L_true = np.cumsum(true_order) / np.sum(true_order) # 로렌츠 곡선
-    G_true = np.sum(L_mid - L_true)       # 예측이 완벽할 때 지니계수
-
-    # 정규화된 지니계수
-    return G_pred / G_true  
-    
-########## 에러 메시지 ############
-
-class ErrorChecker():
-    def __init__(self, test_size=None, evaluation='mse'):
-        self.test_size = test_size
-        self.evaluation = evaluation
-    
-    def check_error(self, pred):
-        """
-        error_code
-        1: 음수 값 제출시 에러
-        2: test셋의 length와 맞지 않음
-        """
-        msg = "[통과] 문제가 발견되지 않았습니다."
-        try:
-            if (self.evaluation == 'rmsle') and (pred[pred < 0].size > 0):
-                msg = "[오류]\n\n예측 값에(prediction) 음수 값이 있습니다!!\n\n대여량은 음수 값을 가질 수 없으므로 음수 값을 포함하는 정답은 제출이 불가합니다.\n\n음수값 확인 방법(코드):\n\nprediction[prediction < 0]"
-            elif (self.test_size) and len(pred) != self.test_size:
-                msg = f"[오류] \n\n예측 값인 prediction의 길이가 {self.test_size}개 이어야 합니다.\n\nlen(prediction) 의 값이 {self.test_size}개가 나오지 않는다면 제출이 불가 합니다.\n\n(test 세트로 예측했는지 확인해 주세요)"
-        except Exception as err:
-            msg = f'[오류] {err}'
-        print(msg)
-    
-    def set_values(self,  test_size=None, evaluation=None):
-        if test_size is not None:
-            self.test_size = test_size
-        if evaluation is not None:
-            self.evaluation = evaluation
-    
-    def get_values(self):
-        print(f'test case: {self.test_size}\nevaluation: {self.evaluation}')
-
-err_checker = ErrorChecker(test_size=6493, evaluation='rmsle')
-
-def check_error(prediction):
-    global err_checker
-    err_checker.check_error(prediction)
-
-def set_error_values(test_size=None, evaluation=None):
-    global err_checker
-    err_checker.set_values(test_size=test_size, evaluation=evaluation)
-
-
-
-
+import codecs
+import json
+import os
+
+# 코드 입력 문구 (코드를 삭제하고 출력을 박제하는 Cell)
+code_input_msgs = [
+    '# 코드입력',
+    '# 코드를 입력하세요.',
+    '# 코드를 입력해 주세요',
+]
+
+# 검증코드 (출력 값을 삭제하지 않음)
+validation_msgs =  [
+    '# 검증코드',
+    '# 코드 검증',
+    '# 코드검증',
+]
+
+
+def convert_ipynb(from_file, to_file=None, folder_path=None, post_fix='-변환.ipynb'):
+    """
+    from_file: 읽어 올 해설 파일 이름
+    to_file: 변환 후 내보낼 파일 명, None
+    folder_path: 기본 값 None. None이 아니면 해당 폴더경로에 생성
+    post_fix: 파일 뒤에 붙혀줌. 그대로 두면 -변환 이라고 postfix 가 붙어서 자동 생성
+    
+    (예시)
+    - 폴더 지정 안하는 경우, 같은 경로에 생성
+    convert_ipynb(filename)
+    - 폴더 지정시 해당 경로의 폴더에 생성
+    convert_ipynb(filename, folder_path='00-Workshop/변환')
+    - 아무 post_fix 없이 생성
+    convert_ipynb(filename, folder_path='00-Workshop/변환', post_fix='.ipynb')
+    """
+    try:
+        f = codecs.open(from_file, 'r')
+        source = f.read()
+    except UnicodeDecodeError:
+        f = codecs.open(from_file, 'r', encoding='utf-8')
+        source = f.read()
+    except Exception as e:
+        raise Exception("파일 변환에 실패 했습니다. 에러 메세지:" + e)
+
+    y = json.loads(source)
+
+    idx = []
+    sources = []
+
+    for i, x in enumerate(y['cells']):
+        flag = False
+        valid_flag = False
+        for x2 in x['source']:
+            for msg in code_input_msgs:
+                if msg in x2:
+                    flag = True
+                    break
+
+            for valid_msg in validation_msgs:
+                if valid_msg in x2:
+                    valid_flag = True
+                    break
+
+        if flag:
+            new_text = []
+            for x2 in x['source']:
+                if x2.startswith('#'):
+                    new_text.append(x2)
+            x['source'] = new_text
+
+        if 'outputs' in x.keys():
+            if not flag and not valid_flag:
+                x['outputs'] = []  
+            elif len(x['outputs']) > 0:
+                for outputs in x['outputs']:
+                    if 'data' in outputs.keys():
+                        clear_flag = False
+                        for key, value in outputs.items():
+                            if type(value) == dict and len(value) > 0:
+                                add_cnt = 0
+                                for key2 in value.keys():
+                                    if 'text/html' == key2:
+                                        idx.append(i + add_cnt)
+                                        html_text = value['text/html']
+                                        html_text.insert(0, '<p><strong>[출력 결과]</strong></p>')
+                                        sources.append(html_text)
+                                        clear_flag = True
+                                        break
+                                    elif 'text/plain' == key2:
+                                        idx.append(i + add_cnt)
+                                        plain_text = value['text/plain']
+                                        plain_text[0] = '<pre>' + plain_text[0]
+                                        plain_text[len(plain_text)-1] = plain_text[len(plain_text)-1] + '</pre>'
+                                        plain_text.insert(0, '<p><strong>[출력 결과]</strong></p>')
+                                        sources.append(plain_text)
+                                        clear_flag = True
+                                        add_cnt += 1
+                                    elif 'image/png' == key2:
+                                        idx.append(i + add_cnt)
+                                        plain_image = value['image/png']
+                                        plain_image = '<img src="data:image/png;base64,' + plain_image.replace('\n','') + '"/>'
+                                        sources.append(plain_image)
+                                        clear_flag = True
+                                        add_cnt += 1
+                        if clear_flag:
+                            x['outputs'] = []
+
+                if len(x['outputs']) > 0 and 'text' in x['outputs'][0].keys():
+                    idx.append(i)
+                    text = x['outputs'][0]['text']
+                    
+                    if len(text) > 0:
+                        text[0] = '<pre>' + text[0]
+                        text[len(text) - 1] = text[len(text) - 1] + '</pre>'
+                        text.insert(0, '<p><strong>[출력 결과]</strong></p>')
+                    sources.append(text)
+                    x['outputs'][0]['text'] = []
+
+        if 'execution_count' in x.keys():
+            x['execution_count'] = None
+
+    cnt = 0
+    tmp = []
+    for i, s in zip(idx, sources):
+        v = {'cell_type': 'markdown',
+             'metadata': {},
+             'source': s}
+        tmp.append((i + 1 + cnt, v))
+        cnt += 1
+
+    for i in range(len(tmp)):
+        y['cells'].insert(tmp[i][0], tmp[i][1])
+
+    if to_file is None:
+        if '해설' in from_file:
+            to_file = from_file.replace('해설', '실습')
+            to_file = to_file[:-6] + post_fix
+        else:
+            to_file = from_file[:-6] + post_fix
+
+    if folder_path is not None:
+        # 폴더 경로 없으면 생성
+        if not os.path.isdir(folder_path):
+            os.mkdir(folder_path)
+        # 폴더 경로를 포함한 파일 경로 생성
+        to_file = os.path.join(folder_path, os.path.basename(to_file))
+
+    with open(to_file, "w") as json_file:
+        json.dump(y, json_file)
+    print('생성완료')
+    print(f'파일명: {to_file}')
+    
+
+# folder_path: 변환할 폴더 경로
+# new_folder_name: 기본값은 /자동변환. 새로 생성할 폴더명
+def convert_ipynb_folder(folder_path, new_folder_name='변환', post_fix='-변환.ipynb'):
+    """
+    folder_path: 변환할 폴더 경로
+    new_folder_name: 기본값은 /자동변환. 새로 생성할 폴더명
+    
+    (예시)
+    convert_ipynb_folder(folder_path, new_folder_name='실습폴더', post_fix='.ipynb')
+    
+    변환 (post_fix 적용)
+    convert_ipynb_folder(folder_path, post_fix='-자동변환.ipynb')
+    """
+    new_folder_path = os.path.join(folder_path, new_folder_name)
+    
+    if not os.path.isdir(new_folder_path):
+        os.mkdir(new_folder_path)
+
+    ipynb_list = [os.path.join(folder_path, f) for f in os.listdir(folder_path) if f.endswith('ipynb')]
+
+    for file in ipynb_list:
+        convert_ipynb(file, folder_path=new_folder_path, post_fix=post_fix)
+
+### Util 함수
+import matplotlib.pyplot as plt
+import seaborn as sns
+import numpy as np
+import pandas as pd
+from sklearn.metrics import mean_squared_error, mean_squared_log_error, mean_absolute_error
+
+
+class ModelPlot():
+    def __init__(self, error='mse', figsize=(15, 10)):
+        self.my_predictions = {}
+
+        self.figsize = figsize
+        self.font_big = 15
+        self.font_small = 12
+        self.graph_width = 10
+        self.round = 5
+        self.error_name, self.error = self.set_error(error)
+
+        self.colors = ['r', 'c', 'm', 'y', 'k', 'khaki', 'teal', 'orchid', 'sandybrown',
+                       'greenyellow', 'dodgerblue', 'deepskyblue', 'rosybrown', 'firebrick',
+                       'deeppink', 'crimson', 'salmon', 'darkred', 'olivedrab', 'olive',
+                       'forestgreen', 'royalblue', 'indigo', 'navy', 'mediumpurple', 'chocolate',
+                       'gold', 'darkorange', 'seagreen', 'turquoise', 'steelblue', 'slategray',
+                       'peru', 'midnightblue', 'slateblue', 'dimgray', 'cadetblue', 'tomato'
+                       ]
+
+    def set_plot_options(self, figsize=(15, 10), font_big=15, font_small=12, graph_width=10, round=5):
+        self.figsize = figsize
+        self.font_big = font_big
+        self.font_small = font_small
+        self.graph_width = graph_width
+        self.round = round
+
+    def set_error(self, error='mse'):
+        if error == 'mse':
+            self.error = mean_squared_error
+            self.error_name = 'mse'
+            return error, self.error
+        elif error == 'rmse':
+            def rmse(y_true, y_pred):
+                return np.sqrt(mean_squared_error(y_true, y_pred))
+            self.error = rmse
+            self.error_name = 'rmse'
+            return error, self.error
+
+        elif error == 'rmsle':
+            def rmsle(y_true, y_pred):
+                return np.sqrt(mean_squared_log_error(y_true, y_pred))
+            self.error = rmsle
+            self.error_name = 'rmsle'
+            return error, self.error
+        elif error == 'mae':
+            self.error = mean_absolute_error
+            self.error_name = 'mae'
+            return error, self.error
+        else:
+            self.error = mean_squared_error
+            self.error_name = 'mse'
+            return 'mse', mean_squared_error
+
+    def plot_predictions(self, name_, actual, pred):
+        df = pd.DataFrame({'prediction': pred, 'actual': actual})
+        df = df.sort_values(by='actual').reset_index(drop=True)
+
+        plt.figure(figsize=self.figsize)
+        plt.scatter(df.index, df['prediction'], marker='x', color='r')
+        plt.scatter(df.index, df['actual'], alpha=0.7, marker='o', color='black')
+        plt.title(name_, fontsize=self.font_big)
+        plt.legend(['prediction', 'actual'], fontsize=self.font_small)
+        plt.show()
+
+    def plot_error(self, name_, actual, pred):
+        pred = np.asarray(pred).reshape(-1)
+        actual = np.asarray(actual).reshape(-1)
+
+        self.plot_predictions(name_, actual, pred)
+
+        err = self.error(actual, pred)
+        self.my_predictions[name_] = err
+
+        y_value = sorted(self.my_predictions.items(), key=lambda x: x[1], reverse=True)
+
+        df = pd.DataFrame(y_value, columns=['model', 'error'])
+
+        print(df)
+
+        min_ = max(df['error'].min() - 10, 0)
+        max_ = df['error'].max()
+        diff = (max_ - min_)
+        max_ += diff * 0.25
+        offset = diff * 0.05
+
+        length = len(df) / 2
+
+        fig, ax = plt.subplots(1, 1)
+        fig.set_size_inches(self.graph_width, length)
+        ax.set_yticks(np.arange(len(df)))
+        ax.set_yticklabels(df['model'], fontsize=self.font_small)
+
+        bars = ax.barh(np.arange(len(df)), df['error'], height=0.3)
+
+        for i, v in enumerate(df['error']):
+            idx = np.random.choice(len(self.colors))
+            bars[i].set_color(self.colors[idx])
+            ax.text(v + offset, i, str(round(v, self.round)), color='k', fontsize=self.font_small, fontweight='bold',
+                    verticalalignment='center')
+
+        ax.set_title(f'{self.error_name.upper()} Error', fontsize=self.font_big)
+        ax.set_xlim(min_, max_)
+
+        plt.show()
+
+    def plot_all(self):
+        y_value = sorted(self.my_predictions.items(), key=lambda x: x[1], reverse=True)
+
+        df = pd.DataFrame(y_value, columns=['model', 'error'])
+
+        print(df)
+
+        min_ = max(df['error'].min() - 10, 0)
+        max_ = df['error'].max()
+        diff = (max_ - min_)
+        max_ += diff * 0.25
+        offset = diff * 0.05
+
+        length = len(df) / 2
+
+        fig, ax = plt.subplots(1, 1)
+        fig.set_size_inches(self.graph_width, length)
+        ax.set_yticks(np.arange(len(df)))
+        ax.set_yticklabels(df['model'], fontsize=self.font_small)
+
+        bars = ax.barh(np.arange(len(df)), df['error'], height=0.3)
+
+        for i, v in enumerate(df['error']):
+            idx = np.random.choice(len(self.colors))
+            bars[i].set_color(self.colors[idx])
+            ax.text(v + offset, i, str(round(v, self.round)), color='k', fontsize=self.font_small, fontweight='bold',
+                    verticalalignment='center')
+
+        ax.set_title(f'{self.error_name.upper()} Error', fontsize=self.font_big)
+        ax.set_xlim(min_, max_)
+
+        plt.show()
+
+    def add_model(self, name_, actual, pred):
+        err = self.error(actual, pred)
+        self.my_predictions[name_] = err
+
+    def remove_model(self, name_):
+        if name_ in self.my_predictions:
+            self.my_predictions.pop(name_)
+        else:
+            print('(에러) 지정한 키 값으로 등록된 모델이 없습니다.')
+
+    def clear_error(self):
+        self.my_predictions.clear()
+
+
+plot = ModelPlot(error='mse')
+
+
+def set_plot_error(error='mse'):
+    global plot
+    '''
+    error: 'mse', 'rmse', 'rmsle', 'mae'
+    '''
+    plot.set_error(error)
+
+
+def plot_error(name_, actual, prediction):
+    global plot
+    plot.plot_error(name_, actual, prediction)
+
+
+def plot_all():
+    global plot
+    plot.plot_all()
+
+
+def remove_error(name_):
+    global plot
+    plot.remove_model(name_)
+
+
+def add_error(name_, actual, prediction):
+    global plot
+    plot.add_model(name_, actual, prediction)
+
+
+def clear_error():
+    global plot
+    plot.clear_error()
+
+
+def set_plot_options(figsize=(15, 10), font_big=15, font_small=12, graph_width=10, round=5):
+    global plot
+    plot.set_plot_options(figsize=figsize, font_big=font_big, font_small=font_small, graph_width=graph_width, round=round)
+
+def summary(df):
+    print(f'데이터 프레임 형태(shape) : {df.shape}')
+    s = pd.DataFrame(df.dtypes, columns=['데이터 타입'])
+    s['최소값'] = df.min()
+    s['최대값'] = df.max()
+    s = s.reset_index()
+    s = s.rename(columns={'index':'특성명'})
+    s['결측치 개수'] = df.isna().sum().values
+    s['고유값 개수'] = df.nunique().values
+    s['고유값'] = [df[col_name].unique() for col_name in df.columns]
+    return s
+
+
+from sklearn.metrics import mean_squared_log_error
+def rmsle(true, pred):
+    return np.sqrt(mean_squared_log_error(true, pred)) 
+
+def gini(y_true, y_pred):
+    # 실제값과 예측값의 크기가 같은지 확인 (값이 다르면 오류 발생)
+    if y_true.shape != y_pred.shape:
+        raise Exception('Shape Error : 실제값과 예측값의 개수가 일치하지 않습니다.')
+
+    n_samples = y_true.shape[0]                      # 데이터 개수
+    L_mid = np.linspace(1 / n_samples, 1, n_samples) # 대각선 값
+
+    # 1) 예측값에 대한 지니계수
+    pred_order = y_true[y_pred.argsort()] # y_pred 크기순으로 y_true 값 정렬
+    L_pred = np.cumsum(pred_order) / np.sum(pred_order) # 로렌츠 곡선
+    G_pred = np.sum(L_mid - L_pred)       # 예측 값에 대한 지니계수
+
+    # 2) 예측이 완벽할 때 지니계수
+    true_order = y_true[y_true.argsort()] # y_true 크기순으로 y_true 값 정렬
+    L_true = np.cumsum(true_order) / np.sum(true_order) # 로렌츠 곡선
+    G_true = np.sum(L_mid - L_true)       # 예측이 완벽할 때 지니계수
+
+    # 정규화된 지니계수
+    return G_pred / G_true  
+    
+########## 에러 메시지 ############
+
+class ErrorChecker():
+    def __init__(self, test_size=None, evaluation='mse'):
+        self.test_size = test_size
+        self.evaluation = evaluation
+    
+    def check_error(self, pred):
+        """
+        error_code
+        1: 음수 값 제출시 에러
+        2: test셋의 length와 맞지 않음
+        """
+        msg = "[통과] 문제가 발견되지 않았습니다."
+        try:
+            if (self.evaluation == 'rmsle') and (pred[pred < 0].size > 0):
+                msg = "[오류]\n\n예측 값에(prediction) 음수 값이 있습니다!!\n\n대여량은 음수 값을 가질 수 없으므로 음수 값을 포함하는 정답은 제출이 불가합니다.\n\n음수값 확인 방법(코드):\n\nprediction[prediction < 0]"
+            elif (self.test_size) and len(pred) != self.test_size:
+                msg = f"[오류] \n\n예측 값인 prediction의 길이가 {self.test_size}개 이어야 합니다.\n\nlen(prediction) 의 값이 {self.test_size}개가 나오지 않는다면 제출이 불가 합니다.\n\n(test 세트로 예측했는지 확인해 주세요)"
+        except Exception as err:
+            msg = f'[오류] {err}'
+        print(msg)
+    
+    def set_values(self,  test_size=None, evaluation=None):
+        if test_size is not None:
+            self.test_size = test_size
+        if evaluation is not None:
+            self.evaluation = evaluation
+    
+    def get_values(self):
+        print(f'test case: {self.test_size}\nevaluation: {self.evaluation}')
+
+err_checker = ErrorChecker(test_size=6493, evaluation='rmsle')
+
+def check_error(prediction):
+    global err_checker
+    err_checker.check_error(prediction)
+
+def set_error_values(test_size=None, evaluation=None):
+    global err_checker
+    err_checker.set_values(test_size=test_size, evaluation=evaluation)
+
+
+
+
```

## Comparing `mySUNI-1.6.0.dist-info/LICENSE` & `mySUNI-2.0.0.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,661 +1,661 @@
-                    GNU AFFERO GENERAL PUBLIC LICENSE
-                       Version 3, 19 November 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU Affero General Public License is a free, copyleft license for
-software and other kinds of works, specifically designed to ensure
-cooperation with the community in the case of network server software.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-our General Public Licenses are intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  Developers that use our General Public Licenses protect your rights
-with two steps: (1) assert copyright on the software, and (2) offer
-you this License which gives you legal permission to copy, distribute
-and/or modify the software.
-
-  A secondary benefit of defending all users' freedom is that
-improvements made in alternate versions of the program, if they
-receive widespread use, become available for other developers to
-incorporate.  Many developers of free software are heartened and
-encouraged by the resulting cooperation.  However, in the case of
-software used on network servers, this result may fail to come about.
-The GNU General Public License permits making a modified version and
-letting the public access it on a server without ever releasing its
-source code to the public.
-
-  The GNU Affero General Public License is designed specifically to
-ensure that, in such cases, the modified source code becomes available
-to the community.  It requires the operator of a network server to
-provide the source code of the modified version running there to the
-users of that server.  Therefore, public use of a modified version, on
-a publicly accessible server, gives the public access to the source
-code of the modified version.
-
-  An older license, called the Affero General Public License and
-published by Affero, was designed to accomplish similar goals.  This is
-a different license, not a version of the Affero GPL, but Affero has
-released a new version of the Affero GPL which permits relicensing under
-this license.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU Affero General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Remote Network Interaction; Use with the GNU General Public License.
-
-  Notwithstanding any other provision of this License, if you modify the
-Program, your modified version must prominently offer all users
-interacting with it remotely through a computer network (if your version
-supports such interaction) an opportunity to receive the Corresponding
-Source of your version by providing access to the Corresponding Source
-from a network server at no charge, through some standard or customary
-means of facilitating copying of software.  This Corresponding Source
-shall include the Corresponding Source for any work covered by version 3
-of the GNU General Public License that is incorporated pursuant to the
-following paragraph.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the work with which it is combined will remain governed by version
-3 of the GNU General Public License.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU Affero General Public License from time to time.  Such new versions
-will be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU Affero General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU Affero General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU Affero General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU Affero General Public License as published
-    by the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU Affero General Public License for more details.
-
-    You should have received a copy of the GNU Affero General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If your software can interact with users remotely through a computer
-network, you should also make sure that it provides a way for users to
-get its source.  For example, if your program is a web application, its
-interface could display a "Source" link that leads users to an archive
-of the code.  There are many ways you could offer source, and different
-solutions will be better for different programs; see section 13 for the
-specific requirements.
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU AGPL, see
-<https://www.gnu.org/licenses/>.
+                    GNU AFFERO GENERAL PUBLIC LICENSE
+                       Version 3, 19 November 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU Affero General Public License is a free, copyleft license for
+software and other kinds of works, specifically designed to ensure
+cooperation with the community in the case of network server software.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+our General Public Licenses are intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  Developers that use our General Public Licenses protect your rights
+with two steps: (1) assert copyright on the software, and (2) offer
+you this License which gives you legal permission to copy, distribute
+and/or modify the software.
+
+  A secondary benefit of defending all users' freedom is that
+improvements made in alternate versions of the program, if they
+receive widespread use, become available for other developers to
+incorporate.  Many developers of free software are heartened and
+encouraged by the resulting cooperation.  However, in the case of
+software used on network servers, this result may fail to come about.
+The GNU General Public License permits making a modified version and
+letting the public access it on a server without ever releasing its
+source code to the public.
+
+  The GNU Affero General Public License is designed specifically to
+ensure that, in such cases, the modified source code becomes available
+to the community.  It requires the operator of a network server to
+provide the source code of the modified version running there to the
+users of that server.  Therefore, public use of a modified version, on
+a publicly accessible server, gives the public access to the source
+code of the modified version.
+
+  An older license, called the Affero General Public License and
+published by Affero, was designed to accomplish similar goals.  This is
+a different license, not a version of the Affero GPL, but Affero has
+released a new version of the Affero GPL which permits relicensing under
+this license.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU Affero General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Remote Network Interaction; Use with the GNU General Public License.
+
+  Notwithstanding any other provision of this License, if you modify the
+Program, your modified version must prominently offer all users
+interacting with it remotely through a computer network (if your version
+supports such interaction) an opportunity to receive the Corresponding
+Source of your version by providing access to the Corresponding Source
+from a network server at no charge, through some standard or customary
+means of facilitating copying of software.  This Corresponding Source
+shall include the Corresponding Source for any work covered by version 3
+of the GNU General Public License that is incorporated pursuant to the
+following paragraph.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the work with which it is combined will remain governed by version
+3 of the GNU General Public License.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU Affero General Public License from time to time.  Such new versions
+will be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU Affero General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU Affero General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU Affero General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU Affero General Public License as published
+    by the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU Affero General Public License for more details.
+
+    You should have received a copy of the GNU Affero General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If your software can interact with users remotely through a computer
+network, you should also make sure that it provides a way for users to
+get its source.  For example, if your program is a web application, its
+interface could display a "Source" link that leads users to an archive
+of the code.  There are many ways you could offer source, and different
+solutions will be better for different programs; see section 13 for the
+specific requirements.
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU AGPL, see
+<https://www.gnu.org/licenses/>.
```

