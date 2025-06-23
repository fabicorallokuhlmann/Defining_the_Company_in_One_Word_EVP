 <h1>🌟 Word Cloud - Defining the Company in One Word</h1>

  <p>
    This project analyzes feedback from a spreadsheet where employees define the company using a single, most remarkable word.
    It processes and cleans the text, identifies the most frequent terms, translates them into English, and generates a visual <strong>word cloud</strong>.
  </p>

  <hr>

  <h2>📌 Purpose</h2>
  <p>
    To visually highlight the most recurring words that employees associate with the company, helping with qualitative analysis related to organizational culture and perception.
  </p>

  <hr>

  <h2>🗂️ Project Structure</h2>
  <pre>
📁 wordcloud-company
├── wordcloud_company.ipynb
├── company_feedback.xlsx
└── README.md
  </pre>

  <hr>

  <h2>⚙️ Requirements</h2>
  <p>Python version 3.7 or above and the following libraries:</p>
  <ul>
    <li><code>pandas</code></li>
    <li><code>nltk</code></li>
    <li><code>matplotlib</code></li>
    <li><code>wordcloud</code></li>
    <li><code>googletrans==4.0.0-rc1</code></li>
    <li><code>deep-translator</code></li>
  </ul>

  <h3>Install Dependencies</h3>
  <pre><code>pip install googletrans==4.0.0-rc1 deep-translator nltk pandas matplotlib wordcloud</code></pre>

  <h3>NLTK Resources</h3>
  <p>The following resources will be downloaded automatically:</p>
  <pre><code>
nltk.download('punkt')
nltk.download('stopwords')
  </code></pre>

  <hr>

  <h2>📁 Input File</h2>
  <p>The script expects an <strong>.xlsx</strong> file with:</p>
  <ul>
    <li>A sheet named <code>Planilha1</code></li>
    <li>A column labeled <code>Comentário</code> containing the textual feedback</li>
  </ul>
  <p>Make sure to update the file path in the code:</p>
  <pre><code>file_path = 'C:\\Users\\YourUsername\\Downloads\\company_feedback.xlsx'</code></pre>

  <hr>

  <h2>🔍 Workflow</h2>
  <ol>
    <li>Loads the spreadsheet and extracts the <code>Comentário</code> column.</li>
    <li>Processes the text: lowercasing, tokenizing, and removing stopwords and generic terms.</li>
    <li>Counts the most frequent words and displays the top 5.</li>
    <li>Translates all relevant words to English using <code>googletrans</code>, with fallback to <code>deep-translator</code>.</li>
    <li>Generates and displays a translated word cloud.</li>
  </ol>

  <hr>

  <h2>🖼️ Output</h2>
  <p>
    The script will print the top 5 most frequent words with their frequency count and render a colorful word cloud in English using <code>matplotlib</code>.
  </p>

  <hr>

  <h2>🔧 Customization Tips</h2>
  <ul>
    <li>Edit the <code>custom_exclusions</code> list to ignore company-specific or frequent irrelevant words.</li>
    <li>Change the translation target language by replacing <code>target='en'</code> with any supported language code.</li>
    <li>Adjust the color scheme of the word cloud using the <code>colormap</code> parameter (e.g., <code>plasma</code>, <code>cool</code>, <code>inferno</code>).</li>
  </ul>

  <hr>

  <h2>👩‍💻 Author</h2>
  <p><strong>Fabiana Corallo Mello de Azevedo Kuhlmann</strong></p>

  <hr>

  <h2>📄 License</h2>
  <p>This project is licensed under the <strong>MIT License</strong>. You are free to use, modify, and share it with appropriate credit.</p>

</body>
</html>
