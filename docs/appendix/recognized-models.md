# 인정 인공지능 모델

이 목록은 신청 제품·서비스에 적용된 AI 모델을 설명할 때 참고할 수 있는 예시입니다. 목록에 없는 모델도 학습·추론 특성을 확인할 수 있다면 검토될 수 있습니다.

!!! note "주의"
    모델 목록은 기술 발전과 정책 운영에 따라 변경될 수 있습니다. 공개 전 최신 목록 반영 여부를 확인하세요.

## 주요 머신러닝 기반 모델

| 유형 | 라이브러리 | 공식 모듈명 |
|---|---|---|
| 지도학습: 분류·회귀 | scikit-learn | `sklearn.linear_model.LinearRegression` |
| 지도학습: 분류·회귀 | scikit-learn | `sklearn.linear_model.LogisticRegression` |
| 지도학습: 분류·회귀 | scikit-learn | `sklearn.svm.SVC` |
| 지도학습: 분류·회귀 | scikit-learn | `sklearn.ensemble.RandomForestClassifier` |
| 지도학습: 분류·회귀 | scikit-learn | `sklearn.linear_model.Ridge` |
| 지도학습: 분류·회귀 | scikit-learn | `sklearn.linear_model.Lasso` |
| 지도학습: 분류·회귀 | scikit-learn | `sklearn.linear_model.ElasticNet` |
| 지도학습: 분류·회귀 | scikit-learn | `sklearn.svm.SVR` |
| 지도학습: 분류·회귀 | scikit-learn | `sklearn.ensemble.RandomForestRegressor` |
| 지도학습: 분류·회귀 | scikit-learn | `sklearn.ensemble.GradientBoostingClassifier` |
| 지도학습: 분류·회귀 | scikit-learn | `sklearn.ensemble.GradientBoostingRegressor` |
| 지도학습: 분류·회귀 | scikit-learn | `sklearn.ensemble.AdaBoostClassifier` |
| 지도학습: 분류·회귀 | scikit-learn | `sklearn.ensemble.ExtraTreesClassifier` |
| 지도학습: 분류·회귀 | scikit-learn | `sklearn.tree.DecisionTreeClassifier` |
| 지도학습: 분류·회귀 | scikit-learn | `sklearn.tree.DecisionTreeRegressor` |
| 지도학습: 분류·회귀 | scikit-learn | `sklearn.neighbors.KNeighborsClassifier` |
| 지도학습: 분류·회귀 | scikit-learn | `sklearn.neighbors.KNeighborsRegressor` |
| 지도학습: 분류·회귀 | scikit-learn | `sklearn.naive_bayes.GaussianNB` |
| 지도학습: 분류·회귀 | scikit-learn | `sklearn.naive_bayes.MultinomialNB` |
| 지도학습: 분류·회귀 | scikit-learn | `sklearn.cross_decomposition.PLSRegression` |
| 부스팅 알고리즘 | XGBoost / LightGBM | `xgboost.XGBClassifier`, `xgboost.XGBRegressor` |
| 부스팅 알고리즘 | XGBoost / LightGBM | `lightgbm.LGBMClassifier`, `lightgbm.LGBMRegressor` |
| 비지도학습: 군집 | scikit-learn | `sklearn.cluster.KMeans` |
| 비지도학습: 차원축소 | scikit-learn | `sklearn.decomposition.PCA` |
| 통계식 시계열 분석 | statsmodels | `statsmodels.tsa.arima.model.ARIMA` |

## 주요 딥러닝 기반 모델

| 유형 | 라이브러리 | 모듈명 |
|---|---|---|
| 시각 인지: CNN 계열 | PyTorch / TensorFlow / Ultralytics | `torchvision.models.resnet50` |
| 시각 인지: CNN 계열 | PyTorch / TensorFlow / Ultralytics | `keras.applications.resnet50.ResNet50` |
| 시각 인지: CNN 계열 | PyTorch / TensorFlow / Ultralytics | `ultralytics.YOLO`, `ultralytics.YOLOv8`, `ultralytics.YOLOv10`, `ultralytics.YOLO11` |
| 시각 인지: CNN 계열 | PyTorch | `torchvision.models.resnet101`, `torchvision.models.vgg16` |
| 시각 인지: CNN 계열 | PyTorch | `torchvision.models.efficientnet_b0`, `torchvision.models.efficientnet_v2_s` |
| 시각 인지: CNN 계열 | PyTorch | `torchvision.models.convnext_tiny`, `torchvision.models.vit_b_16`, `torchvision.models.swin_t` |
| 시각 인지: CNN 계열 | Keras | `keras.applications.efficientnet.EfficientNetB4` |
| 시각 인지: CNN 계열 | Keras | `keras.applications.mobilenet_v3.MobileNetV3Large` |
| 시각 인지: 이미지 확장·페이스 등 | timm | `timm.models.resnet50`, `timm.models.efficientnet_b0` |
| 시각 인지: 이미지 확장·페이스 등 | segmentation_models_pytorch | `segmentation_models_pytorch.Unet` |
| 시각 인지: 이미지 확장·페이스 등 | Detectron2 | `detectron2.modeling.build_model` |
| 시계열: RNN 계열 | PyTorch / Keras | `torch.nn.LSTM`, `torch.nn.GRU`, `keras.layers.LSTM`, `keras.layers.GRU` |
| 시계열: Transformer | PyTorch | `torch.nn.Transformer` |
| 자연어 이해: NLU | Hugging Face Transformers | `transformers.BertModel` |
| 자연어 이해: NLU | Hugging Face Transformers | `transformers.AutoModelForSequenceClassification` |
| 자연어 이해: NLU | Hugging Face Transformers | `transformers.RobertaModel`, `transformers.DistilBertModel` |
| 자연어 이해: NLU | Hugging Face Transformers | `transformers.ElectraModel`, `transformers.AlbertModel` |
| 자연어 이해: NLU | Hugging Face Transformers | `transformers.T5Model`, `transformers.BartModel` |

