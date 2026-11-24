# Galaxy Labs

Your Galaxy has more to offer than its settings might suggest. Features still being tested, hidden options, and features that haven’t reached your device yet. Curious about what you can already try?

Welcome to **Galaxy Labs**.

Galaxy Labs lets you explore and enable supported experimental Samsung features. You choose what to try!

## What can you do with it?

Galaxy Labs brings supported tweaks for Samsung apps and One UI together. Depending on your device and installed software, you can:

- Access hidden settings and experimental features.
- Enable features that Samsung doesn’t show by default.
- Manage tweaks for supported apps.

You’ll find the available options in the app. Compatibility depends on your device, One UI version, and the versions of the Samsung apps you’re using.

Making a hidden menu appear doesn’t necessarily mean the entire feature will work. Some features also require newer software, additional components, or support from Samsung’s servers.

## Download

Download the APK from the [latest release](https://github.com/erikhoevik/Galaxy-Labs-Releases/releases/latest), open it on your device, and follow the installation prompts.

If Android asks for permission to install apps from this source, allow it for the browser or file manager you’re using to open the APK.

## Before you start

For features that use root or LSPosed, you’ll need a working combination of:

- **Root access**, such as temporary root through DFRoot.
- **KernelSU** to manage superuser permissions.
- **A Zygisk implementation**, such as NeoZygisk.
- **An LSPosed implementation**, such as Vector.

Use versions compatible with your device and software. DFRoot only works on supported firmware, so the instructions below apply to devices that support this setup.

Already have everything working? Skip ahead to **Enable Galaxy Labs in Vector or LSPosed**.

## 1. Activate temporary root

Make sure **DFRoot** and **KernelSU** are installed on your device.

Open **DFRoot** and tap **Launch root**. If successful, KernelSU should open in **jailbreak mode**, with temporary root active.

Temporary root is lost when you restart your device. Repeat these steps after a restart.

## 2. Grant Galaxy Labs superuser access

1. In **KernelSU**, open the **Superuser** section.
2. Find **Galaxy Labs** and enable superuser access.
3. Reopen Galaxy Labs.

If Galaxy Labs isn’t listed yet, open the app and use a feature that requests root access, then check KernelSU again.

## 3. Set up Zygisk and Vector or LSPosed

Some tweaks require Galaxy Labs to apply changes inside a supported app. For those, you’ll need a Zygisk implementation together with Vector or another compatible LSPosed implementation.

**NeoZygisk** provides Zygisk support. **Vector** provides the LSPosed functionality that lets you activate the Galaxy Labs module for specific apps.

The general setup is:

1. Open the **Modules** section in KernelSU.
2. Install a compatible Zygisk module, such as **NeoZygisk**.
3. Install a compatible LSPosed implementation, such as **Vector**, following that project’s instructions.
4. Complete any required activation steps and restart (soft reboot) if instructed.
5. Check that both Zygisk and Vector or LSPosed are active.

The exact installation steps vary between implementations. Follow the instructions for the versions you’re installing.

## 4. Enable Galaxy Labs in Vector or LSPosed

One more step: choose which apps the module can apply its changes to.

1. Open **Vector** or your **LSPosed manager**.
2. Go to **Modules**.
3. Select **Galaxy Labs** and enable the module.
4. Under **Scope**, select the apps you want to use the tweaks with.
5. Follow the module’s recommended scope.
6. Fully close the affected apps and reopen them.

**Superuser access and LSPosed scope are separate settings.** Granting access in KernelSU doesn’t automatically enable the module in Vector. Make sure both are configured.

## A feature isn’t working

Check the following first:

- Is root still active?
- Does Galaxy Labs have superuser access in KernelSU?
- Are Zygisk and Vector or LSPosed active?
- Is the Galaxy Labs module enabled?
- Is the version of the app installed on your device supported by Galaxy Labs?
- Have you restarted the affected app?

If an option still doesn’t appear or only partly works, your software may be missing something it needs. Sometimes an experimental feature simply isn’t ready yet.

## Installing updates

You can find new versions on the [releases page](https://github.com/erikhoevik/Galaxy-Labs-Releases/releases).

Install an update over your existing installation. Follow any additional instructions in the release notes, and check afterward that the module is still enabled with the correct scope.

## Reporting issues

Found something that doesn’t work as expected? Report it through [Issues](https://github.com/erikhoevik/Galaxy-Labs-Releases/issues).

Please include:

- Your device model.
- Your Android and One UI versions.
- Your Galaxy Labs version.
- The feature you were using and what happened.
- A screenshot or error, with personal information removed.

The more specific your report, the easier it is to investigate.

## Good to know

Galaxy Labs is an independent project and is not affiliated with Samsung.

These are experimental features. Availability and behavior may change after updates to Samsung apps or One UI. Try enabling tweaks one at a time so you know where to look if something unexpected happens.

Enjoy exploring.
