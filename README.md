# azure-tts
A simple bash script to use Azure Text-to-Speech on macOS

Before starting using the script, you need to create Azure Text-to-Speech service on Azure Portal. The voice "en-US-JessaNeural" is set by default, so you need to configure the service with 'Standard' (S0) Pricing Tier to enable neural voice. Also, you need to install Azure CLI. e.g. brew install azure-cli

How to enable the script as a service.

1. Double Click the Azure-TTS.workflow to install it under ~/Library/Services/
2. Create a directory, "bin" under your home directory. e.g. mkdir ~/bin/
3. Put azure-tts under ~/bin/
4. Add permission to execute. e.g. chmod 755 ~/bin/azure-tts

After enabling the service, you can call it from any apps on macOS with the contextual menu.

If you get the message related to accessibility settings, try tccutil to reset the permissions.

$ tccutil reset Accessibility
