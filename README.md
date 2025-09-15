# Privacy Policy for GettingStoned

_Last updated: January 2025_

## Overview

GettingStoned ("we," "our," or "us") is committed to protecting your privacy and ensuring transparency about how we collect, use, and safeguard your information when you use our Buddhist meditation and mindfulness mobile application. This comprehensive Privacy Policy explains our data practices across all features of the app.

## Information We Collect

### 1. Location Data

#### Karma Map and Spiritual Journey Tracking
- **GPS Coordinates**: We collect your device's location coordinates (latitude and longitude) when you use the karma map feature
- **Accuracy**: Location data is collected with 100-meter accuracy and updated every 30 seconds when the app is active
- **Purpose**: To visualize your meditation journey on a map, track where you practice meditation, and provide location-based spiritual insights
- **Storage**: Location coordinates are stored in Firebase with your user account for cross-device synchronization
- **Retention**: Location data is retained as long as your account is active

#### CarPlay Integration
- **Driving Behavior**: We monitor driving patterns and behavior when connected to CarPlay
- **Location Context**: Location data is used to provide context-aware driving insights and ethical driving guidance
- **Purpose**: To track calm vs. aggressive driving patterns and award merit stones for mindful driving
- **Processing**: Driving behavior analysis happens on-device; only aggregated insights are stored

### 2. Computer Vision and Machine Learning Data

#### Prostration Detection
- **Pose Data**: We use Core ML and Vision framework to analyze your body poses for prostration counting
- **Processing**: All pose analysis happens entirely on your device using the ProstrationClassifier ML model
- **Data Flow**: 
  - Input: 450 frames (15 seconds at 30 FPS) of pose data
  - Processing: Real-time pose estimation via Vision framework
  - Output: Action predictions (prostration vs. other movements)
- **Storage**: No raw pose data is stored; only prostration counts and session statistics
- **Privacy**: All computer vision processing occurs locally on your device

#### Mantra Counting (TrueDepth Camera)
- **Facial Landmark Data**: We collect real-time 3D facial mesh data and blend shape coefficients
- **Specific Data Points**:
  - Jaw opening measurements (jawOpen)
  - Mouth funnel detection (mouthFunnel)
  - Mouth puckering (mouthPucker)
  - Lip rounding scores (roundScore)
- **APIs Used**: ARFaceTrackingConfiguration, ARSCNView, ARFaceAnchor, ARSCNFaceGeometry
- **Processing**: All facial data is processed entirely on your device in real-time using ARKit
- **Retention**: Facial data is discarded immediately after processing each frame
- **Storage**: No facial data is stored or transmitted to any servers

#### NSFW Content Detection
- **Content Analysis**: We use machine learning models to detect inappropriate content
- **Processing**: Content filtering happens entirely on your device
- **Purpose**: To maintain a safe and respectful environment for spiritual practice
- **Data**: No content is stored; only filtering decisions are made locally

### 3. Health and Wellness Data

#### Apple Health Integration
- **Sleep Data**: We read sleep patterns and duration from Apple Health
- **Health Metrics**: We may read wellness metrics to provide holistic spiritual insights
- **Purpose**: To award merit stones for healthy sleep patterns and track overall wellness
- **Permissions**: Requires explicit user consent through Apple Health permissions
- **Storage**: Only aggregated sleep statistics are stored; raw health data remains in Apple Health

#### Muse EEG Integration
- **Brain Activity**: We collect real-time EEG data from your Muse headband via Bluetooth
- **Metrics Collected**:
  - Calmness levels
  - Focus scores
  - Meditation quality metrics
  - Brain wave patterns
- **Processing**: EEG data is processed locally on your device
- **Purpose**: To provide real-time meditation feedback and enhance mindfulness practice
- **Storage**: Only meditation session summaries and scores are stored; raw EEG data is not retained

### 4. Meditation and Spiritual Practice Data

#### Stone Entries
- **Stone Types**: White stones (merit) and black stones (non-virtue) you select
- **Categories**: Spiritual practice categories (patience, compassion, wisdom, etc.)
- **Reflection Notes**: Personal notes and reflections you choose to record
- **Timestamps**: Date and time of each meditation session
- **Location Context**: Optional location coordinates where you practiced
- **Purpose**: To track your spiritual progress and provide personalized insights

#### Session Data
- **Meditation Duration**: Length of meditation sessions
- **Practice Type**: Type of meditation (mantra, prostration, mindfulness, etc.)
- **Progress Tracking**: Cumulative counts and streaks
- **Achievements**: Merit stones earned and spiritual milestones reached

