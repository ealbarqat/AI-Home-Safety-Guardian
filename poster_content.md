# AI Home Safety Guardian: Predictive Risk Monitoring for Seniors
## Poster Content for Master's Level Presentation

---

## TITLE SECTION

**AI Home Safety Guardian: Predictive Risk Monitoring for Seniors**

*An IoT-Enhanced AI Solution for Independent Elderly Living in Luxembourg and the Greater Region*

**Authors:** Parsa AKBARI CHIANEH, Esraa ALBARAQAT, Katarina BOŽIČ

**University:** University of Luxembourg

**Supervisor:** Prof. Christoph SCHOMMER

**Date:** December 2025

---

## 1. ABSTRACT

Independent living for elderly populations is increasingly prioritized across Europe, particularly in Luxembourg where rural elderly communities face challenges in accessing immediate care. According to Luxembourg's national statistics (STATEC), approximately 19.5% of the population is over 65 years, with many residing in dispersed rural areas. This project proposes an AI-powered home safety monitoring system that integrates Internet of Things (IoT) sensors with machine learning algorithms to predict and prevent domestic accidents among seniors living alone.

The system employs non-intrusive environmental sensors—temperature, gas detection, passive infrared (PIR) motion sensors, and electricity consumption monitors—to analyze behavioral patterns. Through time-series analysis using Long Short-Term Memory (LSTM) networks and Gated Recurrent Units (GRU), the system establishes individualized behavioral baselines. Anomaly detection algorithms including Isolation Forest, One-Class Support Vector Machines (OC-SVM), and Autoencoders identify deviations indicating potential emergencies such as falls, forgotten appliances, or unusual inactivity periods.

The proposed methodology employs a three-tier architecture: (1) edge computing for local sensor data processing, (2) cloud-based storage and advanced analytics, and (3) real-time alert generation via multi-level notification systems. This solution addresses the growing need for non-intrusive, privacy-preserving care assistance in the Greater Region, while maintaining elderly autonomy and dignity through GDPR-compliant data handling and transparency mechanisms.

**Keywords:** Elderly Care, IoT, Anomaly Detection, Predictive Analytics, Home Safety, Luxembourg, GDPR-Compliant Monitoring, LSTM, Time-Series Analysis

---

## 2. INTRODUCTION & MOTIVATION

### Problem Statement

Luxembourg faces significant demographic challenges with its aging population. Recent statistics indicate that approximately 19.5% of residents are over 65 years of age, with a projected increase to 26% by 2050 (STATEC, 2024). This demographic shift coincides with a growing preference for independent living among elderly individuals, particularly in rural areas where access to immediate care is limited.

Traditional monitoring solutions present several limitations: (1) constant video surveillance raises substantial privacy concerns and violates GDPR principles, (2) wearable devices face compliance issues and user resistance, particularly among elderly populations who may find them uncomfortable or stigmatizing, and (3) existing systems lack predictive capabilities, operating reactively rather than preventively.

The most common home accidents among elderly populations include: falls (accounting for approximately 40% of home accidents), fire hazards from forgotten appliances (15%), gas leaks (8%), and health emergencies indicated by unusual inactivity patterns (37% of unassisted living situations).

### Relevance for Luxembourg & Greater Region

**Geographic Context:** Luxembourg's dispersed rural population creates unique access challenges. Elderly residents in municipalities such as Vianden, Wiltz, and Clervaux face average emergency response times of 15-20 minutes, compared to 5-7 minutes in urban areas like Luxembourg City.

**Economic Factor:** Healthcare expenditures for elderly care in Luxembourg have increased by 12% annually over the past five years. Preventive monitoring solutions could reduce emergency interventions by an estimated 30-40%, resulting in significant cost savings for both families and the national healthcare system.

**Social Dimension:** Luxembourg's cross-border workers and internationally mobile population often results in elderly family members living alone while relatives work in neighboring countries (Belgium, France, Germany). Remote monitoring systems can bridge geographic distances and provide peace of mind.

**Regulatory Environment:** Luxembourg's strong GDPR framework and proactive stance on digital health initiatives make it an ideal testbed for privacy-compliant AI solutions. The Luxembourg National Commission for Data Protection (CNPD) provides clear guidance on AI deployment in healthcare contexts.

**Scalability:** The Greater Region (Luxembourg, Belgium, France, Germany border areas) shares similar demographic trends and regulatory frameworks, making regional deployment feasible.

---

## 3. OBJECTIVES

### Primary Objectives

1. **Develop a Non-Intrusive Monitoring System**
   - Design and implement an IoT sensor network using non-wearable, environmental sensors (temperature, motion, gas, electricity consumption)
   - Ensure zero use of cameras or microphones to eliminate privacy concerns associated with continuous surveillance
   - Achieve 99.5% system uptime through redundant edge computing infrastructure

2. **Implement AI Algorithms for Real-Time Anomaly Detection**
   - Deploy time-series analysis models (LSTM/GRU networks) with >95% accuracy in baseline pattern recognition
   - Implement ensemble anomaly detection combining Isolation Forest, OC-SVM, and Autoencoders to achieve <5% false positive rate
   - Develop predictive risk scoring algorithms that identify subtle pattern changes preceding accidents by 15-30 minutes

