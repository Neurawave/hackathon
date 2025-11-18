# Hackathon Instructions

**Theme:** Health and wellbeing or Migraine prediction & insights

Welcome to the Hackathon! In this repository, you will find all the necessary instructions and resources to get started with your hackathon project.

## 📁 Repository Structure

### Data (`data/`)
The heart of the project with several different data sources to choose from:

#### 1. **MBRAIN21 Dataset** (`data/mbrain21-csv/`)
- Real research data about migraines from Kaggle
- Contains event dumps for 4 patients (MBRAIN21-001 to MBRAIN21-004)
- Perfect for building prediction models based on real patient data
- More info: https://www.kaggle.com/datasets/jonvdrdo/mbrain21

#### 2. **Relief aHead API** (`data/relief ahead/`)
- OpenAPI specification showing how our real API is structured
- **Note:** This is a reference/example only - there is no running backend available for the hackathon
- You can use the `openapi.yaml` specification to understand the API structure
- View the API documentation with Swagger UI: see instructions in `reliefaheadAPI.md`
- Build your own backend based on this specification, or use it as inspiration for your data model

#### 3. **Open Seizure Detector** (`data/openseizuredetector/`)
- Open source project for health data management
- Can be customized and further developed even after the hackathon
- GitHub: https://github.com/OpenSeizureDetector/webApi/tree/master/api
- Website: https://www.openseizuredetector.org.uk/

#### 4. **Synthetic Data** (`data/synthetic/`)
- Large amounts of synthetic (generated) data for testing
- Two sizes: 10,000 and 100,000 persons
- Contains:
  - `person_data_*.csv` - Personal information
  - `health_data_*.csv` - Health data with triggers and migraine events
  - `weather_data.csv` - Weather data
- Detailed documentation of all fields in `synthetic.md`
- Perfect for training machine learning models without privacy concerns

### Frontend (`flutter_app/`)
A ready-made Flutter app with Bootstrap-inspired design that you can use as a foundation:
- Support for web, iOS and Android
- Run with `flutter run` (see `README.md` for details)

### API Examples (`api_examples/`)
- `weather_api_example.ipynb` - Jupyter notebook with examples of how to fetch weather data from SMHI
- Can be used to connect weather data with migraine triggers




