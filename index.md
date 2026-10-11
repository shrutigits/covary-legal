---
title: Covary privacy policy
---

# Covary privacy policy

**The test version.** The version of Covary in TestFlight and Google Play testing sends your data to Covary's development API, which runs on Google Cloud with the same services as the rest of this policy. Feedback is sent from inside the app in every version, and section 2.7 says what it holds. The test tools of Apple and Google also have their own feedback forms, which are theirs. Everything below describes the released app.

Covary is a wellness app for women's health. It helps you log how you feel, compare yourself anonymously with women like you, talk to a companion, read and write in a community, and build a report you can take to a doctor. Covary is not a medical device and does not diagnose.

Your use of Covary is also covered by the [terms of use](https://shrutigits.github.io/covary-legal/terms).

This policy says exactly what Covary does today. Nothing here describes a plan. Where a part of Covary is built but not switched on, this policy says so.

## 1. Who runs Covary and how to reach it

| | |
|---|---|
| Operator | Shruti Dwivedi |
| Registered address | 8 Enggor St, Singapore 079718 |
| Contact for privacy questions | appsforbetterlife330@gmail.com |
| Data protection officer | Shruti Dwivedi, appsforbetterlife330@gmail.com |
| Representative in the European Union | None yet. Covary is not open in the EEA, and a representative is appointed before it opens |
| Grievance officer for India | Shruti Dwivedi, appsforbetterlife330@gmail.com |

Covary has no email sending of its own today, so the contact address above is read by a person, not answered by the app.

## 2. What Covary collects

### 2.1 Account and identity

| What | Why | Encrypted with a key that belongs to your record alone |
|---|---|---|
| Phone number, and a keyed hash of it | Sign-in, and finding an invite that was sent to you | No |
| Sign-in identifier from Google Cloud Identity Platform, Apple or Google | Sign-in | No |
| Email address, if you add one | Contacting you about your account | No |
| Name, date of birth, country, state, city, language, gender, sex at birth | Showing your data back to you, the age floor for your country, and the language screens are shown in | No |
| One-time sign-in code, stored as a hash, with the number of attempts | Checking the code you type | No |
| Invite code, who invited whom, a keyed hash of the invited phone number, the channel and the join time | The invite gate: a new phone number needs an unused invite code to create an account, and sharing invites unlocks comparison | No |
| For a member permanently removed from the community: a keyed hash of her phone number | Stopping her from opening a new Covary account with the same number. It is kept after her account is deleted, for as long as Covary runs, unless the removal is overturned on appeal | No |
| A record that an account was deleted, with no personal data in it | Showing that a deletion was carried out | No |
| The link between your account and your health record | Keeping identity and health data apart | No |

To open an account you have to give your phone number, your name, your date of birth, your country, your state where your country has states, your city, the language you want, your gender and your sex at birth. Without all of them the account cannot be created, because the age floor, the screens and your own record are built from them. Your email address is optional, and so is everything you log after that. A new phone number also needs an unused invite code.

Your city is asked for at sign-up, stored, shown back to you in Settings and included in your export. Its one use is the snapshot taken when you send feedback (section 2.7).

### 2.2 Health logs, profile answers and consent

| What | Why | Encrypted with a key that belongs to your record alone |
|---|---|---|
| Every log entry: periods and cycle, body, sleep, movement, fertility planning and Check answers, with the value, unit, times, where it came from and its status | Your log, your charts, your reports and, if you allow it, anonymous comparison | Free text inside an entry, such as a medicine name: yes. The numbers and the options you picked stay readable, because comparisons are worked out from them |
| Your own words behind an entry | Keeping what you actually wrote | Yes |
| Your journal: the text you write, and the files and photos you add to it | Your private journal. It needs your "Store and analyse my health data" consent and does not need the companion. Journal files are always kept | Yes, the text and the files |
| Profile answers kept as versioned periods of time, including your age at your first period and, if your periods have stopped for good, your age at your last | Your health history, and the context the app needs | Your own words, and free text inside an answer such as a medicine name or anything you type under "Other": yes. The options you pick and the dates: no |
| Your situation, with the evidence behind it, including notes in your own words | Choosing what to show you | Your notes in your own words: yes. The rest: no |
| Topics you chose to skip | Not asking you again | No |
| Your answer to a question about a missing period or a period with no end: the kind of question, the dates and your answer | Not asking you again. Nothing you logged is changed by the answer | No |
| A copy of your log on your phone | Logging and charts without a network | No. It is ordinary app storage on your device |
| One receipt for each consent answer: the purpose, your answer, the version, the language, which translation of the text you saw, where you answered it and when | Showing what you agreed to, and checking it on every read | No |
| The time the comparison layer was unlocked for you | The invite gate | No |

Your situation means where you are in your health at a given time, for example whether you are pregnant, trying to conceive, breastfeeding or recovering from surgery.

Answering "When did your last period start?" with a date writes a period start entry on that date, the same as if you had logged it. "Don't remember" writes nothing. Your answers to the missing-period and unclosed-period questions are included in your export.

If you speak your journal entry, the recording is sent to the AI service for transcription. This needs the companion switched on. The recording is not stored and the transcript is not logged.

### 2.3 Companion messages, voice and your Safe

| What | Why | Encrypted with a key that belongs to your record alone |
|---|---|---|
| Chat messages, already masked on your phone | The conversation | Yes |
| Session details: kind, condition, message counts | Running the conversation | No |
| Every AI call's output, model, prompt version, timing and which log lookups happened | Checking what the AI said and catching mistakes | Voice transcripts and the exact words pulled out of your message: yes. The rest: no |
| Crisis events: which screen, which category, which country | Showing the safety card and counting how often it fires | No |
| Reports you built, as lines you can edit | Your doctor's report | Yes, every line you can edit |
| Your Settings choice "Save photos and files to Safe", off unless you turn it on | Deciding whether a photo or file you send the companion is kept in your Safe or deleted as soon as the companion has read it | No |
| Photos and files you send the companion | Reading them. They go to your Safe only if "Save photos and files to Safe" is on. Otherwise they are deleted once the companion has read them. Reading them needs the companion switched on | See the next row |
| Files in your Safe: kind, type, size, storage key, a checksum, how it was captured, and the file itself | Holding documents you upload | Files are not encrypted with your own key. The file storage service, Cloud Storage, is connected in the development project for the test version and encrypts them: see the note at the end of section 8 |

Before a companion message leaves your phone, Covary removes your name, your phone number, email addresses, web links, card-like numbers and long runs of digits from the text. Dates are kept. Only companion messages are masked: feedback and community posts are sent as you wrote them.

The microphone button is also on notes, the journal, community posts and replies. Speech is sent to the AI service for transcription and needs the companion switched on. Transcripts are kept in the log of AI outputs, encrypted, except journal transcripts, which are not logged. Every transcript is checked for words that signal a crisis, and the emergency card is shown if they do.

### 2.4 Community

| What | Why | Encrypted with a key that belongs to your record alone |
|---|---|---|
| Username and avatar | How other members see you | No |
| Your community membership: when you joined and which version of the community rules you agreed to. You agree again when the rules change | Showing that you agreed to the rules | No |
| Posts and replies, and their machine translations | The community | No |
| Reactions and blocks | Showing counts, and hiding people you block | No |
| Reports you file or receive | Moderation | What you write when you report a post or a person: yes. A report someone files about you was written with their key, not yours, so you never see its words |
| Moderation decisions, the rule applied, the admin's note and your appeal | Moderation, and telling you the outcome | What you write in an appeal: yes. The decision, the rule and the admin's note: no |

### 2.5 Device, push and app settings

| What | Why | Encrypted with a key that belongs to your record alone |
|---|---|---|
| Platform, install id, and when the device was checked. Your push token is stored once, with your health record, not with this row | Sending notifications to the right device | No |
| Notifications and your category preferences | The notification list inside the app | No |
| Sign-in tokens on your phone | Keeping you signed in | Held by the phone's keychain or keystore |

### 2.6 Audit and security records

| What | Why | Encrypted with a key that belongs to your record alone |
|---|---|---|
| Audit lines for consent changes, every write, exports, deletions, moderation and any unusually large read of your entries. Ids and codes only, never a phone number, name, email or health value | Showing what happened to your data | No |
| A line for every use of the link between your account and your health record, with the reason recorded | Showing every time your account and your health record were connected, and why | No |
| Emergency admin sessions, with the reason | Security | No |
| Rejected network traffic | Security | No |

Covary does not collect usage analytics or crash reports. There is no analytics, advertising, attribution or crash-reporting code from any other company in the app. TestFlight and Google Play testing give Apple and Google their own crash and usage reports for the test version; that is their tooling, not Covary's.

### 2.7 Feedback

| What | Why | Encrypted with a key that belongs to your record alone |
|---|---|---|
| Your feedback message, up to three screenshots, and a snapshot taken when you send it of your email address, country, state, city, the page you were on, the app version and the update id | Reading what you sent. Feedback is read on the admin dashboard and is never shown back to you | No. The message and the snapshot are stored plain, and the screenshots go to file storage under their own key, not into your Safe |

Feedback can be sent from inside the app in every version. It is linked to your account, stored as plain text, deleted with your account (screenshots first, then the rows) and not in your export.

### 2.8 Data that comes from other people or other places

- **Invite contacts.** When you invite someone, your phone's contact picker opens on your phone. Only the one number you pick is sent, and it is stored only as a keyed hash.
- **Health stores on your phone.** Apple Health and Health Connect are not read. The reader is not built, and what each platform needs to read them is left out of the app on both: the Health Connect read permissions on Android, and the HealthKit entitlement and its usage strings on iOS.
- **Posts by other members.** Posts and replies written by others may mention your username. They are stored under their author's account and are visible to every community member.

## 3. Why Covary uses your data, and the legal basis

Nothing is ever pre-ticked. Each answer you give is recorded as its own receipt with the version, the language and the time.

| Purpose | Your toggle, exactly as it is shown | Legal basis |
|---|---|---|
| Keeping your health data and showing it back to you | "Store and analyse my health data" / "Data is encrypted and never used to train AI models." (required) | Your explicit consent |
| Comparing you anonymously with other women | "Include me in anonymous comparisons" / "No one can identify me." | Your explicit consent |
| The AI companion, including letting it read your logs while it answers | "Let the companion help" / "It reads what I write and looks at my logs." | Your explicit consent |
| Product news and offers | "Send me tips and updates" / "New features, health content, and offers." | Your consent |
| Medical research | "Help medical research" (off unless you turn it on) | Your explicit consent |

Sign-up shows four of these choices. The fifth, medical research, is in Settings only.

"Store and analyse my health data" cannot be turned off, because Covary cannot work without it. To stop it, delete your account. Turning any other toggle off takes effect on the next query: your data is skipped from then on. Turning a toggle off stops the use from then on. It does not undo what was already done while it was on, and what was already done stays lawful.

Everyone who allows comparison is compared with the same group: every other woman who allows it. Values are worked out over every consenting woman. The cycle comparison places you against that group by your cycle length, your cycle variation and your period length, and figures from published research are blended into the bars, which is why they carry the footnote "Based on app users and published research". A group is shown only when enough women are in it; below that number the comparison says there is not enough data. This is what backs "No one can identify me." Nothing about you narrows that group today, not your age, your country, your situation or your condition. Narrowing is switched off in the settings file and is not built.

Other bases, used only where the app really does this:

| Purpose | Legal basis |
|---|---|
| Creating your account, signing you in, sending a one-time code, keeping the app working | Performance of the agreement with you |
| The community: your username and avatar, your posts and replies, your reactions and blocks | Performance of the agreement with you, for running a feature you chose to use (GDPR Article 6(1)(b)). For any health detail you write into a post, your own act of publishing it to the other members (GDPR Article 9(2)(e)) |
| Keeping consent receipts and the record that a deletion was carried out | Legal obligation, to be able to show that consent was given and that your request was done |
| Security: rate limits, device checks, audit lines, emergency admin access, and community moderation | Legitimate interests in keeping the service and its members safe |
| Keeping a keyed hash of the phone number of a member permanently removed from the community | Legitimate interests in keeping the community safe, by stopping a removed member from signing up again |

Health data is never used for advertising, and is never used to train AI models.

"Send me tips and updates" and "Help medical research" are recorded and nothing uses them yet. No marketing message is sent, and no research use of any kind is happening.

## 4. Automated processing

When the companion is switched on, the AI:

- reads the message you send, after your phone has masked it,
- writes a reply,
- pulls out possible log entries, from your message or from a file you add to your Safe, which are saved as "to confirm" and count for nothing until you confirm them yourself,
- looks at your logs while it answers,
- screens every community post before it is translated or shown, and translates posts. This runs on every post, whether or not you use the companion.

No decision with a legal effect or anything close to it is automated. Some community steps run by themselves, by fixed rules:

- A post the AI screening holds back is shown to you as being reviewed, and a person keeps it or removes it.
- A post reported by two different members is hidden until a person decides.
- A person running Covary can also warn, suspend or permanently remove a member after a report about her.
- Three removals in 30 days give a 7-day suspension from posting and replying.
- A second suspension gives a permanent removal from the community.

These steps limit posting and replying only. Posts are limited to 20 a day, and 5 a day in your first 72 hours. Feedback is limited to 10 a day. You can still read, log, use the companion and sign in. If a post is removed you are told which rule it broke. You get one appeal for a removal, a suspension or a permanent removal.

The models behind Vertex AI come from Google (Gemini) and Anthropic (Claude). Google Cloud Vertex AI runs both, at location global. What is sent to the model: masked chat text and chat history, your age and country, your situation codes, sensitivity flags, your time zone and local date, chart facts, the log item codes and the log rows fetched for an answer, photos and PDF documents sent for extraction, voice recordings sent for transcription, community post text for screening and translation, and conversation turns for summaries. Your display name is not sent. Community posts are sent as written, for screening and translation.

Predictions of your next period, your cycle day and your phase are worked out by fixed rules, not by the AI: from your own entries and your answers to the Periods & Cycle questions until three complete cycles are logged, and from your own cycles after that. They have no legal effect.

The AI provider, Vertex AI, is connected in the development project for the test version.

## 5. Who receives your data

| Receiver | What it gets, and why | Status |
|---|---|---|
| Google Cloud, Singapore (asia-southeast1) | Everything in section 2. Google Cloud runs the database, the servers, the file storage, the keys and the logs | In use in the development project for the test version. Production is not in use |
| Google Cloud Identity Platform, global | Phone number, email, Apple and Google sign-in identifiers, for sign-in | In use in the development project for the test version |
| Google Cloud, Vertex AI, location global | Models from Google (Gemini) and Anthropic (Claude), both run by Google Cloud Vertex AI at location global. Sent: masked chat text and chat history, your age and country, situation codes, sensitivity flags, time zone and local date, chart facts, the log item codes and the log rows fetched for an answer, photos and PDF documents sent for extraction, voice recordings sent for transcription, community post text for screening and translation, and conversation turns for summaries | In use in the development project for the test version. Its settings are not verified yet |
| Apple | Sign in with Apple. Push notifications, HealthKit and the App Store | Sign-in is in use from the phone only; the server does not contact Apple yet. Push is not in use until the push sender is built. HealthKit is not read at all |
| Google | Sign in with Google. Push notifications, Health Connect and the Play Store | Sign-in is in use from the phone only; the server does not contact Google yet. Push is not in use until the push sender is built. Health Connect is not read at all |
| Google Cloud Identity Platform (sends the one-time code) | Your phone number and the one-time code | Not in use until SMS is connected. No real code is sent today |
| Expo, United States | On every launch the released app asks Expo's update servers whether newer app code is available, sending device and runtime details. No account or health data | In use in the released app. The test version has this check switched off |

Pushes, when they start, carry a category code and a row id only. No health detail ever goes to Apple or Google that way.

### Cross-border transfers

Everything in the database and in file storage stays in Singapore. What would leave Singapore:

| What leaves | To | Where | Status |
|---|---|---|---|
| Masked chat text and chat history, age, country, situation codes, sensitivity flags, time zone, local date, chart facts, log item codes and log rows, photos, PDF documents, voice recordings, post text, and conversation turns | Vertex AI (Google Gemini and Anthropic Claude) | Global location | In use in the development project for the test version |
| Phone number and one-time code | Google Cloud Identity Platform | Depends on your country | Not in use |
| Push token, a category code and a row id | Apple and Google push services | United States | Not in use |
| Apple and Google sign-in identifiers | Apple, Google | United States | In use, from your phone. The server does not contact Apple or Google |
| App rules and settings files, which hold no personal data | Content delivery edge locations | In most regions (price class 200) | In use |
| Device and runtime details, when the app checks for an update | Expo | United States | In use in the released app; switched off in the test version |

The transfers happening today are the Apple and Google sign-in identifier, which leaves from your phone when you sign in, the update check to Expo, and the calls to Vertex AI in the test version. The first two do not go through Covary's servers.

Safeguards for these transfers: the Google Cloud data processing agreement, which includes the EU Standard Contractual Clauses, is accepted, and a transfer impact assessment, a written check that the country the data goes to protects it well enough, is written.

## 6. How long data is kept

Everything you log is kept until you delete it or delete your account. There is no other rule.

| What | How long |
|---|---|
| Database backups | 35 days |
| Keyed hash of the phone number of a member permanently removed from the community | For as long as Covary runs, unless the removal is overturned on appeal, when it is deleted. It stays after her account is deleted and is used only to stop that number from signing up again |
| Keyed hashes of invited phone numbers | 5 years. An internal route deletes every invite row that still holds a hashed phone number past that window. It runs when it is triggered, not on a timer |
| One-time sign-in codes | 10 minutes |
| Rate-limit counters | Reset at the end of each window; the rows stay |
| Export and Safe download links | 15 minutes, then a new link is made when you ask again |
| An export build that stalls | Marked failed after 10 minutes |
| Comparison results held for speed | 24 hours, and cleared completely the moment anyone withdraws comparison consent |
| Translations of community posts | Kept for as long as the post exists |
| Application logs | 90 days |
| Rejected network traffic logs | 90 days |
| Emergency admin access logs | 10 years |
| The cloud key, if it is ever scheduled for deletion | 30 days. The cloud key service, Cloud KMS, is connected in the development project for the test version: see the note at the end of section 8 |
| The record that an account was deleted, holding no personal data | Kept indefinitely |
| The log of AI outputs | Kept until your account is deleted |
| Crisis events | Kept until your account is deleted |
| Lines recording use of the link between your account and your health record | No limit is set. They stay after your account is deleted |
| Audit lines | 90 days, with the application logs, and they stay after your account is deleted |
| Your consent receipts | Deleted with your account |
| Files in your Safe | Until you delete them or delete your account |
| An export you built | Until you delete your account |

When you delete your account: everything you logged is deleted and cannot be recovered. This includes your journal and its files, your consent receipts, your community membership record and your moderation history. Your posts are deleted too, except posts that other members replied to, which stay as "Post deleted". The reports you filed are deleted. What you wrote in your own words is deleted with your data key. What is kept: the record that an account was deleted, the invite records with a keyed phone hash (up to 5 years), the phone hash of a permanently removed member (as long as Covary runs, unless the removal is overturned on appeal), the audit lines and the lines recording use of the link between your account and your health record (section 6), and backups (35 days). A backup taken before you deleted can still hold your data key and your data until it expires, within 35 days.

No other retention limit exists anywhere in Covary.

## 7. Your rights and how to use them

| Right | How to use it in the app |
|---|---|
| A copy of your data, in a form you can take elsewhere | Settings, "Download everything". You get JSON files for your onboarding details, your logs, your journal and its files, and the messages you wrote to the companion and in the community, plus your uploaded files and photos and a short readme, through a link that lasts 15 minutes and can be made again. The export does not include your feedback or your consent receipts |
| Deletion | Settings, "Delete my account". Your data key is destroyed and any backup still holding it expires within 35 days, your files, your feedback with its screenshots and any export you built are deleted, every health row is hard-deleted, comparison results are cleared, and your phone is wiped of its local copy and its tokens |
| Correction | Edit the entry, or your profile, in the app. The old version is kept as superseded and the new one replaces it, so nothing is rewritten behind you |
| Withdrawing consent | Settings, Privacy. Five toggles (four shown at sign-up, medical research only here), each change recorded as its own receipt. Withdrawing stops future use and does not undo what was already done. |
| Objecting to comparison | Turn off "Include me in anonymous comparisons". You leave every future comparison and the stored results are cleared at once |
| Objecting to the uses based on legitimate interests | Security records, emergency admin access and community moderation rest on legitimate interests. Ask at the contact address in section 1. There is no screen for this |
| Restriction: asking Covary to hold your data and stop using it | Ask at the contact address in section 1, for example while a correction or an objection is being settled. There is no screen for this |
| Naming someone to act for you if you die or cannot act for yourself | The Digital Personal Data Protection Act 2023, section 14, lets you name a nominee. Write to the contact address in section 1 with the person's name and how to reach them. There is no screen for this |
| Complaining | You can complain to the data protection authority in your country. In India this is the Data Protection Board of India |

Requests are answered within one month. Covary does not promise a shorter time than that.

## 8. Security

- Traffic between your phone and Covary is encrypted. File storage and the database refuse any connection that is not encrypted. There is no certificate pinning.
- Everything in the database is encrypted where it sits, with one key that belongs to Covary and is replaced on a schedule. The people who look after that key cannot read the data with it.
- Almost all of your free text is additionally encrypted with a key that belongs to your record alone: your own words behind a log entry, your journal text and files, free text inside an entry or a profile answer such as a medicine name, your chat messages, your notes about your situation, your report lines, what you write when you report a post or a person, what you write in an appeal, voice transcripts, and the exact words pulled out of your messages. Three kinds are not: your community posts, which other members read and which are machine-translated, an admin's own note on a moderation decision, and your feedback message and screenshots, which are read on the admin dashboard. Those are protected by the storage encryption above.
- Your identity details and your health data sit in separate parts of the database, with separate passwords and no route from one to the other. One link joins them, and it can be used in four ways. Three of the four need a written reason, and all four write a line to an access log.
- Deleting your account destroys your data key, then the files, then the rows. A backup taken before you deleted can still hold your data key and your data until it expires, within 35 days.
- Your consent is checked at the moment of every read, in one place, including inside the queries that build comparisons.
- Requests to Covary are logged with the route and the result only. On the fifteen kinds of route that carry personal data the query text is dropped as well, and nothing you send inside a request is written to a log on any route.
- There is a limit of 10 invites for each member, and there are limits on how often you can sign in, message the companion, build a report, export, upload to your Safe and report a post.
- Admin access to production is not standing. An emergency credential lasts one hour, needs a written reason, and raises an alert to the developer before any data is touched.
- You can lock Covary with your phone's own biometric or passcode. Covary never stores a PIN of its own. The app draws a cover over its own screen before it goes into the app switcher; it cannot stop screenshots or screen recording: on Android this needs a native setting the app does not have yet; on iOS no such setting exists. A neutral app icon can be chosen when the app is built; switching it from inside the app does not work yet.
- One Google Cloud project, the development project, holds the test version. Production is not in use.
- Every change is checked automatically before it ships, for known weaknesses in the code, for secrets left inside it and for other people's code with known vulnerabilities, and updates to that code are proposed every week.

Three services behind this section are connected in the development project for the test version: the key service (Cloud KMS) holds your key, the file storage (Cloud Storage) holds Safe files and export archives, and the sign-in service (Identity Platform) holds your sign-in user.

Covary is not end-to-end encrypted. End-to-end encryption means only your phone holds the key, and that is incompatible with computing comparisons on the server. This policy says exactly what is built and nothing stronger.

## 9. Age

You must be at least 16 to use Covary, and at least 18 in India and Indonesia. Age is self-declared from the date of birth you give. It is checked once, at sign-up, against the country you enter. If it is below the floor for that country, you cannot continue. It is not checked again later. Your age at your first period and, if your periods have stopped for good, your age at your last are profile answers and play no part in this check.

## 10. Where Covary is not available

At launch Covary is closed in the countries of the European Economic Area and in the United Kingdom, because the data protection officer, the EU representative and the data protection impact assessment must exist first. It is also closed in China and in Russia, because both restrict where personal data may be stored and how it may leave the country, which needs separate infrastructure and legal work. The country is checked once, at sign-up, on the country you enter.

## 11. Changes to this policy

When Covary changes what it collects, why, or who receives it, this policy is updated and a new version is published in the app before the change takes effect. A future material change also raises the consent version, which shows the Consent screen again.

Version 1.1. Published 11 October 2026. Version 1.0 was published 20 September 2026.