3. **Ensure GDPR Compliance and Ethical Standards**
   - Implement data minimization strategies: collect only sensor readings (no personal identifiers)
   - Achieve full GDPR Article 6 compliance through legitimate interest and explicit consent mechanisms
   - Conduct Privacy Impact Assessment (DPIA) before deployment
   - Enable user rights: access, rectification, erasure, and data portability

4. **Validate System Effectiveness**
   - Deploy pilot system in 20-30 elderly households in Luxembourg rural areas
   - Achieve >90% detection accuracy for critical events (falls, gas leaks, forgotten appliances)
   - Maintain <5% false positive rate to prevent alert fatigue
   - Achieve >80% user satisfaction rate among pilot participants

### Secondary Objectives

5. **Establish Scalability Framework**
   - Design modular system architecture for deployment across diverse home environments
   - Create documentation and protocols for regional expansion to Greater Region

6. **Generate Research Contributions**
   - Publish methodology on privacy-preserving elderly care AI systems
   - Contribute to academic literature on non-invasive anomaly detection for health monitoring

---

## 4. SCOPE

### Geographic Scope

**Primary Focus:** Luxembourg, with initial pilot deployment in rural municipalities:
- Northern regions: Clervaux, Wiltz, Vianden
- Eastern regions: Echternach, Grevenmacher
- Target: 20-30 pilot households in year 1

**Secondary Focus (Future):** Greater Region expansion:
- Border regions in Belgium (Province of Luxembourg)
- Border regions in France (Moselle department)
- Border regions in Germany (Trier-Saarburg district)

### Technical Scope

**Included Components:**
- IoT sensor deployment: temperature sensors (±0.1°C accuracy, 1-minute sampling rate)
- Passive Infrared (PIR) motion sensors (3-5 meter detection range, installed in common areas: kitchen, living room, hallway)
- Gas detection sensors (CO/CH4 detection with 50 ppm sensitivity threshold)
- Smart plugs for electricity consumption monitoring (Watt-level granularity)
- Edge computing devices (Raspberry Pi 4 or equivalent, 4GB RAM, local processing)
- Cloud infrastructure (Luxembourg-based servers for GDPR compliance)
- Mobile/web dashboard for family/caregiver notifications
- Real-time alert system (SMS, push notifications, email)

**Excluded Components:**
- Cameras or video surveillance equipment
- Microphones or audio recording devices
- Wearable devices (fitness trackers, smartwatches)
- Direct integration with medical devices (blood pressure monitors, glucose meters) - future consideration
- Continuous 24/7 video monitoring systems

### Functional Scope

**Supported Use Cases:**
1. Fall detection: Identify sudden cessation of movement patterns
2. Forgotten appliance detection: Detect extended high electricity consumption without movement
3. Unusual inactivity alerts: Flag deviations from established daily activity baselines
4. Gas leak detection: Immediate binary alerts for gas sensor threshold violations
5. Temperature anomalies: Detect patterns indicating fever, hypothermia, or heating issues

**Not Supported (Out of Scope):**
- Medical diagnosis or health condition assessment
- Medication adherence monitoring
- Social interaction or communication facilitation
- Meal preparation assistance
- Medication reminders (future consideration)

### Temporal Scope

**Phase 1 (Months 1-3):** Prototype development and initial sensor deployment
- Hardware procurement and configuration
- Baseline data collection (4-6 weeks per household)
- Initial model training

**Phase 2 (Months 4-6):** Model refinement and validation
- Algorithm comparison and selection
- Cross-validation on held-out data
- Threshold optimization

**Phase 3 (Months 7-12):** Pilot deployment and evaluation
- Expanded deployment to 20-30 households
- Real-world performance monitoring
- User feedback collection and system refinement

**Phase 4 (Year 2+):** Regional expansion and commercialization
- Greater Region deployment
- Integration with healthcare systems
- Partnership development

### Data Scope

**Data Types Collected:**
- Temperature readings: Continuous, 1-minute intervals, ±0.1°C precision
- Motion sensor data: Binary events (movement detected/non-detected), timestamped
- Electricity consumption: Aggregated watt-hour readings per 15-minute windows
- Gas sensor data: Binary alerts only (threshold exceeded/not exceeded), no continuous monitoring
- Derived features: Computed patterns (activity levels, energy usage trends, temperature variations)

**Data Retention:**
- Raw sensor data: 30 days for model refinement
- Aggregated patterns: 365 days for baseline maintenance
- Alert events: Permanent (required for system validation)

**Privacy Boundaries:**
- No personally identifiable information (PII) collected
- No behavioral data shared with third parties beyond family/caregivers
- No integration with commercial data brokers or advertisers

---

## 5. METHODOLOGY

### 5.1 System Architecture

The system employs a hierarchical architecture with three distinct layers:

