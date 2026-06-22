# Network Anomaly Detection

Multi-class classifier distinguishing normal network traffic from four 
categories of attack (DoS, Probe, Privilege Escalation, Access) using a 
Random Forest.

**Approach:** One-hot encoded categorical features (`protocol_type`, 
`service`), combined with numeric traffic statistics. Trained a 
`RandomForestClassifier` on the resulting feature set, with a held-out 
validation split for tuning and a separate test set for final evaluation.

**Dataset:** [NSL-KDD](https://www.unb.ca/cic/datasets/nsl.html) 
(refined version of KDD Cup 1999)

**Result:** ~99.5% weighted accuracy on the test set, though performance 
on minority classes (notably Privilege Escalation, the rarest category) 
was noticeably weaker — a good illustration of how class imbalance 
shows up in practice even when aggregate accuracy looks strong.
