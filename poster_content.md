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

The system employs non-intrusive environmental sensors—temperature, gas detection, motion sensors, and electricity consumption monitors—to analyze behavioral patterns without compromising privacy. The system learns each person's normal daily routines over 4-6 weeks using AI models (LSTM networks) to establish personalized baselines. Anomaly detection algorithms then continuously monitor for deviations from these baselines, identifying potential emergencies such as falls, forgotten appliances, or unusual inactivity periods.

The proposed methodology employs a simple three-layer architecture: (1) sensors in the home that collect environmental data, (2) cloud-based AI processing that analyzes patterns and detects anomalies, and (3) alert systems that notify family members and caregivers via email, SMS, or phone calls. This solution addresses the growing need for non-intrusive, privacy-preserving care assistance in the Greater Region, while maintaining elderly autonomy and dignity through GDPR-compliant data handling.

**Keywords:** Elderly Care, IoT, Anomaly Detection, Predictive Analytics, Home Safety, Luxembourg, GDPR-Compliant Monitoring

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

The system employs a simple three-layer architecture:

```
┌─────────────────────────────────────────────────────────────────┐
│                    LAYER 1: SENSORS (Home)                      │
│  • Temperature sensors (kitchen, bedroom)                        │
│  • Motion sensors (living room, hallway)                       │
│  • Gas detection sensors (kitchen)                              │
│  • Electricity monitors (smart plugs on appliances)             │
│  • Edge device (Raspberry Pi) collects sensor data            │
└─────────────────────────────────────────────────────────────────┘
                              ↓
┌─────────────────────────────────────────────────────────────────┐
│              LAYER 2: AI PROCESSING (Cloud)                      │
│  • Data sent securely to Luxembourg-based cloud                 │
│  • AI models analyze patterns and detect anomalies              │
│  • Risk scoring: calculates probability of emergency            │
└─────────────────────────────────────────────────────────────────┘
                              ↓
┌─────────────────────────────────────────────────────────────────┐
│                 LAYER 3: ALERTS (Notifications)                 │
│  • Multi-level alerts: Email, SMS, or Phone Call               │
│  • Dashboard for families/caregivers to monitor status         │
│  • Real-time notifications when anomalies detected             │
└─────────────────────────────────────────────────────────────────┘
```

### 5.2 AI/ML Components

#### 5.2.1 Pattern Learning

**How It Works:**
- The system learns each person's normal daily patterns over 4-6 weeks
- Uses **LSTM (Long Short-Term Memory)** networks to understand:
  - When they typically wake up and go to sleep
  - Normal movement patterns throughout the day
  - Typical electricity usage (cooking times, TV watching, etc.)
  - Normal temperature variations in the home

**Purpose:** Establish a personalized baseline of "normal" behavior for each elderly person.

#### 5.2.2 Anomaly Detection

**How It Works:**
- The system continuously compares current sensor readings to the learned baseline
- Uses **anomaly detection algorithms** to identify when something is unusual:
  - **Isolation Forest:** Detects outliers in the data
  - **One-Class SVM:** Learns what's normal and flags deviations
  - **Autoencoders:** Learns compressed patterns and detects when patterns don't match

**Ensemble Approach:**
- Combines all three methods for more reliable detection
- If multiple methods agree something is unusual, an alert is generated
- Reduces false alarms while maintaining high detection accuracy

#### 5.2.3 Risk Scoring

**How It Works:**
- Combines information from all sensors to calculate a risk score (0-1 scale)
- Factors considered:
  - Motion patterns (unusual inactivity?)
  - Temperature (too hot/cold?)
  - Electricity usage (forgotten appliance?)
  - Time of day (unusual activity at odd hours?)

**Alert Levels:**
- **Low (0.6-0.7):** Email notification
- **Medium (0.7-0.8):** SMS notification
- **High (>0.8):** SMS + Phone call

### 5.3 Detection Logic for Specific Use Cases

#### Use Case 1: Fall Detection