#### Advanced Spiritual Analytics
- **Bayesian Enlightenment Analysis**: Statistical modeling of your spiritual development using Beta-Binomial models
- **Karma Scoring**: Volume-adjusted karma calculations with comprehensive metrics
- **Predictive Analytics**: 30-day and 90-day spiritual development projections
- **Engagement Metrics**: Consistency scores, streak analysis, and practice patterns
- **Realm Balance**: Analysis of mind, speech, body, and special practice realms
- **Category Weighting**: Spiritual practice categories weighted by importance (merit: 2.5x, insight: 2.0x, meditation: 1.5x)

### 5. Technical and Analytics Data

#### App Usage Analytics
- **Performance Metrics**: App crashes, performance issues, and stability data
- **Feature Usage**: Which features you use most frequently
- **Session Duration**: How long you use the app
- **Purpose**: To improve app functionality and user experience
- **Collection**: Through Firebase Analytics (anonymized)

#### Device Information
- **Device Type**: iPhone, iPad model and iOS version
- **App Version**: Current version of the GettingStoned app
- **Technical Specifications**: Device capabilities for AR and ML features
- **Purpose**: To ensure compatibility and optimize performance

## Data Processing and Storage

### On-Device Processing (Private)
The following data is processed entirely on your device and never transmitted:

- ✅ **Facial Recognition Data**: All TrueDepth camera data for mantra counting
- ✅ **Pose Detection Data**: All body pose analysis for prostration counting
- ✅ **EEG Data**: Real-time brain activity processing from Muse headband
- ✅ **NSFW Content Detection**: All content filtering decisions
- ✅ **AR Stone Placement**: 3D rendering and placement of virtual stones
- ✅ **Personal Reflections**: Your meditation notes and thoughts

### Cloud Processing (Firebase/CloudKit)
The following data is synchronized across your devices:

- 🔄 **Location Coordinates**: GPS coordinates for karma mapping
- 🔄 **Stone Entries**: Your meditation progress and stone collections
- 🔄 **Session Statistics**: Aggregated meditation session data
- 🔄 **User Preferences**: App settings and customization
- 🔄 **Karma Statistics**: Spiritual progress metrics
- 🔄 **Cross-Device Sync**: Data synchronization between your devices
- 🔄 **Bayesian Analysis Results**: Enlightenment probability calculations and spiritual development projections
- 🔄 **Karma Scoring Data**: Volume-adjusted karma scores, engagement metrics, and consistency analysis
- 🔄 **Leaderboard Data**: Anonymous rankings and comparative spiritual progress metrics
- 🔄 **Predictive Analytics**: 30-day and 90-day spiritual development forecasts

### Third-Party Services

#### Firebase (Google)
- **Purpose**: Analytics, crash reporting, data synchronization, and advanced spiritual analytics
- **Data Shared**: 
  - Anonymized usage statistics and app performance data
  - Stone entries and spiritual practice data for karma analysis
  - Bayesian enlightenment probability calculations
  - Volume-adjusted karma scoring and leaderboard rankings
  - Predictive spiritual development analytics
- **Privacy**: 
  - Firebase Analytics data is anonymized and aggregated
  - Spiritual practice data is processed for personalized insights
  - Individual user data is isolated and private
- **Location**: Data stored in Google Cloud with standard security measures
- **Advanced Functions**:
  - `bayesianAnalysis.js`: Enlightenment probability calculations using Monte Carlo simulation
  - `karmicAnalysis.js`: Volume-adjusted karma scoring with comprehensive metrics
  - `getKarmicAnalysis.js`: User karma analysis and comparison
  - `leaderboardAggregation.js`: Anonymous leaderboard functionality
  - `generateStones.js`: Personalized stone recommendations

#### CloudKit (Apple)
- **Purpose**: Cross-device data synchronization
- **Data Shared**: Your meditation progress, stone entries, and preferences
- **Privacy**: Data is encrypted and stored in your personal iCloud account
- **Location**: Data stored in Apple's secure data centers

## Data We Do NOT Collect

We explicitly do not collect the following types of data:

- ❌ **Personal Photos or Videos**: Camera is used only for pose/facial detection
- ❌ **Audio Recordings**: Microphone is not accessed by the app
- ❌ **Personal Messages**: No communication or messaging features
- ❌ **Contact Information**: No access to your address book or contacts
- ❌ **Browsing History**: Browser features are sandboxed and isolated
- ❌ **Financial Information**: No payment or financial data collection
- ❌ **Raw Biometric Data**: Facial and pose data is processed locally and discarded
- ❌ **Personal Identifiable Information**: No names, addresses, or personal details

## Machine Learning and AI Features

### On-Device AI Processing
- **Prostration Detection**: Core ML model processes pose data locally
- **Mantra Counting**: Vision framework analyzes facial movements locally
- **Content Filtering**: NSFW detection happens on-device
- **EEG Analysis**: Brain activity processing occurs locally
- **AR Rendering**: 3D stone placement and visualization on-device