```
┌─────────────────────────────────────────────────────────────────┐
│                    IoT Sensor Layer (Edge)                       │
│  • DHT22 Temperature/Humidity Sensors (kitchen, bedroom)       │
│  • PIR Motion Sensors (living room, hallway, bathroom)          │
│  • MQ-2/MQ-5 Gas Detection Sensors (kitchen)                    │
│  • TP-Link HS110 Smart Plugs (stove, refrigerator, TV)         │
│  • Communication: WiFi 802.11n, sampling rate: 1 Hz            │
└─────────────────────────────────────────────────────────────────┘
                              ↓
┌─────────────────────────────────────────────────────────────────┐
│              Edge Computing & Preprocessing Layer                 │
│  Hardware: Raspberry Pi 4 (4GB RAM, Quad-core CPU)             │
│  • Real-time data acquisition (Python, paho-mqtt library)      │
│  • Local preprocessing: normalization, missing value imputation │
│  • Feature extraction: temporal windows (15-min, 1-hour, 24-hour)│
│  • Edge inference: Lightweight anomaly detection models        │
│  • Data encryption: AES-256 before cloud transmission          │
└─────────────────────────────────────────────────────────────────┘
                              ↓
┌─────────────────────────────────────────────────────────────────┐
│              Cloud Storage & Advanced Analytics Layer            │
│  Infrastructure: Luxembourg-based cloud (AWS EU-Central-1)     │
│  • Secure data storage: encrypted PostgreSQL database           │
│  • Time-series database: InfluxDB for sensor data              │
│  • Model training: GPU-enabled instances (NVIDIA T4)           │
│  • Batch processing: historical pattern analysis                │
│  • API endpoints: RESTful services for dashboard access         │
└─────────────────────────────────────────────────────────────────┘
                              ↓
┌─────────────────────────────────────────────────────────────────┐
│                 Decision & Alert System Layer                   │
│  • Risk scoring engine: ensemble of anomaly detection models    │
│  • Multi-level alerts: Low (email), Medium (SMS), High (call)   │
│  • Notification channels: Twilio SMS API, SendGrid email       │
│  • Dashboard: React.js web app, React Native mobile app        │
│  • Integration: Emergency services API (future consideration)  │
└─────────────────────────────────────────────────────────────────┘
```

### 5.2 AI/ML Components

#### 5.2.1 Time-Series Pattern Learning

**LSTM Network Architecture:**
- **Purpose:** Learn temporal dependencies in daily activity patterns
- **Architecture:** 
  - Input layer: 24-hour sliding window (1440 timesteps, 4 features: temp, motion, electricity, gas_binary)
  - LSTM layer 1: 128 units with dropout (0.2)
  - LSTM layer 2: 64 units with dropout (0.2)
  - Dense layer: 32 units, ReLU activation
  - Output layer: 4 units (predicted values for each sensor)
- **Training:** 
  - Baseline period: 4-6 weeks of continuous data collection
  - Loss function: Mean Squared Error (MSE)
  - Optimizer: Adam (learning rate: 0.001)
  - Batch size: 32, epochs: 100 with early stopping
- **Implementation:** TensorFlow 2.12, Keras API

**GRU Alternative:**
- Similar architecture to LSTM but using Gated Recurrent Units (faster training, comparable performance)
- 96 units per layer (fewer parameters than LSTM)
- Used for comparison in ensemble approach

#### 5.2.2 Anomaly Detection Algorithms

**1. Isolation Forest:**
- **Purpose:** Detect outliers in multi-dimensional sensor data without requiring labeled anomaly data
- **Parameters:** 
  - Number of estimators: 100
  - Max samples: 256
  - Contamination rate: 0.05 (5% expected anomaly rate)
- **Implementation:** scikit-learn IsolationForest
- **Advantage:** Unsupervised learning, handles high-dimensional data efficiently

**2. One-Class Support Vector Machine (OC-SVM):**
- **Purpose:** Learn decision boundary around normal behavior, flag deviations
- **Parameters:**
  - Kernel: Radial Basis Function (RBF)
  - Nu: 0.05 (upper bound on fraction of outliers)
  - Gamma: 'scale' (automatic kernel coefficient scaling)
- **Implementation:** scikit-learn OneClassSVM
- **Advantage:** Flexible kernel selection, handles non-linear patterns

**3. Autoencoder (Deep Learning):**
- **Purpose:** Learn compressed representation of normal patterns; high reconstruction error indicates anomalies
- **Architecture:**
  - Encoder: Input (1440, 4) → Dense(512, ReLU) → Dense(256, ReLU) → Latent(128)
  - Decoder: Latent(128) → Dense(256, ReLU) → Dense(512, ReLU) → Output(1440, 4)
  - Loss: Mean Absolute Error (MAE) - more robust to outliers than MSE
  - Threshold: 95th percentile of reconstruction error on validation set
- **Implementation:** TensorFlow/Keras
- **Advantage:** Captures complex non-linear patterns, unsupervised feature learning

**Ensemble Approach:**
- Combine predictions from all three methods
- Voting mechanism: Anomaly if ≥2 models flag event as anomalous
- Weighted scoring: Isolation Forest (0.4), OC-SVM (0.3), Autoencoder (0.3)
- Final risk score: Normalized to 0-1 scale (0.8+ triggers high-priority alert)

#### 5.2.3 Predictive Risk Modeling

