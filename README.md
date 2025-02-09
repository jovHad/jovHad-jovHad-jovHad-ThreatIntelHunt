# Threat Hunting Project: Detecting Anomalies in Computer Network Communication

This project focuses on analyzing a dataset of network traffic logs and packets to identify anomalies and potential threats, specifically Denial of Service (DoS) attacks. The analysis utilizes Python libraries such as pandas, numpy, matplotlib, scipy, and seaborn for data manipulation, statistical analysis, and visualization.

## Dataset

The dataset used for this analysis is the "DAPT 2020" dataset, which contains network traffic data collected over five days, with each day representing three months in a real-world scenario. The dataset is designed to help researchers understand anomalies and identify Advanced Persistent Threat (APT) attacks in their early stages.

## Methodology

The analysis involves the following steps:

1.  **Data Aggregation:** Grouping data by destination IP and 5-minute time slots to identify patterns and trends.
2.  **Outlier Detection:** Using statistical methods like the Interquartile Range (IQR) and Z-score to identify outliers in various network traffic features.
3.  **Attack Classification:** Developing rules and thresholds to classify potential DoS attacks based on the identified outliers and patterns.
4.  **Visualization:** Creating various plots and graphs to visualize the network traffic data, anomalies, and attack patterns.

## Key Findings

The analysis revealed a suspected SYN Flood attack within the dataset, characterized by:

*   A high SYN to ACK ratio, indicating incomplete handshake patterns
*   A significant spike in SYN packets at 15:15
*   An unusual point of SYN flag above 1200
*   No correlation between SYN and ACK flags
*   High Packet to Byte flow, indicating a lot of Syn Packets but no Payload

## Code

The code for this project is implemented in Python using Jupyter Notebook. It utilizes various libraries such as Pandas, Matplotlib, Seaborn, Numpy, and Scipy for data analysis and visualization. The code includes functions for data aggregation, outlier detection, attack classification, and visualization.

### Some of the Graphs to Display for Example:
   ![image](https://github.com/user-attachments/assets/a0a0254a-49a8-4716-9e54-599ac11d40c9)
   
   ![image](https://github.com/user-attachments/assets/fb733795-b15d-4def-bf38-7286e7535cde)

## Conclusion

This project successfully developed a framework for analyzing network traffic data and detecting potential DoS attacks. The analysis identified a SYN Flood attack within the dataset, highlighting the importance of proactive threat hunting and anomaly detection in maintaining network security.

## Future Work

*   Enhancing detection using AI-based anomaly detection  techniques and unsupervized Data Science methods.
*   Improving response strategies for customer service and incident handling.

## Author

Yovel Hadari

## Contact

yovela03@gmail.com
