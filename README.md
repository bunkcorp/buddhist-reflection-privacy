# Privacy Policy for Buddhist Reflection

_Last updated: December 4, 2025_

## Overview

Buddhist Reflection ("we," "our," or "us") is committed to protecting your privacy. This Privacy Policy explains how we collect, use, and safeguard your information when you use our mobile application.

---

## ⚠️ IMPORTANT: TrueDepth API Usage

**This app uses Apple's TrueDepth API (ARKit Face Tracking). All facial data processing occurs entirely on your device and is never stored or transmitted.**

### Purpose and Functionality

Our app uses Apple's TrueDepth API exclusively for the following features:
- **Mantra Counting**: Detecting mouth movements to count mantra recitations during meditation
- **Prostration Detection**: Analyzing body poses for meditation practice tracking

### Data Collected via TrueDepth API

When you use features that require TrueDepth:
- **Facial Landmark Data**: 3D facial mesh coordinates (real-time, frame-by-frame)
- **Blend Shape Coefficients**: 
  - Jaw opening measurements (`jawOpen`)
  - Mouth funnel detection (`mouthFunnel`)
  - Mouth puckering measurements (`mouthPucker`)
  - Lip rounding scores (`roundScore`)
- **Face Geometry**: Facial feature positions and orientations
- **Depth Data**: Spatial depth information for pose estimation

### Data Processing (On-Device Only)

- **All processing occurs entirely on your device** using ARKit
- **Real-time processing**: Data is analyzed frame-by-frame (typically 30 FPS)
- **No storage**: Facial data is discarded immediately after each frame is processed
- **No transmission**: Facial data is never sent to our servers or any third parties
- **Local only**: Data remains on your device at all times
- **No cloud storage**: We do not upload, store, or sync any facial data

### Apple APIs Used

- `ARFaceTrackingConfiguration` - Configures TrueDepth camera access
- `ARSCNView` - Displays AR face tracking visualization
- `ARFaceAnchor` - Provides facial landmark and blend shape data
- `ARSCNFaceGeometry` - Processes 3D facial geometry
- `AVCaptureDevice` (TrueDepth camera) - Camera access for face tracking

### Data Retention

- **Zero retention**: Facial data is discarded immediately after processing each frame
- **No persistent storage**: We do not save any facial data to your device storage or our servers
- **Session-based only**: Data exists only in active memory during active meditation sessions
- **No historical data**: We do not maintain any history of facial measurements

### User Control

You have complete control over TrueDepth API usage:
- **Camera Permission**: Grant or revoke camera access in iOS Settings → GettingStoned → Camera
- **Feature Disable**: You can disable mantra counting features that use TrueDepth
- **Alternative Methods**: App provides manual counting alternatives that don't require camera access
- **No Requirement**: TrueDepth usage is optional; the app functions fully without it
- **Account Deletion**: You can delete your account at any time through Settings → Profile Settings → Delete Account

### Purpose Limitation

TrueDepth API is used **exclusively** for:
1. Counting mantra recitations during meditation practice
2. Tracking prostration movements during meditation practice

We **do NOT** use TrueDepth API for:
- ❌ Face recognition or identification
- ❌ Emotion detection or analysis beyond meditation practice
- ❌ Advertising or marketing purposes
- ❌ Biometric authentication
- ❌ User profiling or tracking
- ❌ Any purpose other than meditation practice features

### Compliance

- ✅ Complies with Apple's App Store Review Guidelines 5.1.1 (Privacy - Data Collection and Storage)
- ✅ Complies with privacy requirements for TrueDepth API usage
- ✅ All processing is on-device as required by Apple's guidelines
- ✅ No data sharing with third parties
- ✅ User consent required via iOS camera permission prompt

---

## ⚠️ IMPORTANT: Sensitive Content Analysis

**This app uses Apple's Sensitive Content Analysis framework. All image analysis occurs entirely on your device and is never stored or transmitted.**

### Purpose and Functionality

Our app uses Apple's Sensitive Content Analysis framework exclusively for the following features:
- **Enhanced Browser**: Detecting NSFW (Not Safe For Work) content in images on web pages you browse
- **Karmic Tracking**: Automatically logging "black stones" when inappropriate content is detected (if auto-logging is enabled)

### Data Collected via Sensitive Content Analysis

When you use the Enhanced Browser feature (available with Premium subscription):
- **Images are extracted** from web pages you visit (up to 5 images per page)
- **Images are analyzed** using Apple's `SCSensitivityAnalyzer` API
- **Analysis results** indicate whether sensitive/inappropriate content was detected

### Data Processing (On-Device Only)

- **All analysis occurs entirely on your device** using Apple's Core ML models
- **Real-time processing**: Images are analyzed as you browse, then discarded immediately
- **No storage**: Image data is discarded immediately after analysis
- **No transmission**: Image data is never sent to our servers or any third parties
- **Local only**: All sensitive content analysis happens locally on your device
- **No cloud storage**: We do not upload, store, or sync any images or analysis results

### Apple APIs Used

