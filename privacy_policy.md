# Privacy Policy

**Last Updated: January 30, 2026**

This Privacy Policy explains how **Spent** ("we", "us", or "our") collects, uses, and discloses your information when you use our mobile application (the "Service").

By actively using the Service, you agree to the collection and use of information in accordance with this policy.

## 1. Information We Collect

### A. Financial Transaction Data
To provide our core service—automated expense tracking—we require access to your device's notifications.
-   **Source:** We use the `BIND_NOTIFICATION_LISTENER_SERVICE` permission to read notifications from specific financial applications (e.g., banks, SMS wallets).
-   **Data Extracted:** We extract specific financial details such as **Merchant Name**, **Amount**, **Date**, and **Currency**.
-   **Processing:**
    1.  **On-Device:** Initial filtering uses Google's ML Kit (on-device) to identify if a notification is finance-related.
    2.  **Cloud AI:** Verified financial text is securely transmitted to our private server and processed using **AWS Bedrock** (Artificial Intelligence) to categorize the transaction (e.g., "Food", "Transport").

### B. Personal Data (Account)
-   **Authentication:** We use **Google Firebase Authentication**. We may collect your email address and User ID to secure your account and sync your data across devices.

### C. Usage Data
-   **Firebase Analytics** and **Crashlytics** to collect anonymous usage statistics and crash reports to improve app stability.

## 2. How We Use Your Information

-   **To Provide the Service:** To automatically record, categorize, and display your spending history.
-   **To Improve AI Accuracy:** We use the transaction text to query our AI models (AWS Bedrock) for better categorization. **We do not use your data to train public AI models.**

## 3. Data Storage & Security

-   **Cloud Storage:** Your transaction history is stored securely in **Google Cloud Firestore**.
-   **Encryption:** All data transmission between the App, our Servers (n8n), and Third-Party Services (Firebase, AWS) is encrypted using TLS/SSL protocols.

## 4. Third-Party Services

We leverage the following trusted third-party services:
-   **Google Firebase:** For authentication, database storage, and analytics. [Google Privacy Policy](https://policies.google.com/privacy)
-   **AWS Bedrock (Amazon Web Services):** For AI-powered transaction categorization. Data sent to Bedrock is not used to improve Amazon's base models. [AWS Data Privacy](https://aws.amazon.com/compliance/data-privacy/)
-   **Google Play Services:** For handling subscriptions and payments.

## 5. Subscription & Payments

We use **Google Play Billing** for all transactions. We do not store or process your credit card information directly. All financial transactions are handled by Google.

## 6. Data Deletion

You have the right to delete your account and all associated data at any time.
-   **In-App:** Go to **Settings > Profile > Delete Account**. This will permanently remove your data from our servers immediately.

## 7. Changes to This Policy

We may update our Privacy Policy from time to time. We will notify you of any changes by posting the new Privacy Policy on this page and updating the "Last updated" date.

## 8. Contact Us

If you have any questions about these Terms, please contact us at:
-   **Email:** contact@invoicegentle.com
