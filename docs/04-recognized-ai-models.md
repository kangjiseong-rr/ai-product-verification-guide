# 인정 인공지능 모델

## 주요 머신러닝 기반 모델

| 유형 | 라이브러리 | 공식 모듈명 |
|---|---|---|
| 지도학습<br>(분류/회귀) | scikit-learn<br>(sklearn) | `sklearn.linear_model.LinearRegression`<br>`sklearn.linear_model.LogisticRegression`<br>`sklearn.svm.SVC` (Support Vector Classification)<br>`sklearn.ensemble.RandomForestClassifier`<br>`sklearn.linear_model.Ridge`<br>`sklearn.linear_model.Lasso`<br>`sklearn.linear_model.ElasticNet`<br>`sklearn.svm.SVR` (Support Vector Regression)<br>`sklearn.ensemble.RandomForestRegressor`<br>`sklearn.ensemble.GradientBoostingClassifier`<br>`sklearn.ensemble.GradientBoostingRegressor`<br>`sklearn.ensemble.AdaBoostClassifier`<br>`sklearn.ensemble.ExtraTreesClassifier`<br>`sklearn.tree.DecisionTreeClassifier`<br>`sklearn.tree.DecisionTreeRegressor`<br>`sklearn.neighbors.KNeighborsClassifier`<br>`sklearn.neighbors.KNeighborsRegressor`<br>`sklearn.naive_bayes.GaussianNB`<br>`sklearn.naive_bayes.MultinomialNB`<br>`sklearn.cross_decomposition.PLSRegression` |
| 부스팅 알고리즘 | XGBoost / LightGBM | `xgboost.XGBClassifier` / `xgboost.XGBRegressor`<br>`lightgbm.LGBMClassifier` / `lightgbm.LGBMRegressor` |
| 비지도학습<br>(군집) | scikit-learn<br>(sklearn) | `sklearn.cluster.Kmeans`<br>`sklearn.decomposition.PCA` |
| 통계식 시계열 분석 | statsmodels | `statsmodels.tsa.arima.model.ARIMA` |

!!! note "유의사항"
    목록에 없는 모델도 항목 1.2에 따라 검토 후 인정 가능합니다.

## 주요 딥러닝 기반 모델

| 유형 | 라이브러리 | 모듈명 |
|---|---|---|
| 시각 인지<br>(CNN 계열) | PyTorch / TensorFlow / Ultralytics | `torchvision.models.resnet50`<br>`keras.applications.resnet50.ResNet50`<br>`ultralytics.YOLO`<br>`ultralytics.YOLOv8`<br>`ultralytics.YOLOv10`<br>`ultralytics.YOLO11`<br>`torchvision.models.resnet101`<br>`torchvision.models.vgg16`<br>`torchvision.models.efficientnet_b0`<br>`torchvision.models.efficientnet_v2_s`<br>`torchvision.models.convnext_tiny`<br>`torchvision.models.vit_b_16`<br>`torchvision.models.swin_t`<br>`keras.applications.vgg16.VGG16`<br>`keras.applications.efficientnet.EfficientNetB4`<br>`keras.applications.mobilenet_v3.MobileNetV3Large` |
| 시각 인지<br>(이미지 확장, 페이스 등) | timm / segmentation_models_pytorch / Detectron2 (Facebook) | `timm.models.resnet50`<br>`timm.models.efficientnet_b0`<br>`segmentation_models_pytorch.Unet`<br>`detectron2.modeling.build_model` |
| 시계열<br>(RNN 계열) | PyTorch / Keras | `torch.nn.LSTM` / `torch.nn.GRU`<br>`keras.layers.LSTM` / `keras.layers.GRU`<br>`torch.nn.Transformer` |
| 자연어 이해<br>(NLU) | Hugging Face<br>(Transformers) | `transformers.BertModel`<br>`transformers.AutoModelForSequenceClassification`<br>`transformers.RobertaModel`<br>`transformers.DistilBertModel`<br>`transformers.ElectraModel`<br>`transformers.AlbertModel`<br>`transformers.T5Model`<br>`transformers.BartModel` |

!!! note "유의사항"
    이외에도 허깅페이스(Hugging Face) 업로드 모델은 확인 후 인정 가능합니다.

## 주요 생성형 AI 모델