**Composite Risk Score Calculation:**
```
Risk_Score = α₁ × Motion_Anomaly + α₂ × Temperature_Anomaly + 
             α₃ × Electricity_Anomaly + α₄ × Temporal_Deviation

Where:
- Motion_Anomaly: Binary (0/1) or continuous score from ensemble
- Temperature_Anomaly: Normalized deviation from baseline (±2°C threshold)
- Electricity_Anomaly: Duration of high consumption without movement (hours)
- Temporal_Deviation: Time-of-day mismatch with baseline pattern
- α₁=0.4, α₂=0.2, α₃=0.2, α₄=0.2 (weights learned from validation set)
```

**Early Warning System:**
- Monitor trend changes over 15-minute, 1-hour, and 24-hour windows
- Flag gradual pattern shifts before critical events occur
- Example: Decreasing activity levels over 3 days may indicate health decline

### 5.3 Detection Logic for Specific Use Cases

#### Use Case 1: Fall Detection

**Detection Algorithm:**
1. Monitor PIR motion sensors in common areas (living room, hallway, kitchen)
2. Baseline: Average movement events per hour during active periods (typically 6-22:00)
3. Anomaly trigger:
   - Sudden cessation: No movement detected for >30 minutes during active period
   - AND: Last movement was in common area (not bedroom)
   - AND: Current time is not within normal sleep window (baseline ±2 hours)
4. Confirmation: Cross-check with electricity consumption (no appliance activity)
5. Alert generation: High-priority alert if all conditions met

**Expected Performance:**
- True Positive Rate: 92% (based on literature)
- False Positive Rate: <3% (tuned via threshold optimization)

#### Use Case 2: Forgotten Stove/Appliance Detection

**Detection Algorithm:**
1. Monitor smart plug on stove (if applicable) OR kitchen electricity consumption
2. Baseline: Average electricity consumption patterns for cooking periods
3. Anomaly trigger:
   - High electricity consumption (>1500W) for >2 hours continuously
   - AND: No corresponding motion sensor activity in kitchen for >30 minutes
   - AND: Temperature sensor in kitchen shows elevated readings (>25°C above ambient)
4. Gas sensor confirmation: If MQ-2 sensor detects gas, immediate high-priority alert
5. Alert generation: Medium-priority alert initially, escalates to high if gas detected

#### Use Case 3: Unusual Inactivity Detection

**Detection Algorithm:**
1. Establish daily activity baseline using LSTM network:
   - Movement events per hour (hourly bins)
   - Electricity usage patterns
   - Temporal features: time-of-day, day-of-week
2. Real-time monitoring: Compare current 24-hour window to predicted baseline
3. Anomaly trigger:
   - Activity level <50% of predicted baseline for >6 hours
   - OR: No movement detected for >8 hours (excluding sleep hours)
4. Contextual validation: Check if deviation is consistent with known patterns (illness, travel)
5. Alert generation: Low-priority initial alert, escalates based on duration

### 5.4 Data Processing Pipeline

**Stage 1: Data Acquisition (Edge Layer)**
- Sensor sampling rate: 1 Hz (1 reading per second)
- Local buffering: 5-minute windows before transmission
- Data format: JSON with timestamp, sensor_id, value, unit
- Preprocessing: Outlier removal (3-sigma rule), missing value imputation (forward-fill)

**Stage 2: Feature Engineering**
- **Temporal features:**
  - Hour of day (sine/cosine encoding for cyclical nature)
  - Day of week (one-hot encoding)
  - Weekend/weekday indicator
- **Statistical features (15-minute windows):**
  - Mean, standard deviation, min, max for each sensor
  - Trend: linear regression slope
  - Variance ratio: current window vs. historical average
- **Cross-sensor features:**
  - Correlation coefficient: motion vs. electricity consumption
  - Lag features: temperature vs. motion (1-hour lag)

**Stage 3: Model Inference**
- Real-time inference: Every 15 minutes on rolling windows
- Batch inference: Daily pattern analysis for baseline updates
- Model versioning: A/B testing for model improvements
- Performance monitoring: Track inference latency (<500ms target)

**Stage 4: Alert Generation**
- Risk score thresholding:
  - Low alert: Risk score 0.6-0.7 (email notification)
  - Medium alert: Risk score 0.7-0.8 (SMS notification)
  - High alert: Risk score >0.8 (SMS + phone call)
- Deduplication: Suppress repeated alerts for same event within 1-hour window
- Escalation: If high-priority alert unacknowledged for >30 minutes, notify emergency contact

### 5.5 Technical Implementation Details

**Hardware Specifications:**
- Edge Device: Raspberry Pi 4 Model B (4GB RAM, 32GB microSD)
- Sensors:
  - Temperature: DHT22 (±0.5°C accuracy, -40 to 80°C range, €5/unit)
  - Motion: HC-SR501 PIR sensor (3-7m range, 120° detection angle, €3/unit)
  - Gas: MQ-2 (LPG, propane, methane) or MQ-5 (natural gas), €4/unit
  - Electricity: TP-Link HS110 smart plug (WiFi, energy monitoring, €25/unit)
- Network: WiFi 802.11n router (minimum requirement)

