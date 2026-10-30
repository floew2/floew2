# Geospatial Data Scientist

Building (geo-)data pipelines and geoprocessing workflows — from ETL automation and data modeling to satellite-based damage assessment (caused by natural disasters or conflict) and environmental monitoring to tackle environmental crimes via satellite images. Combining 12+ years of hands-on geospatial expertise with modern ML engineering practices to solve real-world problems across **agriculture, development cooperation, civil protection, and geointelligence applications**.

---

## 🛠️ Tech Stack

<table>
  <tr>
    <td valign="top" width="50%">
      <strong>ML & Data Science</strong><br>
      <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
      <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" alt="PyTorch"/>
      <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white" alt="TensorFlow"/>
      <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" alt="scikit-learn"/>
      <img src="https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white" alt="Keras"/>
    </td>
    <td valign="top" width="50%">
      <strong>MLOps & DevOps</strong><br>
      <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker"/>
      <img src="https://img.shields.io/badge/MLflow-0194E2?style=for-the-badge&logo=mlflow&logoColor=white" alt="MLflow"/>
      <img src="https://img.shields.io/badge/BentoML-FF69B4?style=for-the-badge" alt="BentoML"/>
      <img src="https://img.shields.io/badge/DVC-8A2BE2?style=for-the-badge&logo=dvc&logoColor=white" alt="DVC"/>
      <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white" alt="GitHub Actions"/>
      <img src="https://img.shields.io/badge/ONNX-005CED?style=for-the-badge&logo=onnx&logoColor=white" alt="ONNX"/>
      <img src="https://img.shields.io/badge/Evidently-4B4B4B?style=for-the-badge" alt="Evidently"/>
    </td>
  </tr>
  <tr>
    <td valign="top" width="50%">
      <strong>Geospatial & Remote Sensing</strong><br>
      <img src="https://img.shields.io/badge/QGIS-589632?style=for-the-badge&logo=qgis&logoColor=white" alt="QGIS"/>
      <img src="https://img.shields.io/badge/ArcGIS%20Pro-007AC2?style=for-the-badge" alt="ArcGIS Pro"/>
      <img src="https://img.shields.io/badge/FME-FF6600?style=for-the-badge&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mP8/5+hHgAHggJ/PchI7wAAAABJRU5ErkJggg==&logoColor=white" alt="FME"/>
      <img src="https://img.shields.io/badge/FME%20Flow-F58220?style=for-the-badge&logo=fme&logoColor=white" alt="FME Flow"/>
      <img src="https://img.shields.io/badge/Google%20Earth%20Engine-4285F4?style=for-the-badge" alt="Google Earth Engine"/>
      <img src="https://img.shields.io/badge/GeoPandas-150458?style=for-the-badge" alt="GeoPandas"/>
      <img src="https://img.shields.io/badge/GDAL-5CA548?style=for-the-badge&logo=gdal&logoColor=white" alt="GDAL"/>
    </td>
    <td valign="top" width="50%">
      <strong>Cloud & Visualization</strong><br>
      <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" alt="Kubernetes"/>
      <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white" alt="Streamlit"/>
      <img src="https://img.shields.io/badge/Plotly-3F4F75?style=for-the-badge&logo=plotly&logoColor=white" alt="Plotly"/>
      <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript"/>
      <img src="https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white" alt="R"/>
    </td>
  </tr>
</table>

---

## 🔬 Recent Projects

### 🌾 [Reading a Drought from Space: Switzerland 2026](https://github.com/floew2/drought-from-space-switzerland)

How hard did the 2026 summer drought hit grassland in the Canton of St. Gallen? A reproducible Sentinel-2 pipeline, run from Python on Google Earth Engine, that measures grassland condition and mowing field by field in three landscapes, against a 2019–2025 baseline and MeteoSwiss station data.

