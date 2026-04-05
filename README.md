# Sinhala Subtitle Translator

A simple, browser-based Sinhala subtitle translator that leverages the Google Gemini 2.5 Flash Lite API to translate English `.srt` subtitle files into Sinhala.

## Features

- **Direct Browser Execution:** No backend server required. Runs cleanly as a single HTML file.
- **Batch Processing:** Subtitles are automatically chunked into manageable batches (30, 50, or 80) to maximize Gemini AI translation efficiency and context accuracy.
- **Translation Styles:** Allows opting between "Spoken" (කතාකරන ප්‍රායෝගික සිංහල) and "Formal" (ලිඛිත සිංහල).
- **Beautiful UI:** Polished interface with film grain elements, scanlines, and an interactive status log.
- **Rate-Limit Aware:** Handled gracefully with built-in retries and 6s delays between batches for free Gemini API tiers.

## Usage

1. Obtain a **Gemini API Key** from [Google AI Studio](https://aistudio.google.com/).
2. Open the `index.html` file in any modern web browser.
3. Paste your Gemini API key in the designated input field.
4. Drag & Drop or select your English `.srt` file.
5. Choose your Preferred translation style and batch size.
6. Click **TRANSLATE** and monitor the log.
7. Once finished, click **DOWNLOAD SINHALA SRT**.

## Technologies

- HTML5 / CSS3 / Vanilla JavaScript
- Google Generative Language API (Gemini 2.5)
