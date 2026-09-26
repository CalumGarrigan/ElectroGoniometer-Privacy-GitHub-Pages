# ElectroGoniometer Privacy Policy site

A small static site for the ElectroGoniometer Google Play privacy-policy requirement.

## Before publishing

Open `index.html` and replace:

`REPLACE_WITH_YOUR_PUBLIC_EMAIL`

with the public email address you want users and Google Play reviewers to use for privacy/support inquiries.

Do not publish the page with the placeholder still present.

## Publish with GitHub Pages

1. Create a **public** GitHub repository named `ElectroGoniometer-Privacy`.
2. Upload the contents of this folder to the repository root.
3. Commit the files to the `main` branch.
4. Open **Settings > Pages** in the repository.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Choose branch **main** and folder **/(root)**.
7. Save.
8. After GitHub publishes the site, your URL will normally be:

   `https://YOUR-GITHUB-USERNAME.github.io/ElectroGoniometer-Privacy/`

9. Open the URL in a private/incognito browser window to confirm that it is accessible without signing in.
10. Paste that HTTPS URL into **Google Play Console > Policy and programs > App content > Privacy policy**.

## Important Play Console consistency

Keep the privacy policy and Play Console Data safety answers consistent with the production app. If ElectroGoniometer later adds cloud sync, analytics, advertising, accounts, online services, new permissions, or third-party SDKs that handle user data, update both the privacy policy and Data safety form before releasing that version.

## Current app behavior reflected in this policy

The policy was prepared against the ElectroGoniometer 2.1.1 project supplied for release preparation. The inspected build:

- stores saved measurements in an on-device SQLite database;
- stores app preferences locally;
- uses device motion/orientation sensor data for angle and quality calculations;
- can store user-entered study ID, participant ID, and notes;
- stores measurement/device metadata including timestamp, device manufacturer/model, Android version, and app version;
- supports user-initiated CSV save/share;
- uses Android FileProvider for share-sheet CSV attachments;
- does not request the Android `INTERNET` permission;
- does not include advertising or analytics SDKs in the inspected Gradle dependencies; and
- provides local measurement deletion and a delete-all control.
