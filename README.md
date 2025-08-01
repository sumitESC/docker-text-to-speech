<h1>🗣️ Docker Text-to-Speech (IBM Watson)</h1>

<p>
  A simple web app that converts user input text into speech using
  <a href="https://cloud.ibm.com/catalog/services/text-to-speech" target="_blank">IBM Watson Text-to-Speech API</a>.
  Built with HTML, JavaScript, Docker, and deployed using Render.
</p>

<p><strong>🔗 Live Demo:</strong> <a href="https://text-to-speech-latest.onrender.com" target="_blank">https://text-to-speech-latest.onrender.com</a></p>
<p><strong>📦 GitHub Repo:</strong> <code>docker-text-to-speech</code></p>

<h2>🚀 Features</h2>
<ul>
  <li>Multiple expressive, natural IBM voices</li>
  <li>Downloadable <code>.wav</code> audio output</li>
  <li>Simple UI powered by Docker container</li>
  <li>Deployed using <a href="https://render.com" target="_blank">Render</a></li>
</ul>

<h2>🧪 How It Works</h2>
<ol>
  <li>User types text and selects a voice</li>
  <li>Text is sent to IBM Watson Text-to-Speech API using Fetch and API Key</li>
  <li>The server responds with audio data</li>
  <li>Audio is played and can be downloaded as WAV</li>
</ol>

<h2>🔑 IBM API Setup</h2>
<ol>
  <li>Create an IBM Cloud account and enable <strong>Text to Speech</strong> service</li>
  <li>Follow IBM's guide: 
    <a href="https://cloud.ibm.com/docs/text-to-speech?topic=text-to-speech-gettingStarted#getting-started-tutorial" target="_blank">
      Getting Started with Text-to-Speech
    </a>
  </li>
  <li>Get your API key and service URL from the "Service credentials" section</li>
  <li>Update this line in your JavaScript:
    <pre><code>const apiKey = "your_api_key";
const apiUrl = "https://your-instance-url/v1/synthesize?voice=voiceName";</code></pre>
  </li>
</ol>

<h2>🐳 Docker Usage</h2>
<pre><code>git clone https://github.com/sumitESC/docker-text-to-speech
cd docker-text-to-speech
docker build -t docker-text-to-speech .
docker run -p 3000:3000 docker-text-to-speech</code></pre>

<h2>🔗 Live Demo</h2>
<p>
  Try the live demo here:<br>
  <a href="https://text-to-speech-latest.onrender.com" target="_blank">
    https://text-to-speech-latest.onrender.com
  </a>
</p>


<h2>📁 File Structure</h2>
<pre><code>.
├── index.html         # Frontend UI
├── Dockerfile         # Docker config
├── README.md          # Documentation
</code></pre>

<h2>🙌 Author</h2>
<p>Developed by <strong>Sumit Kushwaha</strong></p>
