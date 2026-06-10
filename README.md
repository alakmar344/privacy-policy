# Privacy Policy - eSAMz AI

**Last Updated: June 10, 2026**

This Privacy Policy describes how eSAMz AI ("we," "us," or "our") collects, uses, processes, and protects your personal data when you use our AI assistant services (the "Service"). We are committed to safeguarding your privacy and ensuring compliance with applicable data protection laws, including the Digital Personal Data Protection Act (DPDP), 2023, of India, and principles aligned with the General Data Protection Regulation (GDPR). This policy applies to all users of eSAMz AI, including both anonymous visitors and registered users.

## 1. Your Consent

By accessing or using the eSAMz AI Service, you acknowledge that you have read, understood, and agree to the terms of this Privacy Policy. For the processing of your personal data, we obtain your explicit, informed consent through clear affirmative action. Before processing any personal data, you will be presented with a standalone notice detailing:

- The categories of personal data being processed.
- The specific purposes for which your personal data is processed.
- Your rights as a Data Principal under the DPDP Act and other applicable laws.
- The mechanism for exercising these rights and for grievance redressal.
- Contact information for our Data Protection Officer or designated contact person.

Your consent is specific to each purpose and will not be implied by your continued use of the Service. You have the right to withdraw your consent at any time, which will result in the permanent deletion of your account and all associated data as detailed in Section 9.

## 2. Data We Collect and Process

We minimize data collection to what is strictly necessary to provide and improve our Service. The types of personal data we collect and process depend on how you interact with eSAMz AI.

### 2.1. Data Collected from All Users (Anonymous and Signed-in)

- **Session Prompts:** Your input prompts during a chat session are processed in real-time to generate responses. For anonymous users, these are subject to a strict 30-minute retention policy on our servers, after which they are automatically wiped. If `PRIVACY_MODE` is enabled on our servers, no session history is stored at all.
- **Minimal System Logs:** We maintain minimal technical logs strictly for security, debugging, and abuse prevention. These logs may include request timestamps, response codes, and anonymized usage data. Access logs are retained for short periods (typically 48 hours) and then automatically deleted.
- **Local Browser Storage:** Your chat history, session IDs, and user preferences are stored locally on your device using `localStorage` (keys: `esamz_conversations_v9`, `esamz_last_chat_id`). We also utilize `sessionStorage`, `IndexedDB`, and the `Cache API` for application state, service worker functionality, and authentication persistence. This data is not transmitted to our servers unless you are signed in. You can clear this data by clearing your browser's local storage, cookies, or by using the in-app data export and deletion features.
- **Technical Identifiers:** We collect your browser's user agent and IP address for security, abuse prevention, compatibility, analytics, and to record your consent to our Privacy Policy and Terms of Service.

### 2.2. Data Collected from Signed-in Users

When you create or sign in to an account using Clerk authentication, we collect and process additional data:

- **Account Information:** Your email address and unique Clerk User ID (`clerkId`) are used for authentication, account management, and security purposes.
- **Privacy Policy Acceptance Records:** When you explicitly accept our Privacy Policy, we record your acceptance in our MongoDB database, including:
  - `privacyPolicyAccepted`: A boolean indicating acceptance.
  - `privacyPolicyAcceptedAt`: Timestamp of your acceptance.
  - `policyUrl`: The URL of the policy you accepted.
  - `userAgent`: Information about your browser and operating system.
  - `IP Address`: Your IP address at the time of acceptance, collected for legal compliance and audit purposes to demonstrate valid consent.
- **Chat History Synchronization:** For signed-in users, chat history may be synchronized with our backend to provide a consistent experience across devices.
- **Custom System Prompts:** If you choose to provide custom instructions through the "System Prompt Editor," these are treated as part of your session data and are subject to the same retention policies.
- **User-Provided Name:** If you provide your name within a chat message (e.g., "My name is [Name]"), our system may extract and store this name temporarily within your session for personalization. This name is not permanently linked to your account beyond the active session.

## 3. How We Use Your Data

We utilize the collected data for the following essential purposes:

- **Providing and Maintaining the Service:** Generating AI responses using the Google Gemma API and Wikipedia RAG via Serper API, managing your chat sessions, and ensuring the overall functionality of the eSAMz AI platform.
- **Authentication and Account Management:** Verifying your identity and managing your account via Clerk.
- **Security and Abuse Prevention:** Detecting and preventing fraudulent activities, unauthorized access, and other security incidents to protect both our users and our infrastructure.
- **Legal Compliance:** Meeting obligations such as demonstrating valid consent under data protection laws, including the DPDP Act, 2023, and GDPR principles.
- **Service Improvement:** Analyzing anonymized usage data to understand patterns, debug issues, and enhance the performance and features of our Service.
- **Customer Support:** Responding effectively to your inquiries and providing necessary technical assistance.

## 4. Cookies and Tracking Technologies

eSAMz AI uses cookies and similar tracking technologies to operate and improve our Service:

- **Essential Cookies:** Required for the functioning of the Service, including session management, authentication persistence via Clerk, and remembering your privacy policy acceptance. These cannot be disabled as the Service will not function without them.
- **Analytics Cookies:** Google Analytics and Vercel Web Analytics may use cookies to collect anonymous usage data. You will be presented with a cookie consent banner for non-essential cookies, and you may opt out through your browser settings.
- **Local Storage Technologies:** We use `localStorage`, `sessionStorage`, `IndexedDB`, and the `Cache API` to store chat history, user preferences, session IDs, and application state locally on your device.

You can manage your cookie preferences through your browser settings. Disabling certain cookies may affect the functionality of the Service.

## 5. Data Retention

Our data retention policies are designed to be transparent and minimize storage duration:

- **Session Data:** Your chat session inputs are retained on our servers for a maximum of 30 minutes of inactivity. After this period, they are automatically deleted. If `PRIVACY_MODE` is active, no session history is stored on our servers at all.
- **Local Browser Storage:** Data stored in `localStorage`, `sessionStorage`, `IndexedDB`, and the `Cache API` persists until you manually clear it from your browser settings or revoke your consent.
- **Account-Related Data:** This includes your email address, Clerk User ID, privacy policy acceptance records (including IP address and user agent), and synchronized chat history. This data is retained for as long as your account remains active or as legally required for audit purposes. Revoking consent triggers immediate deletion from our MongoDB database (including user records, logs, and conversations) and the Clerk authentication system.
- **System Logs:** Minimal technical logs, essential for security and debugging, are retained for short periods, typically 48 hours, before being automatically deleted.

## 6. Data Sharing and Disclosure

We are committed to not selling your personal data. We may share your data with third parties only under specific, necessary circumstances:

- **AI Model Providers:** Google Gemma API receives your prompts in real-time to generate responses.
- **Authentication Providers:** Clerk processes your email and User ID for authentication.
- **Infrastructure Providers:** Vercel (hosting), MongoDB (database), and Upstash Redis (caching).
- **Analytics Providers:** Google Analytics and Vercel Web Analytics collect anonymous usage data.
- **Search/RAG Providers:** Wikipedia and Serper API are used for Retrieval-Augmented Generation.
- **Legal Requirements:** We may disclose your personal data if legally mandated or in response to valid requests from public authorities.
- **Business Transfers:** In the event of a merger, acquisition, or sale of assets, your personal data may be transferred to the acquiring entity. We will notify you prior to any such transfer.

## 7. Data Transfers

Your data may be transferred to and processed in countries other than your country of residence. By using the Service, you acknowledge that your personal data may be transferred to servers operated by our third-party providers (including Google, Clerk, Vercel, MongoDB, Upstash, and Serper), which may be located in various jurisdictions worldwide. We take appropriate safeguards including:

- Ensuring our third-party providers comply with applicable data protection laws, including GDPR standard contractual clauses where applicable.
- Applying encryption in transit (TLS/SSL) for all data exchanges.
- Conducting due diligence on the data protection practices of our service providers.

## 8. Data Security

We implement robust technical and organizational measures to protect your personal data:

- **Encryption:** Data in transit is encrypted using TLS/SSL protocols. Sensitive data at rest is encrypted in our databases and storage systems.
- **Access Controls:** Stringent access controls ensure that only authorized personnel can access personal data on a need-to-know basis.
- **Permission Restrictions:** We explicitly disable browser permissions for camera, microphone, geolocation, and payments at the HTTP header level to enhance security.
- **Regular Security Assessments:** We conduct periodic security reviews and vulnerability assessments.

No method of transmission over the internet or electronic storage can guarantee absolute security. While we strive to protect your data using commercially reasonable measures, we cannot ensure its absolute security.

## 9. Data Breach Notification

In the event of a personal data breach that is likely to result in a risk to your rights and freedoms, we will:

- Notify the relevant data protection authority within 72 hours of becoming aware of the breach, where required by applicable law (including the GDPR).
- Notify you directly without undue delay when the breach is likely to result in a high risk to your rights and freedoms.
- Take immediate steps to contain and remediate the breach, including conducting a thorough investigation and implementing measures to prevent recurrence.

Notifications will be communicated via email to the address associated with your account or through a prominent notice on our Service.

## 10. Children's Privacy

eSAMz AI is not intended for use by individuals under the age of 18. We do not knowingly collect personal data from anyone under 18. If we become aware that we have inadvertently collected personal data from a child under 18 without verifiable parental consent, we will take immediate steps to delete that information from our servers, databases, and all associated systems. Our Terms of Service explicitly reflect this age restriction.

## 11. Automated Decision-Making and Profiling

We do not engage in automated decision-making or profiling that produces legal or similarly significant effects concerning you. While our AI assistant processes your prompts to generate responses, this processing is limited to providing the Service and does not result in decisions that solely determine legal rights, access to services, or similar outcomes. If we ever introduce such processes, we will update this policy and obtain your explicit consent before implementation.

## 12. Your Rights as a Data Principal (DPDP Act & GDPR Principles)

As a Data Principal, you are afforded several important rights:

- **Right to Access:** You have the right to obtain confirmation as to whether or not your personal data is being processed, and access to that data.
- **Right to Correction/Rectification:** You have the right to request the correction of inaccurate or incomplete personal data.
- **Right to Erasure (Right to be Forgotten):** You can delete your account and all associated data by using the "Revoke Consent" feature. This process hard-deletes your record from MongoDB, clears your Clerk account, and wipes all local browser storage (`localStorage`, `sessionStorage`, `IndexedDB`, and `Cache API`).
- **Right to Data Portability:** You can export your chat history as JSON or Markdown directly from the application menu, and transmit that data to another controller without hindrance.
- **Right to Withdraw Consent:** You may withdraw your consent at any time. Revoking consent will stop all processing and initiate immediate data deletion. The withdrawal of consent will not affect the lawfulness of processing based on consent before its withdrawal.
- **Right to Grievance Redressal:** You have the right to register a grievance with our Data Protection Officer or the relevant data protection authority.

To exercise any of these rights, please contact us using the details provided in Section 14. We will respond within 30 days.

## 13. Changes to This Privacy Policy

We may update this Privacy Policy periodically. We will notify you of any material changes by:

- Posting the new Privacy Policy on this page and updating the "Last Updated" date.
- Sending an email notification to registered users for significant changes.
- Displaying a prominent notice within the Service requiring your renewed consent where required by law.

Your continued use of the Service after any modifications signifies your acceptance of the updated Privacy Policy.

## 14. Contact Us

If you have any questions, concerns, or requests regarding this Privacy Policy or our data practices, please contact our Data Protection Officer at:

**eSAMz AI Data Protection Officer**
Email: esamzai365@gmail.com

We will acknowledge receipt of your request within 7 days and respond substantively within 30 days.

## 15. Governing Law and Jurisdiction

This Privacy Policy shall be governed by and construed in accordance with the laws of India. Any disputes arising from or in connection with this Privacy Policy shall be subject to the exclusive jurisdiction of the courts in India. For users located in the European Union, you also have the right to lodge a complaint with your local supervisory authority under the GDPR.

## 16. Severability

If any provision of this Privacy Policy is found to be invalid, illegal, or unenforceable, the remaining provisions shall continue in full force and effect. The invalid or unenforceable provision shall be modified to the minimum extent necessary to make it valid and enforceable, while preserving the intent of the original provision.

---

**References**

1. Digital Personal Data Protection Act, 2023 (India). Available at: https://www.meity.gov.in/content/digital-personal-data-protection-act-2023
2. General Data Protection Regulation (GDPR) (EU). Available at: https://gdpr-info.eu/
3. Clerk Authentication. Available at: https://clerk.com/
4. Google Analytics. Available at: https://analytics.google.com/
5. Vercel. Available at: https://vercel.com/
6. Upstash Redis. Available at: https://upstash.com/
7. Google Gemma API. Available at: https://ai.google.dev/models/gemma
8. MongoDB. Available at: https://www.mongodb.com/
9. Serper API. Available at: https://serper.dev/
10. Wikipedia. Available at: https://www.wikipedia.org