**Software Stack:**
- Operating System: Raspberry Pi OS (Debian-based, Linux 5.15+)
- Programming: Python 3.10+
- ML Frameworks: TensorFlow 2.12, scikit-learn 1.3.0
- Data Processing: Pandas 2.0, NumPy 1.24
- Communication: paho-mqtt (MQTT protocol), requests (HTTP API)
- Database: PostgreSQL 15 (cloud), InfluxDB 2.7 (time-series)
- Web Framework: FastAPI (backend API), React.js (frontend dashboard)
- Deployment: Docker containers, Kubernetes (cloud orchestration)

**Security Implementation:**
- Data Encryption:
  - In-transit: TLS 1.3 for all network communications
  - At-rest: AES-256 encryption for database storage
- Authentication: OAuth 2.0 for dashboard access, API key rotation every 90 days
- Access Control: Role-based access (elderly user, family member, caregiver, administrator)
- Audit Logging: All data access events logged for compliance

**Cost Estimates (Per Household):**
- Hardware: €150-200 (one-time)
- Cloud infrastructure: €15-25/month (data storage, compute, API services)
- Communication: €5-10/month (SMS alerts)
- **Total per household: €170-235 one-time + €20-35/month**

---

## 6. EXPECTED RESULTS & IMPACT

### 6.1 Quantitative Metrics

**Detection Performance:**
- **Fall Detection Accuracy:** Target >90% true positive rate (TPR), <5% false positive rate (FPR)
  - Baseline comparison: Existing wearable devices achieve ~85% TPR with 8-12% FPR
  - Expected improvement: Non-intrusive approach reduces user compliance issues
- **Forgotten Appliance Detection:** Target >95% accuracy (higher due to clear signal patterns)
- **Unusual Inactivity Detection:** Target >85% accuracy (more challenging due to variable baselines)

**System Performance:**
- **Latency:** Alert generation <2 minutes from anomaly detection
- **Uptime:** 99.5% system availability (target)
- **Data Processing:** Real-time inference <500ms per 15-minute window
- **Scalability:** System designed to support 10,000+ concurrent households

**User Experience Metrics:**
- **User Satisfaction:** Target >80% satisfaction rate (measured via surveys)
- **Technology Adoption:** Target >75% of pilot participants continue using after 6 months
- **False Alert Tolerance:** <5 alerts per week per household (to prevent alert fatigue)

**Healthcare Impact:**
- **Accident Reduction:** Target 30-40% reduction in domestic accidents (falls, fires, gas incidents)
  - Based on literature review: Similar systems achieve 25-35% reduction
  - Luxembourg-specific context may achieve higher due to preventive nature
- **Emergency Response Time:** Average improvement of 10-15 minutes (earlier detection)
- **Hospitalization Reduction:** Estimated 15-20% reduction in fall-related hospitalizations

### 6.2 Qualitative Impact

**For Elderly Users:**
- **Independence Extension:** Enable 1-2 years longer independent living (based on literature)
- **Peace of Mind:** Enhanced sense of security without feeling "watched"
- **Dignity Preservation:** Non-intrusive approach maintains autonomy and privacy
- **Quality of Life:** Reduced anxiety about potential accidents

**For Families/Caregivers:**
- **Reduced Burden:** Less frequent physical check-ins required
- **Remote Reassurance:** Real-time visibility into elderly relative's well-being
- **Geographic Flexibility:** Effective monitoring regardless of distance
- **Early Intervention:** Ability to respond to subtle pattern changes before emergencies

**For Healthcare System:**
- **Cost Savings:** Estimated €500-800 per household annually (reduced emergency interventions)
- **Resource Optimization:** Shift from reactive to preventive care model
- **Data-Driven Insights:** Aggregate patterns inform public health policy

### 6.3 Social Impact

**Aging in Place Support:**
- Aligns with Luxembourg's policy goal of enabling elderly to age in their homes
- Reduces pressure on assisted living facilities (waitlist reduction)
- Supports community-based care models

**Rural Health Equity:**
- Addresses disparity in access to immediate care between urban and rural areas
- Reduces healthcare access inequality
- Strengthens rural community resilience

**Digital Inclusion:**
- Minimal technology interaction required from elderly users (fully automated)
- No smartphone or computer skills necessary
- Reduces digital divide concerns

### 6.4 Scientific Contribution

**Methodological Innovation:**
- Novel ensemble approach combining LSTM, Isolation Forest, OC-SVM, and Autoencoders
- Privacy-preserving anomaly detection without labeled data
- Individualized baseline learning from limited initial data (4-6 weeks)

**Privacy-Preserving AI Framework:**
- Model for GDPR-compliant elderly care monitoring
- Edge computing architecture minimizing cloud data transmission
- Data minimization strategies applicable to other healthcare AI applications

**Predictive Care Paradigm:**
- Shift from reactive (incident after occurrence) to proactive (prediction before incident)
- Early warning system for health decline indicators
- Scalable framework for preventive healthcare technology

---

## 7. CHALLENGES & ETHICS

### 7.1 Technical Challenges

**1. Baseline Learning Period**
- **Challenge:** Requiring 4-6 weeks of data collection before system becomes effective creates initial vulnerability period
- **Mitigation:** Use population-level baselines as initial estimates, gradually personalize
- **Future Work:** Transfer learning from similar households to reduce baseline period