## 주요 생성형 AI 모델

| 유형 | 라이브러리 또는 서비스 | 모듈명 또는 모델명 |
|---|---|---|
| 프레임워크 연동 | LangChain | `langchain_core.language_models.chat_models` |
| 오픈소스 대형 모델 | Hugging Face Transformers | `transformers.AutoModelForCausalLM` |
| 텍스트 임베딩 | OpenAI Python SDK | `openai.resources.embeddings` |
| 상용 독점 모델 API | Anthropic SDK | `anthropic.resources.messages` |
| 상용 독점 모델 API | Google Generative AI | `google.generativeai.GenerativeModel` |
| 상용 독점 모델 API | OpenAI Python SDK | `openai.resources.chat.completions` |
| 오픈소스 LLM 가중치 | Meta AI | Llama 계열 모델 |
| 오픈소스 LLM 가중치 | Mistral AI | Mistral, Mixtral 계열 모델 |
| 오픈소스 LLM 가중치 | Alibaba Cloud | Qwen 계열 모델 |
| 오픈소스 LLM 가중치 | DeepSeek | DeepSeek 계열 모델 |
| 오픈소스 LLM 가중치 | Google | Gemma 계열 모델 |
| 오픈소스 LLM 가중치 | Microsoft | Phi 계열 모델 |
| 국내 도메인 모델 API | Naver Cloud | HyperCLOVA X CLOVA Studio API |
| 국내 도메인 모델 API | Upstage | Solar API |
| 이미지 생성 | Hugging Face Diffusers | `diffusers.StableDiffusionPipeline`, `diffusers.StableDiffusionXLPipeline`, `diffusers.FluxPipeline` |
| 이미지 생성 고속화 | Hugging Face Diffusers | `diffusers.LatentConsistencyModelPipeline` |
| 이미지 조건 제어 | Hugging Face Diffusers | `diffusers.ControlNetModel` |
| 오디오·음성 생성 | Hugging Face Transformers | `transformers.SpeechT5ForTextToSpeech` |
| 음성 인식 | Hugging Face Transformers | `transformers.WhisperForConditionalGeneration` |
| 오디오 오케스트레이션 | Hugging Face Transformers | `transformers.BarkModel` |
| 클라우드 상용 서비스 연동 | Midjourney API | `midjourney.api` |
| 클라우드 상용 서비스 연동 | Suno AI API | `suno.api` |
| 클라우드 상용 서비스 연동 | ElevenLabs API | `elevenlabs.api` |

## 기타 모델

| 유형 | 라이브러리 | 모듈명 |
|---|---|---|
| 강화학습 | Stable-Baselines3 | `stable_baselines3.PPO`, `stable_baselines3.DQN`, `stable_baselines3.A2C`, `stable_baselines3.SAC`, `stable_baselines3.TD3` |
| 강화학습 | Ray RLlib | `ray.rllib.algorithms.ppo.PPO`, `ray.rllib.algorithms.dqn.DQN`, `ray.rllib.algorithms.sac.SAC` |
| 이상징후탐지 | scikit-learn | `sklearn.ensemble.IsolationForest`, `sklearn.svm.OneClassSVM`, `sklearn.neighbors.LocalOutlierFactor`, `sklearn.covariance.EllipticEnvelope` |
| 이상탐지 패키지 | PyOD | `pyod.models.knn.KNN`, `pyod.models.iforest.IForest`, `pyod.models.copod.COPOD`, `pyod.models.auto_encoder.AutoEncoder` |
| 기계학습 기반 시계열 예측 | Prophet | `prophet.Prophet` |
| 기계학습 기반 시계열 예측 | sktime | `sktime.forecasting.arima.ARIMA` |
| 딥러닝 기반 시계열 예측 | GluonTS | `gluonts.mx.model.deepar.DeepAREstimator` |
| 딥러닝 기반 시계열 예측 | Darts | `darts.models.forecasting.tft_model.TFTModel`, `darts.models.forecasting.nhits.NBEATSModel` |
| 그래프 뉴럴 네트워크 | PyTorch Geometric | `torch_geometric.nn.GCNConv`, `torch_geometric.nn.GATConv` |
| 추천 시스템 | Microsoft Recommenders | `recommenders.models.deeprec.models.xdeepfm.XDeepFMModel` |
| 추천 시스템 | LightFM | `lightfm.LightFM` |
| 추천 시스템 | Surprise | `surprise.prediction_algorithms.matrix_factorization.SVD` |
