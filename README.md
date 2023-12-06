# OVERVIEW.
Here is the project I did while studying this subject: Big Data Integration and Processing.
Topic: P2P Lending.
Since we were provided with infrastructure on the Google Cloud Platform during the course and I did all the work on it, after the end of the course we were not allowed access anymore. Unfortunately, I forgot to download these codes to my local machine so I just uploaded these documentation files to this project. Soon I will update the codes and post later.

# OVERALL ARCHITECTURE.
![image](https://github.com/adventurouscricket/p2p_lending_with_GCP/assets/19631259/6c42f697-15b9-420d-a8d2-fb294fe43d28)
Because my topic is not real-time, so I will adjust some things to be appropriate for my project.
![image](https://github.com/adventurouscricket/p2p_lending_with_GCP/assets/19631259/05db203c-1693-4ede-a424-04226a9cf64e)

What distinctions exist?
1.	I won’t utilize Flume, Kafka, or Pub/Sub along with the Speed Layer, as real-time processing isn't a requirement for this project.
2.	I will rearrange the sequence of steps, placing the Data Query step before the Elasticsearch step. I intend to employ Spark for data reading and processing before submitting it for storage in Elasticsearch.

# TOOLS, FRAMEWORKS.
![image](https://github.com/adventurouscricket/p2p_lending_with_GCP/assets/19631259/cc028ec5-93b6-4976-ac5d-35c40a9cde11)
•	Begin by employing Google Cloud Storage (GCS) to store the accumulated data.
•	Utilize Spark to retrieve data from GCS, carry out processing and comprehensive data analysis. Subsequently, send the resultant indexes to Elasticsearch.
•	Allow Elasticsearch to store the indexes provided during the second step.
•	Employ Kibana to create a dashboard with visually engaging representations for effective visualization.