| 유형 | 라이브러리 | 모듈명 |
|---|---|---|
| 프레임워크 연동 | LangChain | `langchain_core.language_models.chat_models` |
| 오픈소스 대형 모델 | Hugging Face (Transformers) | `transformers.AutoModelForCausalLM` |
| 텍스트 임베딩 | OpenAI Python SDK | `openai.resources.embeddings` |
| 상용 독점 모델 API | Anthropic SDK | `anthropic.resources.messages` (Claude) |
| 상용 독점 모델 API | Google Generative AI | `google.generativeai.GenerativeModel` (Gemini) |
| 상용 독점 모델 API | OpenAI Python SDK | `openai.resources.chat.completions` |
| 오픈소스 LLM 가중치 | Meta AI (Llama) | `Llama-3-8B-Instruct`<br>`Llama-3-70B-Instruct` |
| 오픈소스 LLM 가중치 | Mistral AI | `Mistral-7B-Instruct`<br>`Mixtral-8x7B-Instruct` |
| 오픈소스 LLM 가중치 | Alibaba Cloud (Qwen) | `Qwen2.5-7B-Instruct`<br>`Qwen2.5-Coder` |
| 오픈소스 LLM 가중치 | DeepSeek | `DeepSeek-V3`<br>`DeepSeek-R1` |
| 오픈소스 LLM 가중치 | Google (Gemma) | `Gemma-2-9b`<br>`Gemma-2-27b` |
| 오픈소스 LLM 가중치 | Microsoft (Phi) | `Phi-3-mini-instruct` |
| 국내 도메인 모델 API | Naver Cloud (HyperCLOVA-X) | `HyperCLOVA-X CLOVA Studio API` |
| 국내 도메인 모델 API | Upstage (Solar) | `Solar-10.7B-Instruct API` |
| 이미지 생성 (Diffusion) | Hugging Face (Diffusers) | `diffusers.StableDiffusionPipeline`<br>`diffusers.StableDiffusionXLPipeline`<br>`diffusers.FluxPipeline` |
| 이미지 생성 고속화 | Hugging Face (Diffusers) | `diffusers.LatentConsistencyModelPipeline` |
| 이미지 조건 제어 | Hugging Face (Diffusers) | `diffusers.ControlNetModel` |
| 오디오/음성 생성 (TTS) | Hugging Face (Transformers) | `transformers.SpeechT5ForTextToSpeech` |
| 음성 인식 (STT) | Hugging Face (Transformers) | `transformers.WhisperForConditionalGeneration` |
| 오디오 오케스트레이션 | Hugging Face (Transformers) | `transformers.BarkModel` |
| 이미지 생성 최신화 | Hugging Face (Diffusers) | `diffusers.SanaPipeline` |
| 클라우드 상용 서비스 연동 | Midjourney API | `midjourney.api` |
| 클라우드 상용 서비스 연동 | Suno AI API | `suno.api` |
| 클라우드 상용 서비스 연동 | ElevenLabs API | `elevenlabs.api` |

!!! note "유의사항"
    이외에도 허깅페이스(Hugging Face) 업로드 모델은 확인 후 인정 가능합니다.

## 기타

| 유형 | 라이브러리 | 모듈명 |
|---|---|---|
| 강화학습 (RL) | Stable-Baselines3 | `stable_baselines3.PPO`<br>`stable_baselines3.DQN`<br>`stable_baselines3.A2C`<br>`stable_baselines3.SAC`<br>`stable_baselines3.TD3` |
| 강화학습 (RL) | Ray (RLlib) | `ray.rllib.algorithms.ppo.PPO`<br>`ray.rllib.algorithms.dqn.DQN`<br>`ray.rllib.algorithms.sac.SAC` |
| 이상징후탐지 (Anomaly) | scikit-learn (sklearn) | `sklearn.ensemble.IsolationForest`<br>`sklearn.svm.OneClassSVM`<br>`sklearn.neighbors.LocalOutlierFactor`<br>`sklearn.covariance.EllipticEnvelope` |
| 이상탐지 패키지 전문화 | PyOD (Python Outlier Detection) | `pyod.models.knn.KNN`<br>`pyod.models.iforest.IForest`<br>`pyod.models.copod.COPOD`<br>`pyod.models.auto_encoder.AutoEncoder` |
| 기계학습 기반 시계열예측 | Prophet (Meta) | `prophet.Prophet` |
| 기계학습 기반 시계열예측 | sktime | `sktime.forecasting.arima.ARIMA` |
| 딥러닝 기반 시계열예측 | GluonTS (Amazon) | `gluonts.mx.model.deepar.DeepAREstimator` |
| 딥러닝 기반 시계열예측 | Darts | `darts.models.forecasting.tft_model.TFTModel`<br>`darts.models.forecasting.nhits.NBEATSModel` |
| 그래프뉴럴네트워크 (GNN) | PyTorch Geometric (PyG) | `torch_geometric.nn.GCNConv`<br>`torch_geometric.nn.GATConv` |
| 추천시스템 | Microsoft Recommenders | `recommenders.models.deeprec.models.xdeepfm.XDeepFMModel` |
| 추천시스템 | LightFM | `lightfm.LightFM` |
| 추천시스템 | Surprise | `surprise.prediction_algorithms.matrix_factorization.SVD` |
