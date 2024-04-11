# Realtime Climate Analysis Pipeline

## Overview
This repository contains a powerful realtime climate analysis pipeline leveraging various AWS services and Snowflake, along with Power BI for insightful visualizations. The pipeline is designed to ingest data from a weather API, store it in Dynamo DB, process it through AWS Lambda functions, store it in S3, and finally load it into Snowflake for further analysis. Python scripts are utilized for carrying out advanced analytics such as linear regression on the collected data.
![Realtime_Weather_Analalysis](https://github.com/ritikdhame/Realtime-Climate-Anlsyis/assets/7029092/a02d979c-9490-450d-a3f0-f4c47705998f)

## Features
- **Data Ingestion:** Utilizes AWS Lambda functions to ingest data from the Climate API into Dynamo DB.
- **Data Storage:** Dynamo DB is used as the primary data storage, with Dynamo DB streams used to trigger the ingestion of data into S3.
  ![Screenshot 2024-04-10 170332](https://github.com/ritikdhame/Realtime-Climate-Anlsyis/assets/7029092/099d064d-70a2-48df-8681-8fbebcafa9c5)

- **Data Processing:** Data stored in S3 is processed and loaded into Snowflake stages, followed by ingestion into Snowflake tables using Snowpipe.
- ![Screenshot 2024-04-10 170449](https://github.com/ritikdhame/Realtime-Climate-Anlsyis/assets/7029092/c930114b-bc12-4b9c-9179-5bb487ec2760)

- **Insightful Visualizations:** Leverages Power BI for building insightful visualizations comparing parameters such as humidity, temperature, pressure, and wind speed across multiple cities.
  ![Screenshot 2024-04-11 003924](https://github.com/ritikdhame/Realtime-Climate-Anlsyis/assets/7029092/5cc4f4b1-18e8-4b5b-a7ff-505f211043fa)
![Screenshot 2024-04-10 235552_PB2](https://github.com/ritikdhame/Realtime-Climate-Anlsyis/assets/7029092/962cc780-2c4e-4dca-bd78-9baee0632b3c)

- **Advanced Analytics:** Python scripts are employed for carrying out advanced analytics like linear regression on the collected data.
![image](https://github.com/ritikdhame/Realtime-Climate-Anlsyis/assets/7029092/88e9be61-c5f1-4421-a363-8abff27b8ae7)
-instance prediction of Temprature with XGBoost Model
![image](https://github.com/ritikdhame/Realtime-Climate-Anlsyis/assets/7029092/2d776c68-9afa-4f87-a71a-8b522e973ab7)

- **Optimization and Scaling:** Provides best practices for optimizing and scaling the data pipeline to enhance performance, ensure data integrity, and accommodate evolving project needs.
- **Troubleshooting and Best Practices:** Equips users with troubleshooting skills and industry best practices to overcome common challenges in real-world scenarios, ensuring the reliability and resilience of the data pipeline.
- **Advanced Concepts and Future Trends:** Explores advanced concepts and emerging trends in AWS Data Engineering, keeping users updated with the latest technologies and potential impacts on data engineering practices.

## Installation
1. Clone this repository to your local machine.
2. Install the required dependencies mentioned in `requirements.txt`.
3. Configure AWS credentials and permissions for accessing AWS services.
4. Set up Snowflake credentials for connecting to Snowflake.

## Usage
1. Run the Lambda functions to ingest data from the Climate API into Dynamo DB.
2. Monitor Dynamo DB streams for changes and trigger the ingestion of data into S3.
3. Process the data stored in S3 and load it into Snowflake stages.
4. Ingest the data from Snowflake stages into Snowflake tables using Snowpipe.
5. Utilize Power BI for building insightful visualizations and analytics.
6. Execute Python scripts for advanced analytics like linear regression & XGboost Models for prediction.

## Contributing
Contributions are welcome! Feel free to open issues or pull requests for any improvements or new features.

## License
This project is licensed under the [MIT License](LICENSE).

## Acknowledgements
- Thanks to [Climate API](https://www.climate.com/) for providing the weather data.
- This project was inspired by the need for real-time climate analysis and the power of AWS and Snowflake in handling large-scale data pipelines.

## Contact
For any inquiries or support, please contact [your@email.com].
