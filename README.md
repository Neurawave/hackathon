# Hackathon Instructions

**Theme:** Health and wellbeing or Migraine prediction & insights

Welcome to the Hackathon! In this repository, you will find many resources you may use, and instructions how to use them to get started with your hackathon project.

## 📁 Repository Structure

### Data (`data/`)
The heart of the project with several different data sources to choose from:

#### 1. **MBRAIN21 Dataset** (`data/mbrain21-csv/`)
- Real research data about migraines from Kaggle
- Contains daily event dumps for 4 patients over 3 months (MBRAIN21-001 to MBRAIN21-004)
- Could be useful for building prediction models based on real anonymised user data
- More info and credits: https://www.kaggle.com/datasets/jonvdrdo/mbrain21

#### 2. **Relief aHead API** (`data/relief ahead/`)
- Neurawave API used for tracking personal wellbeing. Only own users data is available.
- Build your own backend based on this specification, or use it as inspiration for your data model
- API url: https://api.reliefahead.com/test
- API structure specification: [`openapi.yaml`](data/relief ahead/openapi.yaml)
- You can also run Swagger to see API structure:
  - Instructions how to run Swagger: [reliefaheadAPI.md](data/relief ahead/reliefaheadAPI.md)
  - The data is a reference/example only - there is no actual backend bundled with OpenAPI & Swagger

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
- **Download:** The CSV files are too large to include in this repository. Please download them manually:
  - [synthetic_data_10_000.zip](https://drive.google.com/file/d/1M6GYn98nnvJ4QKk8xUJeXDGWkdx4Sgld/view?usp=sharing) (108 MB)
  - [synthetic_data_100_000.zip](https://drive.google.com/file/d/1jjFNkutK-YWJnfRY5qEmbPSO1DVuWmDb/view?usp=sharing) (1.09 GB)

### Example applications

#### 1. Mobile app example  (`flutter_app/`)
A ready-made Flutter app with Bootstrap-inspired design that you can use as a foundation:
- Support for web, iOS and Android
- Run with `flutter run` (see [`README.md`](flutter_app/README.md) for details)

#### 2. Fetching weather (`api_examples/`)
- `weather_api_example.ipynb` - Jupyter notebook with examples of how to fetch weather data from SMHI
- Can be used to connect weather data with migraine triggers

#### 3. API Backend examples (`backend/`)
- A simple Flask API example that you can use as a starting point for building your own backend
- Ready to run with just `pip install -r requirements.txt` and `python main.py`
- Includes a basic "Hello World" endpoint - extend it with your own data endpoints
- See [`README.md`](backend/README.md) for detailed instructions

