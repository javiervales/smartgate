# A machine learning approach to improve RFID gate operation

<b> Abstract </b> <it>The aim of this work is to improve the operation of a UHF RFID gate using a supervised learning approach based on Artificial Neural Networks (ANNs). In our setup, we assume that boxes containing items are inventoried using an RFID gate with random perturbations in the box positions as well as random items inside boxes. The gate has two bistatic dislocated antenna pairs and, for each box, it is possible to choose a particular pair or mix both (the antenna selection policy). Based on the interrogation statistics (tags read and average received signal strength) from initial reference frames it is possible to obtain a signature of the interrogation process to predict the probability of identifying the whole batch of items contained in the box. Predictions are carried out using the ANN, which is trained with data generated using a simulator. This system can be used online to select the best policy during operation, in order to minimize the time penalties caused by inventory faults.</it>

## Paper materials

<ul>
  <li> <b>rfidml.ipynb</b> is the jupyter notebook for computing the predictive model, evaluate it and simulate the operation of the smartgate versus a normal gate
  <li> <b>modelrfid.h5</b> are the precomputed weights for the predictive neural network. This network outputs the expected batch identification policy using a given policy for the actual batch
  <li> <b>modelrfidR3_time_plm.h5</b> are the precomputed weights for the auxiliary neural network used to predict interrogation time in the smartgate simulator
  <li> <b>batches.txt</b> contains the simulatation results from the interrogation of 120000 tag batches with random placement, properties, and antennas selection policies
    </ul>
    
