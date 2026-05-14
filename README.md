# sugarcane-irrigation-dataset
Dataset for Sugarcane Irrigation Decision Support System (SIDSS)
Sugarcane Irrigation Dataset for SIDSS Framework
📌 DOI
https://doi.org/10.5281/zenodo.19842337

📖 Description
This dataset contains structured records of sugarcane crop parameters used for irrigation prediction and yield estimation. It integrates physiological, environmental, and computed irrigation variables to support machine learning-based decision-making in precision agriculture.

The dataset is designed for developing and evaluating intelligent irrigation systems such as the Sugarcane Irrigation Decision Support System (SIDSS).

📊 Dataset Details
Total Samples: ~1500 (or specify exact if needed)
File Format: XLSX
File Name: catboostsugarcane_yield_prediction_regularized.xlsx
📂 Features Included
🌿 Physiological Parameters
stomataopenclose
nitrogen
phosphorus
chlorophyll
💧 Leaf & Water Parameters
leafhumidity
leafevaporation
evapotranspiration
🌱 Soil Parameters
soilph
soilhumidity
🌦️ Microclimatic Parameters
microclimatictemp
microclimaticwindspeed
microclimaticseason
🚿 Irrigation Parameter
predicted_water_liters_per_day
🌾 Output Variable
yield_kg_per_plant (actual / simulated)
predicted_yield (model output)
⚙️ Methodology Summary
Data collected from sugarcane cultivation fields
Preprocessed and normalized for model training
Synthetic augmentation applied (LeafGAN)
Deep learning models used:
EfficientNet-B0 (nutrient estimation)
MobileNetV3 (growth stage classification)
CatBoost used for:
Irrigation prediction
Yield estimation
📈 Usage
This dataset can be used for:

Irrigation prediction models
Crop yield estimation
Precision agriculture research
Machine learning benchmarking
Deep learning applications in agriculture
🧪 Example Use
import pandas as pd

df = pd.read_excel("catboostsugarcane_yield_prediction_regularized.xlsx")
print(df.head())
