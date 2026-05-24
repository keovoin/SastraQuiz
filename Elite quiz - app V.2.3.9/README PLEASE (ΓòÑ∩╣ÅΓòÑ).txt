
================================================================================
  UPDATING YOUR APP AND ADMIN PANEL
================================================================================

Updating your app and admin panel to the latest version ensures you have
access to new features, improvements, and crucial bug fixes. This guide
provides clear, step-by-step instructions to make the process smooth and
error-free.

---

I. GENERAL UPDATE STEPS
---

Follow these steps carefully to update your app and admin panel.

0.  BACKUP EVERYTHING
    Before starting, create full backups of your existing admin panel
    code, its database, and your app code. This is your safety net.

1.  APPLY CHANGELOGS
    Begin by applying the provided changelogs to your app code, bringing
    it up to the latest version.

2.  ENABLE MAINTENANCE MODE
    To prevent users from encountering issues during the update,
    activate maintenance mode in your admin panel. This will temporarily
    disable the app for all users.

3.  EXECUTE UPDATE SCRIPTS
    Run the update scripts located within your admin panel.

4.  THOROUGHLY TEST
    After the updates, meticulously test both your admin panel and the
    app. Ensure all functionalities work correctly and as expected.

5.  PUBLISH TO APP STORES
    Once you've confirmed everything is working, publish the updated app
    versions to both app stores (e.g., Google Play Store, Apple App
    Store).

6.  FINAL ADMIN PANEL CONFIGURATION
    After the app is published:
    * Enable force update in your admin panel.
    * Add the current app versions.
    * Disable maintenance mode.

7.  IMPORTANT NOTE
    Panel downgrades are not supported. If you update the panel, you
    MUST also update the app to maintain compatibility.

---

II. UPDATING THE ADMIN PANEL
---

Updating the admin panel is straightforward. You'll need to upload the
specific update script for your version transition (e.g.,
'1.0.0-to-1.0.1.zip').

You can find this update script by:
* Unzipping the new admin panel code zip.
* Navigating to the 'Update Scripts Folder' inside the unzipped content.

Then, upload this zip file within the 'System Update Section' of your
admin panel.

---

III. UPDATING YOUR APP: TWO METHODS
---

There are two primary ways to update your app. Choose the method that
best suits your technical comfort and the extent of the changes in the
new update.

>>> METHOD 1: STARTING FROM SCRATCH (RECOMMENDED) <<<
--------------------------------------------------------------------------------

This method is generally the EASIEST and LESS PRONE TO ERRORS,
especially if you're less technical or if the update involves
significant changes.

STEPS:
1.  PREPARE THE NEW APP CODE
    Start with the new app code provided.
2.  RE-CUSTOMIZE
    You'll need to re-apply your branding and assets, which you should
    already have ready.
3.  CONFIGURE
    Change the package name, app name, and update your configuration
    files.
4.  CONNECT
    Reconnect your app with Firebase and your admin panel.
5.  TEST AND PUBLISH
    Thoroughly test the app to ensure everything works, then publish it
    to the app stores.

---

>>> METHOD 2: USING CHANGELOGS AND 'CHANGED-FILES' FOLDER <<<
--------------------------------------------------------------------------------

This method involves manually applying specific changes.

A. USING THE 'Changelog.txt' FILE
--------------------------------------------------------------------------------

The 'Changelog.txt' file details all modifications, additions,
deletions, and renames in the new update. You'll need to go through this
file entry by entry and apply the changes manually using the new app
code as a reference against your current code.

* ADDED OR MODIFIED FILES:
    If a file was added or modified, copy it from the new app code and
    paste/replace it in your project.
* RENAMED FILES:
    Rename the corresponding file in your code.
* DELETED FILES:
    Delete the specified files from your code.

B. USING THE 'Changed-files' FOLDER
--------------------------------------------------------------------------------

For added and modified files, you can streamline the process using the
'Changed-files' folder. This folder contains the updated files organized
with the same structure as the app code.

1.  COPY AND PASTE
    Simply copy all files from the root of the 'Changed-files' folder
    and paste them directly into your project's root. This will
    automatically add new files and update existing ones, saving you
    from manual, tedious copying.

2.  MANUAL DELETIONS AND RENAMES
    You will still need to manually delete any specified files and check
    for any renamed files as instructed in the changelog.

---

!!! IMPORTANT CONSIDERATIONS !!!
--------------------------------------------------------------------------------

* RECOMMENDATION: This approach is best when there aren't many changes
  in the update, or if there are numerous added/modified files that are
  not heavily linked to critical configuration or rebranding files.

* CAUTION: Be careful when using the 'Changed-files' folder, especially
  if configuration files or files containing rebranding information have
  also been changed in the app code. Copying these directly might
  overwrite your existing customizations. Always ensure you have a
  backup, and if necessary, manually re-integrate your changes into the
  updated config files.


================================================================================
  FREQUENTLY ASKED QUESTIONS (FAQ)
================================================================================

Here are some common questions you might have about the update process.

Q1: WHY SHOULD I UPDATE MY APP AND ADMIN PANEL?
A1: Updates provide new features, performance improvements, bug fixes,
    and security enhancements. Staying updated ensures your app is
    stable and secure.

Q2: IS BACKUP REALLY NECESSARY?
A2: ABSOLUTELY! Backing up your code and database is crucial. It acts
    as a safety net, allowing you to restore your system if any
    unforeseen issues occur during the update process.

Q3: WHAT IS MAINTENANCE MODE AND WHY IS IT NEEDED?
A3: Maintenance mode temporarily disables your app for users. This
    prevents them from encountering errors or incomplete features
    while you are performing critical updates, ensuring a smooth
    transition.

Q4: WHAT HAPPENS IF I ONLY UPDATE THE ADMIN PANEL?
A4: Panel downgrades are not supported. If you update the panel, it is
    IMPERATIVE to also update the app to ensure compatibility and
    proper functionality. Mismatched versions can lead to errors.

Q5: WHICH APP UPDATE METHOD IS RECOMMENDED AND WHY?
A5: Method 1 (Starting from Scratch) is generally recommended. It's
    easier and less error-prone, especially for less technical users
    or when updates involve many changes. It ensures a clean new base.

Q6: WHEN SHOULD I USE THE CHANGELOG AND 'CHANGED-FILES' METHOD?
A6: This method is suitable when updates are minor, or when there are
    many added/modified files but few changes to core configurations
    or rebranding-related files.

Q7: WILL MY CUSTOMIZATIONS BE AFFECTED BY THE UPDATE?
A7: Yes, potentially. If you used Method 2 (Changelog/Changed-files)
    and your customized files (e.g., config, branding) are part of the
    update, they might be overwritten. Always backup, and re-integrate
    your customizations manually if needed.

Q8: WHAT IF I ENCOUNTER AN ERROR DURING THE UPDATE?
A8: Refer to your backups. If you followed the backup steps, you can
    revert to your previous working version. Document the error and
    contact support with details for assistance.

Q9: HOW LONG DOES THE UPDATE PROCESS USUALLY TAKE?
A9: The duration varies depending on the update's complexity and your
    chosen method. Backups and thorough testing will add to the time.
    Plan for adequate downtime.

Q10: DO I NEED TO REPUBLISH MY APP AFTER EVERY ADMIN PANEL UPDATE?
A10: If the admin panel update necessitates an app update for
     compatibility (as noted in step I.7), then yes, you must publish
     the updated app to the stores.