- `SensitiveContentAnalysis` framework
- `SCSensitivityAnalyzer` - Analyzes images for sensitive content
- `CGImage` - Processes images for analysis

### Data Retention

- **Zero retention**: Image data is discarded immediately after analysis
- **No persistent storage**: We do not save any images or analysis results to your device storage or our servers
- **Session-based only**: Analysis occurs only during active browsing sessions
- **Karmic tracking**: Only the fact that NSFW content was detected (resulting in a "black stone") is logged to your karmic tracking data, not the images themselves
- **No historical data**: We do not maintain any history of analyzed images

### Automatic Stone Logging

When NSFW content is detected:
- **A "black stone" is automatically logged** to your karmic tracking system (if auto-logging is enabled in browser settings)
- **Black stones** represent negative karma in our Buddhist meditation tracking system
- **You can control this feature** by enabling or disabling "auto-log stones" in the browser settings
- **Only the detection result is logged**, not the actual images or content

### User Control

You have complete control over Sensitive Content Analysis:
- **Feature Access**: Sensitive Content Analysis is only active in the Enhanced Browser feature (Premium subscription required)
- **Auto-Logging Control**: Enable or disable automatic stone logging in browser settings
- **Browsing Control**: You can navigate away from pages with detected sensitive content at any time
- **No Requirement**: Sensitive Content Analysis is optional; you can browse without it by using other browsers
- **Account Deletion**: You can delete your account at any time through Settings → Profile Settings → Delete Account

### Purpose Limitation

Sensitive Content Analysis is used **exclusively** for:
1. Detecting inappropriate content in images on web pages
2. Providing a safer browsing environment for meditation and mindfulness practice
3. Supporting our karmic tracking system by identifying negative content

We **do NOT** use Sensitive Content Analysis for:
- ❌ Storing or transmitting images
- ❌ User profiling or tracking
- ❌ Advertising or marketing purposes
- ❌ Any purpose other than content safety and karmic tracking

### Compliance

- ✅ Complies with Apple's App Store Review Guidelines
- ✅ Complies with Apple's Sensitive Content Analysis framework requirements
- ✅ Uses proper entitlements: `com.apple.developer.sensitivecontentanalysis.client`
- ✅ All processing is on-device as required by Apple's guidelines
- ✅ No data sharing with third parties
- ✅ User control via browser settings

---

## Information We Collect

### Personal Reflections

* Meditation reflections and thoughts you choose to record
* Stone selections (white/black) and categories you assign
* Timestamps of your meditation sessions
* Location data (optional) - Only if you choose to enable location-based features for the karma map

### Facial Data Collection (TrueDepth API)

**IMPORTANT**: This section describes our use of Apple's TrueDepth API. All data collection and processing described below occurs entirely on your device and is never stored or transmitted.

* **TrueDepth Camera Data**: Our app uses the TrueDepth camera (on supported devices like iPhone X and later) to detect mouth movements for the Mantra Counter feature and body poses for prostration detection
* **Facial Landmark Data**: We collect real-time 3D facial mesh data and blend shape coefficients specifically for mouth movement detection and pose estimation
* **Purpose**: This data is used exclusively for counting Buddhist mantra repetitions by detecting jaw opening, lip rounding, and mouth puckering movements, and for tracking prostration movements during meditation practice
* **Processing**: All facial data is processed entirely on your device in real-time using ARKit and is not stored or transmitted to any servers
* **Retention**: Facial data is discarded immediately after processing and is not retained
* **Transmission**: Facial data is never transmitted to any external server, service, or third party

### Image Analysis Data (Sensitive Content Analysis)

**IMPORTANT**: This section describes our use of Apple's Sensitive Content Analysis framework. All image analysis occurs entirely on your device and is never stored or transmitted.

* **Image Analysis Data**: Our app uses Apple's Sensitive Content Analysis framework to analyze images from web pages you visit in the Enhanced Browser feature
* **Purpose**: This analysis is used exclusively for detecting NSFW (Not Safe For Work) content in images to provide a safer browsing environment and support our karmic tracking system
* **Processing**: All image analysis is processed entirely on your device in real-time using Apple's Core ML models and is not stored or transmitted to any servers
* **Retention**: Image data is discarded immediately after analysis and is not retained
* **Transmission**: Image data is never transmitted to any external server, service, or third party
* **Karmic Tracking**: Only the detection result (whether NSFW content was found) is logged as a "black stone" in your karmic tracking data, not the images themselves

### Technical Information

* Device push notification tokens (for sending meditation reminders) - stored securely in Firebase
* Basic app usage analytics - anonymized and aggregated
* Crash reports to improve app stability - anonymized error logs

### Account Information

* Email address (for account creation and authentication)
* Display name (optional)
* Member since date
* Authentication tokens (stored securely via Firebase Authentication)

---

## How We Use Your Information

* To provide personalized meditation reminders
* To track your mindfulness progress through stone analytics
* To enable hands-free mantra counting through facial movement detection (on-device processing only)
* To provide safer web browsing through automatic NSFW content detection (on-device processing only)
* To improve app functionality and user experience
* To send you gentle Buddhist reflection prompts
* To sync your meditation data across devices (stones, reflections, session history)
* To provide location-based insights on the karma map (if location services are enabled)

