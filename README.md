# azure-tts
a simple bash script to use Azure Text-to-Speech

Before starting using the script, you need to create Azure Text-to-Speech service on Azure Portal. The voice "en-US-JessaNeural" is set by default, so you need to configure the service with 'Standard' (S0) Pricing Tier to enable nural voice.

After creating the instance of Azure TTS, you could find the apiKey on Azure Portal. Put it into the script as follows.

apiKey="b0e9cb8eb92744018b7d1852622c2b84"
