# Movie Subtitle Character Attribution

A web-based tool that automatically attributes character names to lines in a movie SRT subtitle file using the OpenAI API. Ideal for enhancing subtitles with speaker information!

## Features

- Upload SRT subtitle files from your computer
- Uses OpenAI's GPT models to attribute each subtitle line to a likely speaker
- Progress bar and interactive feedback
- Downloadable enriched subtitles
- Clean, Star Wars-inspired design (but works for any movie)

## Usage

1. **Get an OpenAI API Key**

   Sign up at [OpenAI](https://platform.openai.com/signup) and generate an API key under your account settings.

2. **Open `index.html` in Your Browser**

   Simply double-click the file or open it in any modern browser.

3. **Process Subtitles**

   - Enter your OpenAI API key (it is only used in your browser, never sent or stored elsewhere).
   - Enter the movie title, or keep the default "Star Wars: A New Hope".
   - Upload your `.srt` subtitle file.
   - Click **Process Subtitles**. The tool will send subtitle lines (one at a time) to the OpenAI API, guessing who speaks each.
   - Wait for processing (it takes a few seconds per line due to API and rate limits).
   - Download the result as a text file with speakers prepended!

## Security & Privacy

- Your API key is never stored or transmitted outside of your browser session.
- All processing happens client-side (in your browser).
- Subtitle files are never uploaded to any server.

## Technical Details

- Built as a single-page app (`index.html` with inline JavaScript and CSS)
- Uses [OpenAI GPT-3.5-turbo](https://platform.openai.com/docs/models/gpt-3-5) chat API
- Performs basic SRT parsing in JavaScript
- All processing and API calls are rate-limited for safety

## Example Output
Luke: I want to learn the ways of the Force and become a Jedi like my father. Han Solo: Hokey religions and ancient weapons are no match for a good blaster at your side, kid. Leia: Aren't you a little short for a stormtrooper?

## Troubleshooting

- Make sure your API key is correct and has an active billing plan.
- Large SRT files may take a long time or hit OpenAI rate limits.
- You can refresh or reopen the page to restart.

## License

MIT License

---

Created for movie subtitle processing. May the Force be with you!