**2. False Positive Rate Management**
- **Challenge:** Too many false alerts lead to alert fatigue and user trust erosion
- **Mitigation:** Multi-level confirmation before alert generation, adaptive threshold tuning based on user feedback
- **Target:** Maintain <5% false positive rate through continuous model refinement

**3. Sensor Reliability and Failure Detection**
- **Challenge:** Sensor malfunctions can create blind spots or false alarms
- **Mitigation:** Redundant sensors in critical areas, automated health checks, alert family if sensor offline >24 hours
- **Monitoring:** Track sensor uptime, battery life (if applicable), communication failures

**4. Internet Connectivity Dependency**
- **Challenge:** Rural areas may have unreliable internet connectivity
- **Mitigation:** Edge computing for local processing, buffering alerts until connectivity restored, cellular backup (4G/5G modem option)
- **Limitation:** Some remote areas may require infrastructure investment

**5. Algorithmic Bias and Generalization**
- **Challenge:** Models trained on limited pilot data may not generalize to diverse elderly populations (different routines, cultural backgrounds, living situations)
- **Mitigation:** Diverse pilot participant selection, continuous learning with privacy safeguards, regular model validation on new data
- **Ethical Consideration:** Ensure equitable performance across demographic groups

### 7.2 Data & GDPR Challenges

**1. Health Data Classification**
- **Challenge:** Some behavioral patterns (activity levels, sleep patterns) may constitute health data under GDPR Article 9, requiring special conditions
- **Solution:** 
  - Minimize data collection to environmental sensors only
  - Avoid inferring specific health conditions (focus on safety events only)
  - If health data classification unavoidable: Rely on Article 9(2)(h) - healthcare purposes, or Article 9(2)(a) - explicit consent
  - Regular DPIA updates as system evolves

**2. Consent Validity for Elderly Users**
- **Challenge:** Ensuring elderly individuals have capacity to give informed consent, particularly those with cognitive decline
- **Solution:**
  - Clear, accessible consent forms (multiple languages, large print)
  - Involvement of family members/caregivers in consent process
  - Option for legal guardian consent if individual capacity in question
  - Regular consent renewal (annual)

**3. Third-Party Access (Family Members)**
- **Challenge:** Balancing privacy of elderly individual with family's need for information
- **Solution:**
  - Granular access controls: Family can view alerts but not raw sensor data
  - Elderly user controls which family members receive alerts
  - Audit logging of all data access

**4. International Data Transfers**
- **Challenge:** If using cloud services outside EU, must ensure GDPR adequacy
- **Solution:**
  - Prioritize Luxembourg/EU-based cloud providers (AWS EU-Central-1, Azure Europe)
  - If non-EU transfer necessary: Standard Contractual Clauses (SCCs) with data processing agreements
  - Minimize data transfer: Edge computing reduces cloud transmission

**5. Data Retention and Deletion**
- **Challenge:** Balancing data retention for model improvement vs. privacy minimization
- **Solution:**
  - Clear retention policies: Raw data 30 days, aggregates 365 days
  - Automated deletion after retention period
  - User right to immediate deletion (Article 17 GDPR)

### 7.3 Ethical Considerations

**Autonomy vs. Surveillance Tension**

**Respecting Autonomy:**
- **Transparency:** Clear explanation of what data is collected, how it's used, and when alerts are generated
- **User Control:** 
  - Elderly user can disable monitoring at any time
  - Adjustable alert thresholds (within safety bounds)
  - Choice of notification recipients
- **Dignity:** System operates in background without requiring user interaction or compliance

**Surveillance Concerns:**
- **Minimal Intrusion:** No cameras or microphones eliminates most privacy concerns
- **Purpose Limitation:** Data used solely for safety monitoring, not for other purposes (cost-saving, insurance assessment)
- **Bounded Monitoring:** Respect privacy zones (bedroom during sleep hours - reduced monitoring, no alerts unless critical)
- **Transparency to Users:** Users always know when system is active and what it's detecting

**Social Implications**

**Digital Divide:**
- **Challenge:** Technology-averse elderly may be excluded
- **Mitigation:** Fully automated system requires no user interaction, professional installation service available

**Family Dynamics:**
- **Positive:** Reduced anxiety for distant family members, enables more frequent but less intrusive connection
- **Negative:** Potential for over-reliance on technology, reduction in personal visits/interaction
- **Mitigation:** System designed to complement, not replace, human care and interaction

**Inequality:**
- **Challenge:** Initial cost may create divide between those who can afford and those who cannot
- **Mitigation:** 
  - Explore insurance/healthcare system partnerships for subsidized deployment
  - Government funding for vulnerable populations
  - Community-based models (shared infrastructure)

**Dependency Risk:**
- **Challenge:** Over-reliance on technology reducing human interaction
- **Mitigation:** System alerts prompt human interaction (family calls to check in), not replace it

### 7.4 Risk Assessment

**Critical Risks:**

**1. False Negatives (Missed Emergencies)**
- **Impact:** Fatal - missing a real emergency could have life-threatening consequences
- **Probability:** Low (<1% based on literature) but catastrophic impact
- **Mitigation:**
  - Redundant detection mechanisms (multiple algorithms, multiple sensors)
  - Regular system testing and validation
  - Clear disclaimers: System is assistive, not replacement for emergency services
  - User education: Maintain emergency buttons/call systems as backup

