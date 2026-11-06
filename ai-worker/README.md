# AI Shree helper (Cloudflare Worker + Gemini)

This small free service lets AI Shree answer any question with a real AI.
It keeps your Gemini API key secret, so the key is never put in the website.

1. Get a free key at https://aistudio.google.com/apikey (Create API key).
2. Create a free account at https://dash.cloudflare.com , open Workers & Pages, Create, Create Worker, name it `ai-shree`, Deploy.
3. Click Edit code, delete everything, paste all of `worker.js`, and Deploy.
4. Open the Worker, Settings, Variables and Secrets, Add: type Secret, name `GEMINI_API_KEY`, value = your key. Deploy.
5. Copy the Worker address (it looks like https://ai-shree.YOURNAME.workers.dev) and give it to Claude, or put it in `index.html` as `AI_URL`.
