# Privacy Policy - eSAMz AI

**Last Updated: June 9, 2026**

This Privacy Policy describes how eSAMz AI ("we," "us," or "our") collects, uses, processes, and protects your personal data when you use our AI assistant services (the "Service"). We are committed to safeguarding your privacy and ensuring compliance with applicable data protection laws, including the Digital Personal Data Protection Act (DPDP), 2023, of India, and principles aligned with the General Data Protection Regulation (GDPR).

## 1. Your Consent

By accessing or using the eSAMz AI Service, you acknowledge that you have read, understood, and agree to the terms of this Privacy Policy. For the processing of your personal data, we obtain your explicit, informed consent through clear affirmative action. Before processing any personal data, you will be presented with a standalone notice detailing:

*   The categories of personal data being processed.
*   The specific purposes for which your personal data is processed.
*   Your rights as a Data Principal under the DPDP Act and other applicable laws.
*   The mechanism for exercising these rights and for grievance redressal.
*   Contact information for our Data Protection Officer or designated contact person.

Your consent will be specific to each purpose and will not be implied by your continued use of the Service. You have the right to withdraw your consent at any time, as detailed in Section 8.

## 2. Data We Collect and Process

We minimize data collection to what is strictly necessary to provide and improve our Service. The types of personal data we collect and process depend on how you interact with eSAMz AI.

### 2.1. Data Collected from All Users (Anonymous and Signed-in)

*   **Session Prompts:** Your input prompts during a chat session are processed in real-time to generate responses. These are subject to a strict 30-minute retention policy on our servers, after which they are automatically wiped. We do not store these prompts beyond this period for anonymous users. If `PRIVACY_MODE` is enabled on our servers, no session history is stored at all.
*   **Minimal System Logs:** We maintain minimal technical logs strictly for security, debugging, and abuse prevention. These logs may include request timestamps, response codes, and anonymized usage data. Access logs are retained for short periods (typically 48 hours) and then deleted.
*   **Local Browser Storage:** Your chat history and certain user preferences are stored locally on your device using `localStorage`. This data is not transmitted to or accessed by our servers. You can clear this data by clearing your browser's local storage or cookies.
*   **User Agent Information:** We collect information about your browser and operating system for compatibility, security, and analytics purposes.
*   **IP Address:** Your IP address is collected for security, abuse prevention, and for legal compliance, particularly when recording your consent to our Privacy Policy and Terms of Service.

### 2.2. Data Collected from Signed-in Users

When you create or sign in to an account using Clerk authentication, we collect and process additional data:

*   **Email Address:** Used for authentication, account management, security purposes, and to identify your subscription tier.
*   **Clerk User ID (`clerkId`):** A unique identifier provided by our authentication provider (Clerk) to manage your account.
*   **Privacy Policy Acceptance Records:** When you explicitly accept our Privacy Policy, we record:
    *   `privacyPolicyAccepted`: A boolean indicating acceptance.
    *   `privacyPolicyAcceptedAt`: Timestamp of your acceptance.
    *   `policyUrl`: The URL of the policy you accepted.
    *   `userAgent`: Information about your browser and operating system.
    *   `IP Address`: Your IP address at the time of acceptance. This is collected for legal compliance and audit purposes to demonstrate valid consent.
*   **Payment Information (Reference IDs):** We do not store full credit card or payment details. Payments are processed by third-party providers (Cashfree). We store a `payment reference ID`, your `tier` (e.g., Free, Plus, Pro, Max), and `lastPaymentId` to verify subscription status and manage access to premium features.
*   **Custom System Prompts:** For users with specific subscription tiers (e.g., Max tier), custom system prompts may be collected if you choose to provide them. These are treated as part of your session data and are subject to the same retention policies.
*   **User-Provided Name:** If you provide your name within a chat message (e.g., 
"My name is [Name]"), our system may extract and store this name temporarily within your session for personalization. This name is not permanently linked to your account beyond the active session.

## 3. How We Use Your Data

We utilize the collected data for several essential purposes, all aimed at providing and enhancing your experience with eSAMz AI. Primarily, data is used to **provide and maintain the Service**, which includes generating AI responses, managing your chat sessions, and ensuring the overall functionality of the eSAMz AI platform. For signed-in users, data is crucial for **authentication and account management**, allowing us to verify your identity, manage your account, and grant access to features corresponding to your subscription tier. We also employ data for **security and abuse prevention**, actively detecting and preventing fraudulent activities, unauthorized access, and other security incidents to protect both our users and our infrastructure. Furthermore, data collection supports **legal compliance**, enabling us to meet our obligations, such as demonstrating valid consent under data protection laws. We continuously strive for **service improvement** by analyzing anonymized usage data to understand patterns, debug issues, and enhance the performance and features of our Service. Lastly, data assists in **customer support**, allowing us to respond effectively to your inquiries and provide necessary technical assistance.

## 4. Data Retention

Our data retention policies are designed to be transparent and minimize storage duration:

*   **Session Data:** Your chat session inputs are retained on our servers for a maximum of 30 minutes of inactivity. After this period, they are automatically deleted. If `PRIVACY_MODE` is active, no session history is stored on our servers at all.
*   **Local Browser Storage:** Data stored in your browser's `localStorage` persists until you manually clear it from your browser settings.
*   **Account-Related Data:** This includes your email address, Clerk User ID, privacy policy acceptance records (including IP address and user agent), and payment reference IDs. This data is retained for as long as your account remains active or as legally required for audit purposes. You have the right to request the erasure of this data, as detailed in Section 8.
*   **System Logs:** Minimal technical logs, essential for security and debugging, are retained for short periods, typically 48 hours, before being automatically deleted.

## 5. Data Sharing and Disclosure

We are committed to not selling your personal data. We may share your data with third parties only under specific, necessary circumstances:

*   **AI Model Providers:** To generate responses, your session prompts are sent in real-time to third-party AI model providers, such as the Google Gemma API. Their respective privacy policies govern the processing of your data by these providers, and we ensure our agreements align with our data protection commitments.
*   **Authentication Providers:** We use Clerk for user authentication. Your email address and Clerk User ID are processed by Clerk as part of their service, governed by their privacy policy.
*   **Payment Processors:** For subscription payments, we utilize third-party payment processors like Cashfree. We do not store your full payment details; instead, your payment information is provided directly to these processors, whose privacy policies dictate their data handling. We only retain a payment reference ID and your subscription tier.
*   **Analytics Providers:** Google Analytics is used to understand website traffic and usage trends. This service collects anonymous usage data and may use its own cookies. You will be presented with a cookie consent banner for non-essential cookies.
*   **Infrastructure Providers:** Our services are hosted on Vercel, and we use Upstash Redis for caching. These providers may process data as part of their infrastructure services, and their privacy policies govern their data handling practices.
*   **Legal Requirements:** We may disclose your personal data if legally mandated or in response to valid requests from public authorities, such as a court order or government agency.
*   **Business Transfers:** In the event of a merger, acquisition, or sale of all or a portion of our assets, your personal data may be transferred to the acquiring entity.

## 6. Data Security

We implement robust technical and organizational measures to protect your personal data from unauthorized access, disclosure, alteration, or destruction. These measures include encryption, stringent access controls, and regular security assessments. However, it is important to acknowledge that no method of transmission over the internet or electronic storage can guarantee 100% security. While we strive to protect your data, we cannot ensure its absolute security.

## 7. Children’s Privacy

eSAMz AI is not intended for use by individuals under the age of 18. We do not knowingly collect personal data from anyone under 18. If we become aware that we have inadvertently collected personal data from a child under 18 without verifiable parental consent, we will take immediate steps to delete that information. Our Terms of Service explicitly reflect this age restriction.

## 8. Your Rights as a Data Principal (DPDP Act & GDPR Principles)

As a Data Principal, you are afforded several important rights concerning your personal data, consistent with the DPDP Act and GDPR principles:

*   **Right to Access:** You have the right to obtain confirmation as to whether or not your personal data is being processed, and, where that is the case, access to the personal data and certain information regarding its processing.
*   **Right to Correction/Rectification:** You have the right to request the correction of inaccurate or incomplete personal data concerning you.
*   **Right to Erasure (Right to be Forgotten):** You have the right to request the deletion of your personal data under certain conditions, such as when the data is no longer necessary for the purposes for which it was collected.
*   **Right to Data Portability:** You have the right to receive your personal data in a structured, commonly used, and machine-readable format and to transmit that data to another controller without hindrance.
*   **Right to Withdraw Consent:** You have the right to withdraw your consent to the processing of your personal data at any time. The withdrawal of consent will not affect the lawfulness of processing based on consent before its withdrawal.
*   **Right to Grievance Redressal:** You have the right to register a grievance with our Data Protection Officer or the relevant data protection authority.

To exercise any of these rights, please contact us using the details provided in Section 10. We will respond to your request in accordance with applicable data protection laws.

## 9. Changes to This Privacy Policy

We may update this Privacy Policy periodically to reflect changes in our practices, technology, legal requirements, or other factors. We will notify you of any material changes by posting the new Privacy Policy on this page and updating the "Last Updated" date. We encourage you to review this Privacy Policy regularly for any changes. Your continued use of the Service after any modifications signifies your acceptance of the updated Privacy Policy.

## 10. Contact Us

If you have any questions or concerns about this Privacy Policy or our data practices, please contact us at:

**eSAMz AI Data Protection Officer**
Email: esamzai365@gmail.com

---

**References**

[1] Digital Personal Data Protection Act, 2023. (India). Available at: [https://www.meity.gov.in/content/digital-personal-data-protection-act-2023](https://www.meity.gov.in/content/digital-personal-data-protection-act-2023)
[2] General Data Protection Regulation (GDPR). (EU). Available at: [https://gdpr-info.eu/](https://gdpr-info.eu/)
[3] Clerk Authentication. Available at: [https://clerk.com/](https://clerk.com/)
[4] Cashfree Payments. Available at: [https://www.cashfree.com/](https://www.cashfree.com/)
[5] Google Analytics. Available at: [https://analytics.google.com/](https://analytics.google.com/)
[6] Vercel. Available at: [https://vercel.com/](https://vercel.com/)
[7] Upstash Redis. Available at: [https://upstash.com/](https://upstash.com/)
[8] Google Gemma API. Available at: [https://ai.google.dev/models/gemma](https://ai.google.dev/models/gemma)