**2. Data Breach**
- **Impact:** High - exposure of behavioral patterns could enable profiling, discrimination
- **Probability:** Medium (depending on security measures)
- **Mitigation:**
  - Strong encryption (AES-256), secure authentication (OAuth 2.0)
  - Regular security audits, penetration testing
  - Breach response plan (notification within 72 hours as required by GDPR)
  - Cyber insurance coverage

**3. System Failure During Critical Moment**
- **Impact:** High - system offline when emergency occurs
- **Probability:** Low (99.5% uptime target)
- **Mitigation:**
  - Redundant infrastructure, failover mechanisms
  - Health monitoring: Alert users if system offline >24 hours
  - Battery backup for edge devices (UPS)

**4. Legal Liability**
- **Impact:** Medium - who is responsible if system fails to detect critical event?
- **Probability:** Low but increasing as AI systems become more common
- **Mitigation:**
  - Clear terms of service: System is assistive tool, not replacement for human care
  - Regular model validation and documentation
  - Liability insurance
  - Compliance with emerging EU AI Act requirements

### 7.5 Mitigation Strategies Summary

**Technical:**
- Redundant sensors and algorithms
- Continuous model monitoring and improvement
- Edge computing for reliability
- Regular system health checks

**Privacy/GDPR:**
- Data minimization (only essential sensors)
- Encryption and secure access controls
- Clear consent processes
- Regular DPIA updates

**Ethical:**
- Transparency and user control
- Purpose limitation
- Respect for autonomy
- Community engagement and feedback

**Risk Management:**
- Comprehensive testing before deployment
- Clear disclaimers and liability terms
- Insurance coverage
- Emergency backup systems

---

## 8. REFERENCES

### Academic References

1. **Gabrielli, D., Prenkaj, B., Velardi, P., & Faralli, S. (2025).** AI on the Pulse: Real-Time Health Anomaly Detection with Wearable and Ambient Intelligence. *arXiv preprint arXiv:2508.03436.*
   - **Relevance:** Provides framework for real-time health anomaly detection combining wearable and ambient sensors, applicable to our elderly monitoring approach.

2. **Shahid, Z. K., Saguna, S., & Åhlund, C. (2024).** Detecting Anomalies in Daily Activity Routines of Older Persons in Single Resident Smart Homes: Proof-of-Concept Study. *JMIR Aging, 7, e58394.*
   - **Relevance:** Validates anomaly detection in smart home environments for elderly, demonstrating feasibility of non-wearable sensor approaches.

3. **Reddy, M. V. K., Lathigara, A., & Reddy, N. H. (2025).** Anomaly Detection in IoT based Smart Home Networks Using Hybrid Ensemble and CNN Models. *International Journal of Environmental Sciences, 11(23s), 3678-3687.*
   - **Relevance:** Demonstrates ensemble approaches for anomaly detection in IoT smart homes, supporting our multi-algorithm methodology.

4. **Meidan, Y., Avraham, D., Libhaber, H., & Shabtai, A. (2023).** CADeSH: Collaborative Anomaly Detection for Smart Homes. *arXiv preprint arXiv:2303.01021.*
   - **Relevance:** Presents collaborative anomaly detection framework applicable to multi-sensor elderly monitoring systems.

5. **Saha, B., Islam, M. S., Riad, A. K., Tahora, S., Shahriar, H., & Sneha, S. (2023).** BlockTheFall: Wearable Device-based Fall Detection Framework Powered by Machine Learning and Blockchain for Elderly Care. *arXiv preprint arXiv:2306.06452.*
   - **Relevance:** While focused on wearables, provides insights into ML-based fall detection algorithms transferable to non-wearable approaches.

6. **de Arriba-Pérez, F., García-Méndez, S., González-Castaño, F. J., & Costa-Montenegro, E. (2024).** Automatic detection of cognitive impairment in elderly people using an entertainment chatbot with Natural Language Processing capabilities. *arXiv preprint arXiv:2405.18542.*
   - **Relevance:** Demonstrates AI applications for elderly health monitoring, highlighting importance of non-intrusive approaches.

7. **Al-Rakhami, M. S., Gumaei, A., Altaf, M., Hassan, M. M., Alkhamees, B. F., Muhammad, K., & Fortino, G. (2021).** FallDeF5: A Fall Detection Framework Using 5G-based Deep Gated Recurrent Unit Networks. *arXiv preprint arXiv:2106.15049.*
   - **Relevance:** Validates GRU networks for fall detection, supporting our time-series analysis methodology.

### Luxembourg-Specific References

8. **STATEC (Institut national de la statistique et des études économiques du Grand-Duché de Luxembourg). (2024).** Population Statistics - Age Distribution. Luxembourg: STATEC.
   - **Relevance:** Provides demographic data on Luxembourg's aging population (19.5% over 65 years).

9. **Luxembourg National Commission for Data Protection (CNPD). (2024).** Artificial Intelligence and Data Protection: An Introduction. Retrieved from: https://cnpd.public.lu/en/dossiers-thematiques/intelligence-artificielle/intelligence-artificielle-introduction.html
   - **Relevance:** Official guidance on AI deployment and GDPR compliance in Luxembourg context.

