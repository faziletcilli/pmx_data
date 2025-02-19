# Predictive Maintence Metadata Repository

branch name: main

Predictive Maintenance poses a number of challenges for machine learning. The general types of machine learning problems encountered in predictive maintenance are:

1. Time to failure prediction
2. Anomaly detection
3. Clustering
4. Fault detection and root cause analysis

The purpose of this repository is to help researchers start working on predictive maintenance quickly. It provides an overview of relevant predictive maintenance data and 'quick start' scripts for researchers. This is a *metadata* repository, so it does not contain the data itself--only information about the data, and scripts for downloading and working with it.

## Table of Contents

1. [Table of Contents](#table-of-contents)
2. [List of Datasets](#list-of-datasets)
3. [Downloading a Dataset](#downloading-a-dataset)
4. [Adding a Dataset](#adding-a-dataset)
5. [Additional Resources](#additional-resources)
6. [Wishlist](#wishlist)

## List of Datasets

| **Dataset**                                                                                                                                              | **Description**                                                                                                                     | **Problems**                       | **Equipment Type**                  | **Note**                                                    |
| -------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------- | ----------------------------------- | ----------------------------------------------------------- |
| [maintnet](https://github.com/autonlab/pmx_data/tree/main/pmx_data/MaintNet)                                                                             | Maintenance action write-ups for aircraft, automotive, and facility domains                                                         | Language model, event forecasting  | Aircraft, automotives, and facility |                                                             |
| [autonomous underwater vehicle](https://github.com/autonlab/pmx_data/tree/main/pmx_data/autonomous_underwater_vehicle)                                   | Time series measurements from an underwater vehicle with 5 fault types                                                              | Time Series Fault Classification   | Maritime                            | rar data compression                                        |
| [cnc mill tool wear](https://github.com/autonlab/pmx_data/tree/main/pmx_data/cnc_mill_tool_wear)                                                         | Time series machining data across 18 CNC milling experiments                                                                        | Time Series Fault Detection        | Tools & Machinery                   |                                                             |
| [Delta Robot](https://github.com/autonlab/pmx_data/tree/main/pmx_data/delta_robot)                                                                       | Time series sensor data for a robot used in a production line                                                                       | Time Series Anomaly Detection      | Robotics                            |                                                             |
| [Diesel Engine Faults](https://github.com/autonlab/pmx_data/tree/main/pmx_data/diesel_engine_faults)                                                     | Diesel engine data from failure scenarios across 4 operating states                                                                 | Diagnostics / Fault Classification | Engines                             |                                                             |
| [electrical fault detection](https://github.com/autonlab/pmx_data/tree/main/pmx_data/electrical_fault_detection)                                         | Line currents and voltages of electrical system with 4 fault conditions                                                             | Fault Detection and Classification | Electrical                          |                                                             |
| [gearbox fault detection](https://github.com/autonlab/pmx_data/tree/main/pmx_data/gearbox_fault_detection)                                               | Bench test gearbox with 7 induced faults to detect in 3 channels, high frequency timeseries                                         | Fault Detection                    | Gearboxes & Mechanisms              |                                                             |
| [gearbox fault diagnosis](https://github.com/autonlab/pmx_data/tree/main/pmx_data/gearbox_fault_diagnosis)                                               | Vibration measurements from healthy and faulty gearboxes with varying loads and recoring frequencies                                | Fault detection                    | Gearboxes & Mechanisms              |                                                             |
| [hdd data](https://github.com/autonlab/pmx_data/tree/main/pmx_data/hdd_data)                                                                             | 2013 BlackBlaze hard drive failure data                                                                                             | Time to failure prediction         | Computer HW & IOT                   |                                                             |
| [hydraulic sensor system](https://github.com/autonlab/pmx_data/tree/main/pmx_data/hydraulic_sensor_system)                                               | Time series sensor readings on a hydraulic test rig with target condition values                                                    | Fault Detection and Classification | Tools & Machinery                   |                                                             |
| [li-ion battery aging](https://github.com/autonlab/pmx_data/tree/main/pmx_data/li-ion_battery_aging)                                                     | Data from tests on 4 Lithium-Ion batteries cycled under random currents                                                             | Time to failure prediction         | Batteries                           |                                                             |
| [machinery faults datasets](https://github.com/autonlab/pmx_data/tree/main/pmx_data/machinery_faults_datasets)                                           | Extremely large dataset of simulated time series machinery data with 6 operating states, each of which can have several fault types | Fault classification               | Tools & Machinery                   |                                                             |
| [Maintenance of naval propulsion plants](https://github.com/autonlab/pmx_data/tree/main/pmx_data/maintenance_of_naval_propulsion_plants)                 | Synthetic gas turbine data                                                                                                          | Time to failure prediction         | Maritime                            |                                                             |
| [nasa milling prognostic dataset](https://github.com/autonlab/pmx_data/tree/main/pmx_data/nasa_milling_prognostic_dataset)                               | Investigating wear on a milling machine under several runs in various operating conditions                                          | Fault Detection                    | Tools & Machinery                   |                                                             |
| [one year industrial component degradation](https://github.com/autonlab/pmx_data/tree/main/pmx_data/one_year_industrial_component_degradation)           | High-frequency time series data documentating degradation of an industrial component over the course of a year                      | Time to failure prediction         | Tools & Machinery                   |                                                             |
| [plant fault detection](https://github.com/autonlab/pmx_data/tree/main/pmx_data/plant_fault_detection)                                                   | Time series measurement from 70 plants with 6 fault types                                                                           | Fault detection                    | Gearboxes & Mechanisms              |                                                             |
| [pmx for aircraft machine and components](https://github.com/autonlab/pmx_data/tree/main/pmx_data/pmx_for_aircraft_machine_and_components)               | telemetry time series data and maintenance records for aircraft                                                                     | Time to failure prediction         | Aircraft                            |                                                             |
| [pmx for ga](https://github.com/autonlab/pmx_data/tree/main/pmx_data/pmx_for_ga)                                                                         | Per-second sensor data from flights of a Cessna 172S preceeding maintenance                                                         | Time to failure prediction         | Aircraft                            |                                                             |
| [pmx from elevator industry](https://github.com/autonlab/pmx_data/tree/main/pmx_data/pmx_from_elevator_industry)                                         | Data on elevator ball bearing wear                                                                                                  | Time to failure prediction         | Tools & Machinery                   |                                                             |
| [pmx iot sensor](https://github.com/autonlab/pmx_data/tree/main/pmx_data/pmx_iot_sensor)                                                                 | Data on failure of heat exchagers on an assembly line                                                                               | Time to failure prediction         | Tools & Machinery                   |                                                             |
| [prediction of downtime duration](https://github.com/autonlab/pmx_data/tree/main/pmx_data/prediction_of_downtime_duration)                               | Predicting downtime duration of car manufacturing assembly lines                                                                    | Time to event prediction           | Tools & Machinery                   |                                                             |
| [predictive maintenance fault classification](https://github.com/autonlab/pmx_data/tree/main/pmx_data/predictive_maintenance_fault_classification)       | Sensor data from a drill press under induced fault conditions                                                                       | Fault detection and classification | Tools & Machinery                   |                                                             |
| [production plant data for condition monitoring](https://github.com/autonlab/pmx_data/tree/main/pmx_data/production_plant_data_for_condition_monitoring) | Sensor data from 8 run-to-failure experiements on a production line component                                                       | Time to failure prediction         | Tools & Machinery                   |                                                             |
| [pump sensor](https://github.com/autonlab/pmx_data/tree/main/pmx_data/pump_sensor)                                                                       | Time series sensor readings from a water pump with status                                                                           | Anomaly detection                  | Tools & Machinery                   |                                                             |
| [robot execution failures](https://github.com/autonlab/pmx_data/tree/main/pmx_data/robot_execution_failures)                                             | Sensor data from a robot after 5 different types of failures                                                                        | Time to failure prediction         | Robotics                            |                                                             |
| [Air pressure system failures in Scania trucks.](https://github.com/autonlab/pmx_data/tree/main/pmx_data/scania_trucks_air_pressure_system_failure)      | Classifying whether truck failure is a result of its air pressure system                                                            | Tabular Failure Classification     | land_vehicles                       |                                                             |
| [solar power generation](https://github.com/autonlab/pmx_data/tree/main/pmx_data/solar_power_generation)                                                 | Power generation and weather data for 2 solar power plants                                                                          | Fault detection                    | Electrical                          |                                                             |
| [telemanom](https://github.com/autonlab/pmx_data/tree/main/pmx_data/telemanom)                                                                           | Telemetry data from 2 spacecraft with labeled anomalies in the testing set                                                          | Supervised Anomaly Detection       | Robotics                            |                                                             |
| [turbofan](https://github.com/autonlab/pmx_data/tree/main/pmx_data/turbofan)                                                                             | Multidimensional sensor data from simulated run to failure experiments                                                              | Time to event prediction           | Aircraft                            |                                                             |
| [Predictive Maintenance for Electrical Wiring Faults](https://github.com/autonlab/pmx_data/tree/main/pmx_data/wiring_dataset)                            | A dataset to support automatic optical inspection tool for electrical components using computer vision.                             | Image Fault Detection              | Electrical                          | Data is structured to be ready to used by a yolov5 network. |

## Downloading a Dataset

To download a dataset:

1. Navigate to that dataset's directory in this repository.
2. Download the get_data.sh script.
3. Run the get_data.sh script in the location where you would like to download the data.

This currently only works on Linux. Some get_data.sh scripts require additional steps before you can run them, which are described in a comment at the top of the file.

## Adding a Dataset

Steps to add a dataset to this repository:

1. If the dataset is not already hosted online: upload it to a data hosting site (we recommend [Mendeley](https://data.mendeley.com)).
2. Clone this repository to your local machine.
3. Make a copy of the [sample_dataset](https://github.com/autonlab/pmx_data/tree/main/sample_scripts/sample_dataset) directory within the pmx_data directory. This contains sample scripts to get you started.
4. Rename the directory to match the name of your dataset.
5. Modify the 'get_data.sh' script to download your data and unpack it into a standard csv format within a subfolder called 'datasets'.
6. Modify the 'info.yaml' file, filling in information about your dataset that will be used to generate a README.
7. Optional: Write a 'custom_writeup.md' markdown file containing any information about your dataset that is not encapsulated by info.yaml. This will be added to the generated README.
8. Optional: Write a 'load_data.py' sample script to load the data into a pandas dataframe or any other python object that is easy to work with ([this sample script](https://github.com/autonlab/pmx_data/blob/main/sample_scripts/load_data_recursive.py) works well in most instances).
9. Push your changes to the repository.

## Additional Resources

https://data.phmsociety.org/

https://www.nasa.gov/content/prognostics-center-of-excellence-data-set-repository

https://zenodo.org/

UCI repository https://archive.ics.uci.edu/ml/datasets.php

https://www.openml.org/

## Wishlist

- More image datasets, i.e. PmX with microscopy or aerial inspection.
- Tracking performance of different autoML tools on datasets over time.
- Support for multiple problem types on same dataset (for instance, fault detection can also be anomaly detection if you remove the target variable).
- Guide to pros and cons of different data hosting services (mendeley, kaggle, etc) for people who want to upload datasets.
- Allow for searching for datasets with different attributes or sorting by attribute.
- Github Pages GUI to make downloading and uploading easier for non-technical users.
- Support for downloading and unpacking data in Windows and MacOS.