# Seeduplex Web Demo - HTTPS deployment

This package is prepared for a Render Web Service. The included Dockerfile binds the Python server to 0.0.0.0 and uses Render's PORT environment variable.

## Deploy
1. Put these files into a GitHub repository.
2. In Render, create New -> Web Service and connect the repository.
3. Choose Docker as the runtime. Render can build the included Dockerfile.
4. Use the Free plan for a temporary test.
5. Deploy. Render gives the service an `https://...onrender.com` URL.
6. Open that URL on the phone, allow microphone permission, enter your Volcengine X-Api-Key, and start the call.

Do not hard-code your API key into the repository. The demo's page is designed to let you type the API key into the browser.

The app uses the backend to connect to the Volcengine realtime endpoint, so it should be deployed as a Web Service, not a Static Site.