### Cloud-Based AI Processing
- **Bayesian Enlightenment Analysis**: Statistical modeling using Beta-Binomial models with Monte Carlo simulation
- **Karma Scoring**: Volume-adjusted karma calculations with logarithmic scaling
- **Predictive Analytics**: Future spiritual development projections using historical patterns
- **Engagement Analysis**: Consistency scoring and streak analysis
- **Category Weighting**: Spiritual practice importance weighting (merit: 2.5x, insight: 2.0x, meditation: 1.5x)

### AI Model Information
- **ProstrationClassifier**: Custom Core ML model for pose recognition
- **Vision Framework**: Apple's on-device computer vision APIs
- **ARKit**: Apple's augmented reality framework for facial tracking
- **Muse SDK**: Interaxon's brain-computer interface processing
- **Bayesian Models**: Custom statistical models for spiritual development analysis
- **Karma Algorithms**: Volume-adjusted scoring with comprehensive metrics

### Data Privacy in AI
- **No Training Data**: We do not use your personal data to train AI models
- **Local Processing**: All biometric and behavioral AI inference happens on your device
- **Cloud Analytics**: Spiritual practice patterns are analyzed for personalized insights
- **Anonymized Processing**: Individual spiritual data is processed privately
- **Model Updates**: AI models are updated through app updates, not data collection

## Advanced Spiritual Analytics

### Bayesian Enlightenment Analysis
- **Purpose**: To provide personalized spiritual development insights using statistical modeling
- **Data Processed**: Your stone entries, spiritual practice patterns, meditation streaks, and category preferences
- **Method**: Beta-Binomial statistical model with Monte Carlo simulation (10,000 samples)
- **Output**: Enlightenment probability calculations and spiritual development projections
- **Privacy**: Individual spiritual patterns are processed privately and not shared with other users
- **Storage**: Analysis results stored in Firebase for personalized insights and progress tracking

### Karma Scoring System
- **Purpose**: To provide fair and comprehensive karma assessment that balances quality and quantity
- **Data Processed**: Stone counts, categories, engagement levels, consistency metrics, and practice patterns
- **Formula**: Multi-factor scoring including positive actions (40%), negative avoidance (30%), engagement (20%), and consistency (10%)
- **Volume Adjustment**: Logarithmic scaling to prevent gaming while rewarding consistent practice
- **Category Weighting**: 
  - Merit practice stones: 2.5x weight (highest)
  - Insight/emptiness analysis stones: 2.0x weight
  - Meditation stones: 1.5x weight
  - Regular white stones: 1.0x weight
  - Analyzed black stones: 0.5x weight (reduced negative impact)
- **Storage**: Karma scores and rankings stored for leaderboard and progress tracking

### Predictive Spiritual Development
- **Purpose**: To project future spiritual development and provide motivation for continued practice
- **Data Processed**: Historical practice patterns, current streak data, and daily meditation averages
- **Projections**: 30-day and 90-day enlightenment probability forecasts
- **Method**: Based on current daily averages and projected consistent practice patterns
- **Privacy**: Projections are personal and not shared with other users
- **Storage**: Future projections stored for personalized goal setting and motivation

### Leaderboard and Comparison Analytics
- **Purpose**: To provide anonymous comparison with other practitioners for motivation
- **Data Processed**: Aggregated karma scores, engagement metrics, and practice consistency
- **Privacy**: Individual identities are not revealed; only anonymous rankings and metrics
- **Storage**: Anonymous leaderboard data stored for community motivation features

## User Controls and Permissions

### Location Permissions
- **When In Use**: Required for karma map and location-based insights
- **Control**: Can be revoked at any time in iOS Settings
- **Impact**: Revoking location access disables karma mapping features

### Camera Permissions
- **TrueDepth Camera**: Required for mantra counting feature
- **Control**: Can be disabled in iOS Settings
- **Impact**: Disabling camera access switches to manual mantra counting

### Health Permissions
- **Apple Health**: Required for sleep tracking and wellness insights
- **Control**: Managed through Apple Health app permissions
- **Impact**: Revoking health access disables sleep-based merit stones

### Bluetooth Permissions
- **Muse Headband**: Required for EEG meditation features
- **Control**: Can be disabled in iOS Settings
- **Impact**: Disabling Bluetooth disables Muse integration

### Notification Permissions
- **Push Notifications**: For meditation reminders and insights
- **Control**: Can be disabled in iOS Settings
- **Impact**: Disabling notifications stops meditation reminders

## Data Security Measures

### Encryption
- **In Transit**: All data transmission uses TLS 1.3 encryption
- **At Rest**: All stored data is encrypted using AES-256
- **Local Storage**: Device data is protected by iOS security features

