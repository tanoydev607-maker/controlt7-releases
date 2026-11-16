<div align="center">
  <img src="assets/controlt7-logo.png" width="230" alt="ControlT7 red feather and silver hand emblem" />
  <h1>ControlT7</h1>
  <p><strong>Your workspace. Your agents. Your control.</strong></p>
  <p>A local-first AI workspace for Windows, by Anew.</p>
  <p><strong>Windows x64 &nbsp; · &nbsp; Preview &nbsp; · &nbsp; Messenger-style agents</strong></p>
  <p>
    <a href="https://github.com/tanoydev607-maker/controlt7-releases/releases"><strong>Download Preview</strong></a>
    &nbsp; · &nbsp;
    <a href="#getting-started">Getting started</a>
    &nbsp; · &nbsp;
    <a href="#updates">Updates</a>
    &nbsp; · &nbsp;
    <a href="https://github.com/tanoydev607-maker/controlt7-releases/issues">Report a bug</a>
  </p>
</div>

---

## Meet ControlT7

Bring your AI agents into one workspace. Give an agent its own identity, send it a task in a private chat, or bring several agents into a group with different roles: planner, developer, reviewer or tester.

ControlT7 includes Hermes as its default assistant and connects to supported, separately installed coding-agent CLIs. Those agents use their native tools and configuration, with ControlT7 providing the messaging interface, workspace controls and shared integrations.

| In the Preview | What you can do |
| --- | --- |
| **Agent conversations** | Create saved agents with names, pictures and instructions; talk to them in individual messenger-style chats. |
| **Group work** | Assign roles and run agents in parallel using the same visible group-history snapshot. Replies become shared context on the next round. |
| **Native CLI agents** | Add supported installed coding agents, or configure a compatible custom adapter. CLI tools, plugins and provider settings remain native. |
| **Files and previews** | Create projects, folders and files in your workspace, inspect outputs and open supported previews inside the app. |
| **Shared MCP tools** | Configure MCP servers and make compatible tools available to agents through ControlT7's approval flow. |
| **Your model choice** | Connect a supported local inference engine or choose a compatible cloud provider using your own credentials. |

Custom CLIs need a supported messaging protocol or adapter. Automatic MCP setup also requires a compatible MCP client; registering an arbitrary terminal command does not add those capabilities by itself.

## Download

**[Open the releases page →](https://github.com/tanoydev607-maker/controlt7-releases/releases)**

Choose a published Preview release, read its notes, then download the **Windows x64 installer** from **Assets**. Installers follow this naming pattern:

```text
ControlT7_<version>_x64-setup.exe
```

Preview builds may be marked **Pre-release**, so use the releases list rather than relying on GitHub's “Latest” label. If no published build is listed, a public download is not available yet.

GitHub's automatically generated **Source code (zip)** and **Source code (tar.gz)** files are not the desktop installer. This repository holds downloads and update-site files; it does not contain the application's full source.

## Getting started

1. Install the Windows x64 build from a published release.
2. Open ControlT7. Sign-in is optional; choose **Continue offline** to use it without an Anew account.
3. Select a workspace and configure a supported local model or cloud provider. Account sign-in does not supply model access or API credits.
4. Start with Hermes, or install and configure another supported agent CLI through agent setup.
5. Open an agent chat, give it a task, and review any requested approvals. Create a group when you want several agents to work together.

Local inference needs suitable hardware, an inference engine and downloaded model files. Fully offline tasks also need tools that work offline. Cloud models, initial downloads and some integrations require an internet connection; provider charges may apply.

## Updates

In an updater-enabled build, open **Settings → Updates → Check for updates**. When a compatible signed update is published to the Preview feed, the app can show its notes and offer **Install and restart**.

Finish active tasks and close agent terminals before updating. Keep a backup of important workspace files. If no update feed is available, use a published manual installer and follow its release notes.

Updater signatures verify update packages. **Windows publisher signing is separate**: Preview installers may be unsigned, and each release should state its signing status. Never substitute a fabricated signature or unverified download URL.

## Local data and agent access

Chats, agent profiles and workspaces are managed locally. Choosing a cloud model sends task data to that provider; connected tools and MCP servers may also communicate with their own services. Optional account sign-in requires an online authentication service.

Native agents and tools run with your Windows account permissions. ControlT7 approvals coordinate shared actions; they are not an operating-system filesystem sandbox. Use trusted CLIs, projects and MCP servers, and give parallel agents clear responsibilities to reduce conflicting file edits.

## Feedback

**[Open an issue →](https://github.com/tanoydev607-maker/controlt7-releases/issues)**

For a useful bug report, include:

- ControlT7 version and Windows version.
- Agent CLI and model/provider involved, if relevant.
- Steps to reproduce, expected behavior and actual behavior.
- A screenshot or a short, sanitized log excerpt.

Remove API keys, passwords, tokens, private chats and personal files before posting. GitHub issues are public. If Issues is unavailable, use the contact method listed in the release notes.

## About this repository

This is the public distribution repository for **ControlT7**. Published releases may include installers, updater signatures, checksums, release notes and applicable third-party notices or component-source archives. The update website is deployed separately from the private application build pipeline.

Repository visibility does not grant an open-source license to the application. Refer to the application's terms and the licenses supplied for individual third-party components.

---

<div align="center">
  <p><strong>ControlT7 by Anew</strong><br />A workspace for the way you want to work with agents.</p>
</div>
