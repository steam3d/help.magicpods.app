# Poor sound and microphone quality

!!! note
    TL;DR All Bluetooth headphones have poor sound and microphone quality and there's no fixing it

Bluetooth devices, including headphones, operate according to specific Bluetooth profiles. These profiles define the functionality of the device. Examples of profiles include A2DP (stereo audio), Fax Profile, File Transfer Profile, and HandsFree Profile. Each profile has standard specifications.

For voice communication, the HandsFree Profile is used. It has mono sound and mono recording for the microphone with a base frequency of 8 kHz. Some Bluetooth drivers allow you to increase the frequency to 16 kHz, but the audio and microphone are still mono. (for comparison, in music files the frequency is usually 44.1 kHz)

No matter what Bluetooth headphones you have, the voice quality will be poor. This is because the HandsFree Profile specification determines the quality.

When you use Bluetooth headphones in Windows, the headphones switch from A2DP (stereo audio) to HandsFree profile as soon as you use the headphone microphone. If you have game voice chat, audio recording, or are talking on Discord, Skype, Teams, Steam, etc., Windows will switch your headphones to HandsFree mode.

To prevent this, change the microphone in the settings of each application or assign a different default microphone in Windows settings. You can also disable the HandsFree profile, so the headphone microphone is no longer available. To do this, open MagicPods on the headphones page. Select the headphones you want and enable the `Auto disable HandsFree` option.