---

## Data Storage and Security

* Your data is stored securely using Firebase/Google Cloud services
* All reflections and personal data are encrypted in transit and at rest
* **Facial data is processed entirely on-device and is never stored or transmitted**
* **Image analysis data is processed entirely on-device and is never stored or transmitted**
* We implement industry-standard security measures to protect your information
* Your meditation data is private and not shared with third parties
* Account credentials are secured using Firebase Authentication with industry-standard encryption

---

## Data Sharing

We do not sell, trade, or share your personal meditation data with third parties. Your reflections, stone selections, facial data, and image analysis data remain private to you. Facial data collected through the TrueDepth API and image data analyzed through Sensitive Content Analysis are processed locally on your device and are never shared with any external parties.

**Third-Party Services Used:**
* **Firebase (Google)**: Used for data storage, authentication, and push notifications. Firebase's privacy policy applies to data stored in their service.
* **Google Analytics**: Used for anonymized app usage analytics. No personally identifiable information is shared.

---

## User Controls and Permissions

### Camera Permissions

* **TrueDepth Camera**: Required for mantra counting and prostration detection features
  * Uses ARKit Face Tracking (TrueDepth API)
  * All processing occurs on-device
  * No facial data is stored or transmitted
  * See "TrueDepth API Usage" section above for complete details
* **Rear Camera**: Alternative for prostration detection if TrueDepth unavailable (same on-device processing)
* **Control**: Can be disabled in iOS Settings → GettingStoned → Camera
* **Impact**: 
  * Disabling TrueDepth camera: Switches to manual mantra counting
  * Disabling camera access: Disables all camera-based features (manual counting still available)

### Location Permissions

* **Location Services**: Optional, used only for karma map features
* **Control**: Can be disabled in iOS Settings → GettingStoned → Location
* **Impact**: Karma map will not show location-based features, but all other app features work normally

### Account Management

* **Account Deletion**: Available in Settings → Profile Settings → Delete Account
* **Data Export**: Contact us at privacy@buddhistreflection.app to request your data export
* **Consent Withdrawal**: Revoke camera or location permissions in iOS Settings at any time

---

## Push Notifications

We use Firebase Cloud Messaging to send you meditation reminders. You can disable these notifications at any time through your device settings or within the app settings.

---

## Data Retention

* Your meditation data (stones, reflections, sessions) is retained as long as you use the app
* **Facial data is not retained** - it is processed in real-time and discarded immediately
* **Image analysis data is not retained** - images are analyzed in real-time and discarded immediately after analysis
* **Account data**: Retained until account deletion
* You may request deletion of your data by:
  - Using the in-app account deletion feature: Settings → Profile Settings → Delete Account
  - Contacting us at privacy@buddhistreflection.app
* Upon account deletion, all personal data is permanently removed within 30 days

---

## Your Rights

You have the right to:

* **Access your personal data** - View all your meditation data within the app
* **Correct inaccurate data** - Edit your profile information and reflection notes
* **Request deletion of your data** - Delete your account through Settings → Profile Settings → Delete Account
* **Disable push notifications** - Manage notification preferences in iOS Settings or app settings
* **Disable facial recognition features** - Revoke camera permission in iOS Settings (app will fall back to manual counting)
* **Disable automatic stone logging** - Turn off "auto-log stones" in browser settings to prevent automatic logging of detected NSFW content
* **Withdraw consent** - Revoke any permission at any time through iOS Settings
* **Export your data** - Contact us at privacy@buddhistreflection.app to request a data export

---

## Account Deletion

If you created an account, you can delete it at any time:

1. Open the app and go to **Settings → Profile Settings**
2. Scroll to the **"Account Management"** section
3. Tap **"Delete Account"**
4. Confirm the deletion

Upon account deletion:
- All your meditation data (stones, reflections, sessions) will be permanently deleted
- Your Firebase Authentication account will be removed
- All Firestore data associated with your account will be deleted
- Local app data will be cleared
- **Facial data**: As noted above, facial data was never stored, so there is nothing to delete
- **Image analysis data**: As noted above, image analysis data was never stored, so there is nothing to delete

Account deletion is permanent and cannot be undone.

---

## Children's Privacy

Our app is not intended for children under 13. We do not knowingly collect personal information from children under 13. If you are a parent or guardian and believe your child has provided us with personal information, please contact us at privacy@buddhistreflection.app and we will delete such information.

---

## Changes to This Policy

We may update this Privacy Policy from time to time. We will notify you of any material changes by:
- Posting the new Privacy Policy on this page
- Updating the "Last updated" date at the top of this policy
- Sending you a notification through the app (if significant changes are made)

---

## Contact Us

If you have any questions about this Privacy Policy, your data, or your privacy rights, please contact us at:

**Email:** privacy@buddhistreflection.app  
**Subject:** Privacy Policy Inquiry

We will respond to your inquiry within 30 days.

---

_Buddhist Reflection App - Bringing mindfulness to daily life_