**How It Works:**
- Motion sensors monitor activity in common areas (living room, hallway, kitchen)
- System learns normal movement patterns (when person is typically active)
- **Alert Trigger:** If no movement detected for >30 minutes during normal active hours
- **Confirmation:** Cross-checks with electricity usage (no appliance activity)
- **Result:** High-priority alert sent to family/caregivers

**Expected Performance:** >90% detection accuracy

#### Use Case 2: Forgotten Stove/Appliance Detection

**How It Works:**
- Electricity monitor tracks kitchen appliance usage
- Temperature sensor monitors kitchen temperature
- Motion sensor checks if person is in kitchen
- **Alert Trigger:** High electricity usage + elevated temperature + no movement in kitchen for >30 minutes
- **Gas Detection:** If gas sensor detects gas, immediate high-priority alert
- **Result:** Medium-priority alert (escalates to high if gas detected)

**Expected Performance:** >95% detection accuracy

#### Use Case 3: Unusual Inactivity Detection

**How It Works:**
- System learns daily activity baseline (normal movement patterns throughout the day)
- Continuously compares current activity to learned baseline
- **Alert Trigger:** Activity significantly lower than normal for extended period (>6 hours)
- **Context:** Excludes normal sleep hours
- **Result:** Low-priority alert initially, escalates if inactivity continues

**Expected Performance:** >85% detection accuracy

### 5.4 Data Processing Pipeline

**Step 1: Data Collection**
- Sensors continuously collect data (temperature, motion, electricity, gas)
- Edge device (Raspberry Pi) collects and temporarily stores sensor readings
- Data sent securely to cloud every few minutes

**Step 2: Pattern Analysis**
- AI models analyze the data to understand normal patterns
- System learns daily routines over 4-6 weeks
- Creates personalized baseline for each person

**Step 3: Anomaly Detection**
- System continuously compares current readings to learned baseline
- When patterns deviate significantly, anomaly is detected
- Risk score calculated based on severity of deviation

**Step 4: Alert Generation**
- If risk score exceeds threshold, alert is generated
- Alert level determines notification method (email, SMS, or phone call)
- Family/caregivers receive notification within 2 minutes

### 5.5 Implementation Details

**Hardware:**
- **Sensors:** Temperature sensors, motion sensors, gas detectors, smart plugs
- **Edge Device:** Raspberry Pi (small computer that processes data locally)
- **Cost:** Approximately €150-200 per household (one-time setup)

**Software:**
- **AI Models:** Python-based machine learning models (LSTM, anomaly detection)
- **Cloud:** Luxembourg-based cloud storage for data and processing
- **Dashboard:** Web and mobile app for families to monitor status
- **Monthly Cost:** Approximately €20-35 per household (cloud services, SMS alerts)

**Security:**
- All data encrypted during transmission and storage
- No personal information collected (only sensor readings)
- Secure access controls for family/caregivers

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

1. **Shahid, Z. K., Saguna, S., & Åhlund, C. (2024).** Detecting Anomalies in Daily Activity Routines of Older Persons in Single Resident Smart Homes: Proof-of-Concept Study. *JMIR Aging, 7, e58394.*
   - **Relevance:** Validates anomaly detection in smart home environments for elderly, demonstrating feasibility of non-wearable sensor approaches. Directly applicable to our project's methodology.

2. **An Innovative IoT and Edge Intelligence Framework for Monitoring Elderly People Using Anomaly Detection on Data from Non-Wearable Sensors. (2024).** *PubMed ID: 40292837.*
   - **Relevance:** Directly applicable framework for non-wearable sensor monitoring of elderly populations using anomaly detection, matching our system architecture and approach.

3. **Reddy, M. V. K., Lathigara, A., & Reddy, N. H. (2025).** Anomaly Detection in IoT based Smart Home Networks Using Hybrid Ensemble and CNN Models. *International Journal of Environmental Sciences, 11(23s), 3678-3687.*
   - **Relevance:** Demonstrates ensemble approaches for anomaly detection in IoT smart homes, supporting our multi-algorithm methodology for combining different anomaly detection techniques.

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