**Key Features**:
- Pixel purity modelled from the Sentinel-2 point-spread function, so small, edge-dominated meadows are measured without mixed-pixel contamination
- Result: the meadows' moisture index (NDMI) fell 23–29 % below normal, the lowest of eight years at both valley sites
- Mowing detector validated like a model: rules frozen after tuning, then scored on 136 hand-labelled field-years including a hold-out (F1 0.87), with its drought-year failure diagnosed
- Runs end to end on calibrated synthetic data; provenance checks refuse stale results; CI with tests

**Tech Stack**: Python • Google Earth Engine • Sentinel-2 • GeoPandas • rasterio • NumPy • pandas • SciPy • pytest • GitHub Actions

### 🏚️ Building Damage Classification
*🚧 Under active development · repository not yet public*

End-to-end MLOps pipeline for automated building damage assessment from satellite imagery using YOLO26 / RT-DETR. Full ML lifecycle from data versioning to production deployment.

**Key Features**:
- FastAPI microservices architecture with JWT authentication, being prepared for Kubernetes deployment
- Automated CI/CD with model promotion logic
- Real-time monitoring and drift detection
- Production-ready API serving

**Tech Stack**: YOLO26 • RT-DETR • PyTorch • DVC • MLflow • GitHub Actions • FastAPI • Docker • Prometheus • Grafana • Evidently

### 🔎 [Hybrid Retrieval for Georeferenced Conflict Event Data](https://github.com/floew2/rag-ucdp)
*🚧 Under active development.*

Routed retrieval-augmented generation (RAG) system over the UCDP Georeferenced Event
Dataset. Combines semantic search with deterministic aggregation on a fully local LLM stack — no data leaves the machine, and every answer
stays traceable to the source events behind it.

**Key Features**:
- Hybrid BM25 + dense retrieval (BGE-large-en-v1.5) fused via reciprocal rank fusion, with multi-query expansion and BGE reranker
- Four-path query router separating semantic retrieval, deterministic aggregation, and out-of-scope refusal
- Source-bias surfacing and geospatial visualization of results
- Non-circular evaluation harness: method-independent gold set via 5-arm pooling, multi-event held-out recall benchmark, nDCG/MAP/MRR
- 214 unit tests with CI; Docker setup for reproducible local runs

**Tech Stack**: Python • ChromaDB • BM25Okapi • BGE-large-en-v1.5 • Mistral 7B via Ollama (local) • Streamlit • Docker

### 🛰️ Multi-temporal Oil Spill Detection
*🚧 Under active development · repository not yet public*

Machine learning system for detecting terrestrial oil spills using multi-temporal Sentinel-2 imagery. Handles extreme class imbalance and spectral confusion through temporal change detection.

**Key Features**:
- Multi-temporal baseline composites for change detection
- Custom augmentation for extreme data scarcity (only few ground validated reference events)
- MLOps pipeline from data ingestion to containerized model serving

**Tech Stack**: PyTorch • U-Net • Prithvi-EO-2.0 • Clay • Sentinel-2 • DVC • MLflow • BentoML • Docker • Microsoft Planetary Computer

### 📚 [Curated Annotation Datasets for Remote Sensing](https://github.com/floew2/remotesensing-annotation-datasets)

A curated and evaluated collection of publicly available, high-quality annotation datasets for training computer vision models on satellite and aerial imagery.

**Key Features**:
- Overview and categorization of datasets by application (building footprint extraction, road segmentation, ship detection)
- Direct links to data sources and relevant academic papers
- Clear criteria for inclusion, focusing on data quality, documentation, and accessibility

---

## 💼 Professional Background

- **Current Focus**: Deep Learning & Remote Sensing, GIS & Data Science Specialist  
- **Previous**: Remote Sensing & ML Specialist (10+ years)  
- **Education**: PhD in Environmental Remote Sensing & Machine Learning
- **Research**: 10+ peer-reviewed publications in GIScience & Remote Sensing, Environmental Management, and Applied Remote Sensing

---
