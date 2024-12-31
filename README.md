# Higgs Data Analysis
Cascade Flow of Higgs Data Mentions 

This project processes and visualizes cascades of mentions in the Higgs dataset, where user interactions are tracked over time between pairs of users. By visualizing these interactions, we can analyze the flow and timing of mentions across a network, starting from a specified user and tracking each subsequent mention in a propagation cascade.
# Data Structure
The Higgs dataset consists of three main fields:
userA: The ID of the user initiating the interaction.
userB: The ID of the user receiving the interaction.
timestamp: The time of interaction (in Unix time).
# Example Row
Starting User
Timestamp
 User B , C , Z 
223789
1341100972
1341413739
1341445126
 B: 213163 , 
C: 66977, 
Z: 2994

This row represents an interaction where userA (223789) mentioned userB,C,Z (213163) at the timestamp of 1341100972 and other time in order.
# Features
Recursive Mention Tracking: Starting from a specified user, the program recursively tracks each mention, building a cascade of interactions that reveals the flow of mentions through the network.

Ordered Timestamps: Each mention interaction is ordered by timestamp, ensuring a time-accurate flow of interactions.

Graph Visualization: Visualizes the cascade of mentions in a directed graph, where nodes represent users and edges represent mention interactions, labeled by timestamps.


