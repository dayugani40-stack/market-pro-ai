Market Pro V16 — Gemini AI backend integrated (Kannada / English / Both)

Frontend and backend are served from ONE origin. No manual backend URL needed once hosted.

DEPLOY ONLINE (Android-friendly):
1. Create a private GitHub repository with index.html, ai_server.py, render.yaml.
2. In Render, create a new Blueprint / Web Service from that repository.
3. Add secret environment variable GEMINI_API_KEY from Google AI Studio. Do NOT put it in index.html, screenshots or chat.
4. Deploy and open the Render HTTPS URL in Chrome.
5. AI status should show green; load market data, then tap Analyze with AI.
6. Choose Kannada / English / Both from language dropdown.

LOCAL TEST (Python):
GEMINI_API_KEY=YOUR_KEY python ai_server.py
Visit http://localhost:8765; check http://localhost:8765/api/health

NOTE: This ZIP contains functional connection code, NOT an already-deployed server. Live AI calls require your own API key, deployment and available Gemini quota.
Do not publish a service without authentication/rate limiting for public use; the demo server can otherwise incur API charges. AI is explanatory only and never changes fixed signals.