### Access Controls
- **User Authentication**: Firebase Authentication for account security
- **Data Isolation**: Each user's data is isolated and private
- **Admin Access**: Limited administrative access with audit logging

### Security Monitoring
- **Intrusion Detection**: Continuous monitoring for security threats
- **Vulnerability Scanning**: Regular security assessments
- **Incident Response**: Established procedures for security incidents

## Data Retention and Deletion

### Retention Periods
- **Meditation Data**: Retained as long as your account is active
- **Location Data**: Retained for karma mapping functionality
- **Analytics Data**: Anonymized data retained for 2 years
- **Biometric Data**: Not retained (processed locally and discarded)

### Data Deletion
- **Account Deletion**: Complete removal of all personal data within 30 days
- **Partial Deletion**: Individual data points can be deleted upon request
- **Backup Cleanup**: Data removed from all backup systems
- **Third-Party Cleanup**: Data deletion requests sent to all service providers

## International Data Transfers

### Data Location
- **Primary Storage**: United States (Firebase/Google Cloud)
- **Backup Storage**: Multiple geographic regions for redundancy
- **Processing**: Data processing occurs in the same regions as storage

### Transfer Safeguards
- **Standard Contractual Clauses**: EU data transfers use approved SCCs
- **Adequacy Decisions**: Transfers to countries with adequate protection
- **Technical Safeguards**: Encryption and access controls for all transfers

## Children's Privacy

### Age Restrictions
- **Minimum Age**: App is not intended for children under 13
- **Parental Consent**: Users under 18 should have parental supervision
- **Data Collection**: We do not knowingly collect data from children under 13

### Special Protections
- **Limited Data**: Reduced data collection for younger users
- **Parental Controls**: Enhanced privacy controls for family accounts
- **Education**: Resources for parents about digital wellness

## Your Rights and Choices

### Access Rights
- **Data Access**: Request a copy of all your personal data
- **Data Portability**: Export your meditation data in standard formats
- **Account Information**: View and update your account details

### Control Rights
- **Data Correction**: Correct inaccurate or incomplete data
- **Data Deletion**: Request deletion of your personal data
- **Processing Restriction**: Limit how your data is processed
- **Objection**: Object to certain types of data processing

### Communication Rights
- **Marketing Opt-out**: Unsubscribe from promotional communications
- **Notification Control**: Manage meditation reminders and alerts
- **Privacy Updates**: Receive notifications about privacy policy changes

## Compliance and Regulations

### GDPR Compliance (European Union)
- **Lawful Basis**: Processing based on consent and legitimate interests
- **Data Subject Rights**: Full compliance with GDPR data subject rights
- **Data Protection Officer**: Designated DPO for EU users
- **Breach Notification**: 72-hour notification requirement compliance

### CCPA Compliance (California)
- **Consumer Rights**: Full compliance with California Consumer Privacy Act
- **Opt-out Rights**: Right to opt-out of data sales (we don't sell data)
- **Disclosure Rights**: Right to know what data is collected and used
- **Deletion Rights**: Right to delete personal information

### COPPA Compliance (Children)
- **Parental Consent**: Required for children under 13
- **Limited Collection**: Minimal data collection for children
- **Parental Rights**: Parents can review and delete children's data

## Changes to This Privacy Policy

### Notification of Changes
- **Material Changes**: 30-day advance notice for significant changes
- **Minor Updates**: Immediate posting for minor clarifications
- **Version History**: Maintained record of all policy changes
- **User Consent**: Re-consent required for material changes

### Effective Date
- **Current Version**: January 2025
- **Previous Versions**: Available upon request
- **Implementation**: Changes effective immediately upon posting

## Contact Information

### Privacy Inquiries
**Email**: privacy@gettingstoned.app  
**Subject**: Privacy Policy Inquiry  
**Response Time**: Within 72 hours

### Data Protection Officer (EU Users)
**Email**: dpo@gettingstoned.app  
**Subject**: GDPR Data Protection Inquiry

### General Support
**Email**: support@gettingstoned.app  
**Website**: https://github.com/your-username/buddhist-stone-app

### Postal Address
BunkCorp  
[Your Business Address]  
[City, State, ZIP Code]  
United States

## Additional Resources

### Privacy Resources
- **Apple Privacy**: https://www.apple.com/privacy/
- **Google Privacy**: https://policies.google.com/privacy
- **Firebase Privacy**: https://firebase.google.com/support/privacy

### Educational Materials
- **Digital Wellness**: Resources for mindful technology use
- **Privacy Best Practices**: Tips for protecting your digital privacy
- **Buddhist Ethics**: How our app aligns with Buddhist principles

---

_GettingStoned - Integrating ancient wisdom with modern technology for mindful living_

**Last Updated**: January 2025  
**Version**: 2.0  
**Effective Date**: January 1, 2025
