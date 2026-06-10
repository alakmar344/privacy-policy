# Privacy Policy - eSAMz AI

**Last Updated: June 10, 2026**

This Privacy Policy describes how eSAMz AI ("we," "us," or "our") collects, uses, processes, and protects your personal data when you use our AI assistant services (the "Service"). We are committed to safeguarding your privacy and ensuring compliance with applicable data protection laws, including the Digital Personal Data Protection Act (DPDP), 2023, of India, and principles aligned with the General Data Protection Regulation (GDPR).

## 1. Your Consent

By accessing or using the eSAMz AI Service, you acknowledge that you have read, understood, and agree to the terms of this Privacy Policy. For the processing of your personal data, we obtain your explicit, informed consent through clear affirmative action. Before processing any personal data, you will be presented with a standalone notice detailing:

*   The categories of personal data being processed.
*   The specific purposes for which your personal data is processed.
*   Your rights as a Data Principal under the DPDP Act and other applicable laws.
*   The mechanism for exercising these rights and for grievance redressal.
*   Contact information for our Data Protection Officer or designated contact person.

Your consent is specific to each purpose. You have the right to withdraw your consent at any time, which will result in the permanent deletion of your account and all associated data as detailed in Section 8.

## 2. Data We Collect and Process

We minimize data collection to what is strictly necessary to provide and improve our Service.

### 2.1. Data Collected from All Users (Anonymous and Signed-in)

*   **Session Prompts:** Your input prompts are processed in real-time to generate responses. For anonymous users, these are subject to a strict 30-minute retention policy on our servers, after which they are automatically wiped. If `PRIVACY_MODE` is enabled on our servers, no session history is stored at all [1].
*   **Local Browser Storage:** Your chat history, session IDs, and user preferences are stored locally on your device using `localStorage` (keys: `esamz_conversations_v9`, `esamz_last_chat_id`). We also utilize `sessionStorage`, `IndexedDB`, and the `Cache API` for application state, service worker functionality, and authentication persistence [2]. This data is not transmitted to our servers unless you are signed in.
*   **Technical Identifiers:** We collect your browser's user agent and IP address for security, abuse prevention, and to record your consent to our Privacy Policy and Terms of Service [3].

### 2.2. Data Collected from Signed-in Users

When you sign in using Clerk authentication, we collect and process additional data:

*   **Account Information:** Your email address and unique Clerk User ID (`clerkId`) [4].
*   **Privacy Policy Acceptance Records:** We record your explicit acceptance in our MongoDB database, including the timestamp (`privacyPolicyAcceptedAt`), policy URL, user agent, and IP address [5].
*   **Chat History Synchronization:** For signed-in users, chat history may be synchronized with our backend to provide a consistent experience across devices [6].
*   **Custom System Prompts:** If you use the "System Prompt Editor" to provide custom instructions, these are processed as part of your session data [7].
*   **User-Provided Name:** Our system may extract your name from messages (e.g., "My name is [Name]") to personalize responses within the active session [8].

## 3. How We Use Your Data

We utilize the collected data for the following purposes:
*   **Providing the Service:** Generating AI responses using the Google Gemma API and Wikipedia RAG [9].
*   **Authentication and Account Management:** Verifying your identity and managing your account via Clerk [4].
*   **Security and Abuse Prevention:** Detecting and preventing fraudulent activities and unauthorized access [3].
*   **Legal Compliance:** Meeting obligations such as demonstrating valid consent under data protection laws [10].
*   **Service Improvement:** Analyzing anonymized usage data to enhance performance [11].

## 4. Data Retention

*   **Session Data:** Anonymous session inputs are deleted after 30 minutes of inactivity [1].
*   **Local Storage:** Data in `localStorage`, `sessionStorage`, `IndexedDB`, and `Cache API` persists until you manually clear it or revoke your consent [2].
*   **Account Data:** Retained as long as your account is active. Revoking consent triggers immediate deletion from our MongoDB database (including user records, logs, and conversations) and the Clerk authentication system [5].
*   **System Logs:** Technical logs are retained for 48 hours for security and debugging [1].

## 5. Data Sharing and Disclosure

We do not sell your personal data. We share data with third parties only as necessary:
*   **AI Model Providers:** Google Gemma API receives your prompts in real-time to generate responses [9].
*   **Authentication:** Clerk processes your email and User ID for authentication [4].
*   **Infrastructure:** Vercel (hosting), MongoDB (database), and Upstash Redis (caching) [12].
*   **Analytics:** Google Analytics and Vercel Web Analytics collect anonymous usage data [11].
*   **Search/RAG:** Wikipedia and Serper API are used for Retrieval-Augmented Generation [9].

## 6. Data Security

We implement technical and organizational measures, including encryption and access controls, to protect your data. We explicitly disable browser permissions for camera, microphone, geolocation, and payments at the header level to enhance security [13].

## 7. Children’s Privacy

eSAMz AI is not intended for use by individuals under the age of 18. We do not knowingly collect personal data from minors.

## 8. Your Rights (DPDP Act & GDPR)

As a Data Principal, you have the following rights:
*   **Right to Access and Correction:** You can view and update your personal data by managing your account settings or contacting us.
*   **Right to Erasure (Right to be Forgotten):** You can delete your account and all associated data (including logs in MongoDB and your Clerk record) by using the "Revoke Consent" feature. This process hard-deletes your record from MongoDB, clears your Clerk account, and wipes all local browser storage (localStorage, sessionStorage, IndexedDB, and Cache API) [5].
*   **Right to Withdraw Consent:** Revoking consent will stop all processing and initiate immediate data deletion [5].
*   **Right to Data Portability:** You can export your chat history as JSON or Markdown directly from the application menu [2].

## 9. Changes to This Policy

We may update this policy periodically. We will notify you of material changes by posting the new policy and updating the "Last Updated" date.

## 10. Contact Us

For questions or to exercise your rights, contact our Data Protection Officer at:
**Email: esamzai365@gmail.com**

---
**References**
[1] `main(1).rs(1).txt` (Backend Code)
[2] `esamz.a/app/page.tsx` (Frontend Code)
[3] `main(1).rs(1).txt` (Backend Code), `esamz.a/app/api/user/privacy-policy-acceptance/route.ts` (Frontend API)
[4] `esamz.a/app/api/chat/proxy/route.ts` (Frontend API), `esamz.a/app/api/user/tier/route.ts` (Frontend API)
[5] `esamz.a/app/api/user/privacy-policy-acceptance/revoke/route.ts` (Frontend API)
[6] `esamz.a/app/api/chat/proxy/route.ts` (Frontend API)
[7] `main(1).rs(1).txt` (Backend Code)
[8] `main(1).rs(1).txt` (Backend Code)
[9] `main(1).rs(1).txt` (Backend Code)
[10] Digital Personal Data Protection Act, 2023. (India). Available at: [https://www.meity.gov.in/content/digital-personal-data-protection-act-2023](https://www.meity.gov.in/content/digital-personal-data-protection-act-2023)
[11] `esamz.a/app/layout.tsx` (Frontend Code)
[12] `main(1).rs(1).txt` (Backend Code)
[13] `esamz.a/Vercel.json` (Vercel Configuration)
