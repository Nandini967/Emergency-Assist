<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Emergency Assist</title>
</head>
<body>
    <h1>Emergency Assist</h1>
    <p><strong>Emergency Assist</strong> is a Python-based program that leverages the <strong>Telegram API</strong> to send SOS messages, including voice-to-text transcription and location sharing, to a specified Telegram contact. This system is designed to provide quick assistance by capturing audio, converting it into text, and sharing the user's location via IP-based geolocation.</p>
    
    <h2>Features</h2>
    <ul>
        <li><strong>Voice to Text Conversion:</strong> Captures audio input from the user and transcribes it into text using Google Speech Recognition.</li>
        <li><strong>Location Sharing:</strong> Fetches the current location using IP-based geolocation and sends it to a Telegram contact.</li>
        <li><strong>Audio File Generation:</strong> Saves the captured audio as a <code>.mp3</code> file and sends it to the recipient.</li>
        <li><strong>Telegram Integration:</strong> Automates the sending of text and location messages to a predefined user.</li>
        <li><strong>Ease of Use:</strong> Requires minimal input, ensuring swift action during emergencies.</li>
    </ul>
    
    <h2>Requirements</h2>
    <h3>Libraries</h3>
    <ul>
        <li><a href="https://pypi.org/project/Telethon/" target="_blank">Telethon</a>: For interacting with the Telegram API.</li>
        <li><a href="https://pypi.org/project/SpeechRecognition/" target="_blank">SpeechRecognition</a>: For audio input and transcription.</li>
        <li><a href="https://pypi.org/project/geocoder/" target="_blank">Geocoder</a>: For IP-based geolocation.</li>
    </ul>
    
    <h3>Python Version</h3>
    <p>Python 3.7 or later</p>
    
    <h3>Environment Variables</h3>
    <ul>
        <li><code>api_id</code>: Your Telegram API ID from <a href="https://my.telegram.org" target="_blank">my.telegram.org</a>.</li>
        <li><code>api_hash</code>: Your Telegram API hash from <a href="https://my.telegram.org" target="_blank">my.telegram.org</a>.</li>
        <li><code>phone</code>: Your registered phone number on Telegram.</li>
        <li><code>username</code>: The Telegram username of the recipient.</li>
    </ul>
    
    <h2>Installation</h2>
    <ol>
        <li>Clone the repository:
            <pre><code>git clone https://github.com/&lt;your-username&gt;/Emergency-Assist.git
cd Emergency-Assist</code></pre>
        </li>
        <li>Install the required dependencies:
            <pre><code>pip install -r requirements.txt</code></pre>
        </li>
        <li>Replace placeholder values in the code (<code>api_id</code>, <code>api_hash</code>, <code>phone</code>, <code>username</code>) with your Telegram API credentials and recipient username.</li>
        <li>Run the script:
            <pre><code>python main.py</code></pre>
        </li>
    </ol>
    
    <h2>How It Works</h2>
    <ol>
        <li>The program listens for audio input through the microphone.</li>
        <li>Converts the captured audio into text using Google Speech Recognition.</li>
        <li>Saves the audio locally as an MP3 file and sends it to the Telegram user.</li>
        <li>Retrieves the current location (latitude and longitude) using IP-based geolocation.</li>
        <li>Sends both the location and text message to the predefined Telegram contact.</li>
    </ol>
    
    <h2>Files in the Project</h2>
    <ul>
        <li><code>main.py</code>: Main script that implements the Emergency Assist functionality.</li>
        <li><code>requirements.txt</code>: List of dependencies required to run the project.</li>
    </ul>
    
    <h2>Example Use Case</h2>
    <ol>
        <li>The user initiates the script.</li>
        <li>The program records the user saying something like, "Please help, I need assistance."</li>
        <li>The recorded audio is transcribed into text and sent to the specified Telegram user.</li>
        <li>The user's approximate location (based on IP) is also sent as a live location message.</li>
    </ol>
    
    <h2>Limitations</h2>
    <ul>
        <li><strong>IP-based Location:</strong> Location accuracy depends on IP geolocation, which may not be precise compared to GPS-based methods.</li>
        <li><strong>Speech Recognition:</strong> Performance depends on the clarity of audio and ambient noise.</li>
    </ul>
    
    <h2>Future Improvements</h2>
    <ul>
        <li>Add GPS-based location sharing for more accurate location data.</li>
        <li>Enable multi-language support for speech recognition.</li>
        <li>Include an option to save chat logs for record-keeping.</li>
    </ul>
    
    <h2>License</h2>
    <p>This project is licensed under the MIT License. See the <code>LICENSE</code> file for details.</p>
    
    <h2>Contribution</h2>
    <p>Feel free to fork this repository, make your changes, and submit a pull request. For major changes, please open an issue first to discuss what you would like to change.</p>
</body>
</html>
