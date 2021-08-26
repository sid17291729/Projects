# Anomaly Detection in Computer Networks
This project was done under the guidance of [Prof. Virendra Shekhawat](https://www.bits-pilani.ac.in/pilani/vsshekhawat/profile).
Our Aim was to detect intrusion in Computer Networks where an attack(an act of intrusion) can be classified as an anomaly. Our approach was similar to [this ](http://dm.snu.ac.kr/static/docs/TR/SNUDM-TR-2015-03.pdf).
Where we use a Variational Autoencoder to learn the latent representation of the normal instances and then compare the reconstruction with the original instance to check for anomalies.
We trained our model on the [KDD99](https://kdd.ics.uci.edu/databases/kddcup99/task.html) Data set.
