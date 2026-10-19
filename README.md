# Podcast Producer

A one-page app that turns a raw two-mic podcast recording into an upload-ready episode for Spotify for Creators.

**Everything runs in your browser.** Your audio is never uploaded anywhere.

## What it does

1. **Reads your AIFF**, including 16/24-bit, 48 kHz stereo files of an hour or more. WAV, MP3 and M4A also work.
2. **Reduces room echo** on the channel of your choice (for example, a guest calling in over FaceTime).
3. **Levels each channel separately**, so both speakers end up equally loud, and turns down background noise and mic bleed between speech.
4. **Mixes to mono** and trims silence from the start and end.
5. **Adds your intro and outro music.** The music dips under your first and last few words.
6. **Exports a mono MP3** at −16 LUFS (podcast standard), with peaks limited to −1.5 dBFS, at 96 kbps by default.

## How to use it

- **Online:** open the GitHub Pages link for this repository.
- **Offline copy:** download `Podcast Producer.html` and double-click it.

Chrome is recommended. Drop in your episode, intro and outro, then click **Produce episode**.

Your intro, outro and settings are remembered between visits, in your own browser only.

## Built with

- Plain HTML and JavaScript, with no build step.
- [lamejs](https://github.com/zhuker/lamejs) for MP3 encoding.
- Audio processing (levelling, de-reverb, limiting) written from scratch. Loudness is measured to ITU-R BS.1770.

---

# Sun Finder

`sun-finder.html` finds the closest place in mainland UK (England, Scotland and Wales) where the sun is out today.

1. Click **Use my location**, or type a town or postcode.
2. It checks the live forecast every mile or so around you, up to 5, 10, 15, 25 or 50 miles away. Points at sea, on the islands or in Northern Ireland are skipped.
3. It shows the nearest sunny spot, with distance, direction, cloud cover, hours of sun left, temperature in °C and sunset time, plus a map and a **Get directions** link.

Choose **Right now** (clear sky at this moment) or **Rest of today** (mostly sunny until sunset).

If nowhere nearby is sunny, it tells you when the sun is next expected (later today or tomorrow), where it arrives first, and when it reaches you.

Weather comes from [Open-Meteo](https://open-meteo.com/) and place names from [BigDataCloud](https://www.bigdatacloud.com/); neither needs an API key. Open it from the GitHub Pages link (`…/sun-finder.html`) so your browser lets it ask for your location.