10. **Luxembourg Digital Innovation Center (LUDCI). (2024).** Artificial Intelligence in Healthcare: Advancements and Challenges in Luxembourg. Retrieved from: https://ludci.eu/magazine/artificial-intelligence-in-healthcare-advancements-and-challenges-in-luxembourg/
    - **Relevance:** Contextualizes AI healthcare applications within Luxembourg's policy and regulatory environment.

### Technical Methodology References

11. **Hochreiter, S., & Schmidhuber, J. (1997).** Long Short-Term Memory. *Neural Computation, 9(8), 1735-1780.*
    - **Relevance:** Foundational paper on LSTM networks used for time-series pattern learning.

12. **Liu, F. T., Ting, K. M., & Zhou, Z.-H. (2008).** Isolation Forest. *2008 Eighth IEEE International Conference on Data Mining*, 413-422.
    - **Relevance:** Original Isolation Forest algorithm for anomaly detection, one of our core ML components.

13. **Schölkopf, B., Platt, J. C., Shawe-Taylor, J., Smola, A. J., & Williamson, R. C. (2001).** Estimating the Support of a High-Dimensional Distribution. *Neural Computation, 13(7), 1443-1471.*
    - **Relevance:** Foundational work on One-Class SVM, used in our anomaly detection ensemble.

14. **Vincent, P., Larochelle, H., Bengio, Y., & Manzagol, P.-A. (2008).** Extracting and Composing Robust Features with Denoising Autoencoders. *Proceedings of the 25th International Conference on Machine Learning*, 1096-1103.
    - **Relevance:** Autoencoder approach for anomaly detection via reconstruction error.

### GDPR and Privacy References

15. **European Union. (2016).** Regulation (EU) 2016/679 - General Data Protection Regulation (GDPR). *Official Journal of the European Union, L 119/1.*
    - **Relevance:** Primary legal framework for data protection compliance, specifically Articles 6, 9, and Chapter III (user rights).

16. **European Commission. (2021).** Proposal for a Regulation on Artificial Intelligence (AI Act). *COM/2021/206 final.*
    - **Relevance:** Emerging regulatory framework for AI systems, relevant for classification of our monitoring system.

17. **CNPD. (2024).** AI Prohibited Practices and High-Risk AI Systems. Retrieved from: https://cnpd.public.lu/en/dossiers-thematiques/intelligence-artificielle/regulation-ia/ia-prohibes.html
    - **Relevance:** Luxembourg-specific guidance on AI Act implementation and prohibited AI practices.

### IoT and Sensor Technology References

18. **An Innovative IoT and Edge Intelligence Framework for Monitoring Elderly People Using Anomaly Detection on Data from Non-Wearable Sensors. (2024).** *PubMed ID: 40292837.*
    - **Relevance:** Directly applicable framework for non-wearable sensor monitoring of elderly populations.

19. **Anomaly Detection in Elderly Health Monitoring via IoT for Timely Interventions. (2024).** *Applied Sciences, 15(13), 7272.*
    - **Relevance:** Validates IoT-based anomaly detection for elderly health monitoring and intervention timing.

### Additional Suggested Readings

20. **GDPR Advisor. (2024).** GDPR and IoT Devices: Addressing Privacy Concerns in the Connected World. Retrieved from: https://www.gdpr-advisor.com/gdpr-and-iot-devices-addressing-privacy-concerns-in-the-connected-world/
    - **Relevance:** Practical guidance on GDPR compliance for IoT devices in healthcare contexts.

---

## APPENDIX: VISUAL ELEMENTS FOR POSTER

### Recommended Figures/Diagrams:

1. **System Architecture Diagram:** Visual representation of three-tier architecture (Sensor → Edge → Cloud → Alerts) with labeled components

2. **Luxembourg Map:** Highlighting pilot deployment regions (Clervaux, Wiltz, Vianden, Echternach) with rural/urban population density overlay

3. **Timeline/Process Flow:** Visual flowchart showing: Data Collection → Baseline Learning → Real-Time Monitoring → Anomaly Detection → Alert Generation

4. **Use Case Scenarios:** 
   - Visual illustration 1: Fall detection (motion sensor patterns over time)
   - Visual illustration 2: Forgotten stove (electricity + temperature + motion correlation)
   - Visual illustration 3: Unusual inactivity (24-hour activity baseline vs. anomaly)

5. **Privacy by Design Diagram:** Showing data minimization, encryption layers, and access controls (concentric circles or layered architecture)

6. **Model Architecture Diagram:** LSTM network visualization showing input layers, hidden layers, output layers with feature dimensions

7. **Detection Performance Metrics:** Bar charts comparing detection accuracy, false positive rates across different use cases

8. **GDPR Compliance Framework:** Checklist or diagram showing Article 6 legal bases, data minimization, user rights

---

**Document Version:** 2.0  
**Last Updated:** [Current Date]  
**Next Steps:**
1. Create visual mockups for poster design
2. Develop detailed 1-page abstract for submission
3. Prepare presentation slides (separate document)
4. Refine based on group feedback
