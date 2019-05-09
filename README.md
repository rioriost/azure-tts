# azure-tts
A simple bash script to use Azure Text-to-Speech on macOS

Before starting using the script, you need to create Azure Text-to-Speech service on Azure Portal. The voice "en-US-JessaNeural" is set by default, so you need to configure the service with 'Standard' (S0) Pricing Tier to enable neural voice.

After creating the instance of Azure TTS, you could find the apiKey on Azure Portal. Put it into the script as follows.

apiKey="b0e9cb8eb92744018b7d1852622c2b84"
(This key is just a sample.)

How to enable the script as a service.

1. Double Click the Azure-TTS.workflow to install it under ~/Library/Services/
2. Create a directory, "bin" under your home directory. e.g. mkdir ~/bin/
3. Put azure-tts under ~/bin/
4. Add permission to execute. e.g. chmod 755 ~/bin/azure-tts

After enabling the service, you can call it from any apps on macOS with contextual menu.

If you get the message related to accessibility settings, try tccutil to reset the permissions.

$ tccutil reset Accessibility
