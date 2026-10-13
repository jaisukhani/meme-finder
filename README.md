MemeOrbit — local run instructions

1. Keep these files in the same folder:
   - findthatmeme_clone_fixed.html
   - server.py

2. Install Python 3.9+ if needed.

3. Open a terminal in that folder and run:
   python server.py

4. Open this address in your browser:
   http://127.0.0.1:8000

Important:
- Do not open the HTML file directly with file://; use the local address above.
- The server-side proxy avoids browser CORS restrictions.
- It still relies on the upstream meme index at https://findthatmeme.com/api/v1/search.
  If that service is offline, blocks server requests, or changes its API, live search
  cannot work until a working upstream API is configured.
- Image preview remains local to your browser and does not upload the image.
