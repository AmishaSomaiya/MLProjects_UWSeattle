5G cellular technology is designed to increase speed, reduce latency, and improve flexibility of wireless 
services. Both 5G and MIMO(Multiple Input Multiple Output) utilize radio frequencies in the sub-6 GHz range and the 
millimeter-wave (mmWave) frequency range (30-300GHz). These smaller wavelengths (in millimeters) 
allow to design tinier antennas and, in turn, pack many more at both transmitter and receiver ends. Thus, there are multiple 
antenna array elements at both the transmitter and receiver ends. Selecting the best beam pair out of these becomes essential 
for maximum information gain. To unleash the full power of mmWave communications, a prominent challenge consists in 
reducing the overhead introduced by the beam selection (or alignment) procedures. 

This project proposes a machine learning 
algorithm to reduce this overhead using XGBoost with SMOTE. The data used is from the Raymobtime datasets s008 and s009
with GPS, LiDAR, and image input features. The proposed algorithm outputs a prediction of top k(k=10) best beam pairs 
for every receiver input, thus providing the communication system with a complementary, out-of-band information to reduce 
the processing overhead. The final model combats overfitting with early stopping and uses random search 
cross-validation for hyperparameter tuning. The proposed algorithm has a top 10 accuracy of 94.2%, beating the SOA by 
3.2% and has a computational cost of 0.25 hours, which is 3x lesser than SoA. Also, the proposed algorithm reaches accuracy 
of 98% early at k=20 instead of at k=30 for SoA. The top 20 accuracy with SMOTE to reduce minority class misclassifications
is reasonable at 96.5%.

