<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>ED4 – Universal File Encryption Utility</title>
  <link href="https://fonts.googleapis.com/css2?family=JetBrains+Mono&display=swap" rel="stylesheet" />
  <style>
    body {
      margin: 0;
      font-family: 'JetBrains Mono', monospace;
      background: linear-gradient(to right, #0f2027, #203a43, #2c5364);
      color: #ffffff;
      animation: fadeIn 2s ease-in-out;
    }
    header {
      text-align: center;
      padding: 4rem 2rem 1rem;
      background: #121212cc;
    }
    h1 {
      font-size: 3rem;
      animation: glow 2s ease-in-out infinite alternate;
    }
    h2 {
      margin-top: 2rem;
      font-size: 2rem;
      color: #00ffff;
    }
    p, li {
      font-size: 1rem;
      line-height: 1.6;
    }
    .container {
      max-width: 1000px;
      margin: auto;
      padding: 2rem;
    }
    .features, .stack, .usage, .demo {
      background: rgba(255,255,255,0.05);
      margin: 2rem 0;
      padding: 2rem;
      border-radius: 10px;
      box-shadow: 0 0 20px rgba(0,255,255,0.1);
      backdrop-filter: blur(4px);
    }
    table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 1rem;
    }
    table, th, td {
      border: 1px solid #00ffff44;
    }
    th, td {
      padding: 0.75rem;
      text-align: left;
    }
    .glow-text {
      color: #00ffee;
      text-shadow: 0 0 5px #00ffeeaa, 0 0 10px #00ffeeaa;
    }
    .screenshot {
      width: 100%;
      border-radius: 12px;
      margin-top: 1rem;
      box-shadow: 0 0 25px #00ffff33;
    }
    @keyframes glow {
      from { text-shadow: 0 0 10px #0ff, 0 0 20px #0ff; }
      to { text-shadow: 0 0 20px #00ffff, 0 0 30px #00ffffaa; }
    }
    @keyframes fadeIn {
      0% { opacity: 0; transform: translateY(-20px); }
      100% { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body>
  <header>
    <h1>🔐 ED4 – Universal File Encryption Utility</h1>
    <p class="glow-text">Multi-layered Bash encryption, permission-aware, and beautifully terminal-native</p>
  </header>
  <div class="container">

    <section class="features">
      <h2>✨ Features</h2>
      <ul>
        <li>🔐 <strong>Four-Layer Encryption Stack</strong> — Unique, reversible Bash-based algorithms</li>
        <li>🧠 <strong>Permission-Based Keying</strong> — Chmod-derived entropy logic</li>
        <li>📝 <strong>Smart Logging</strong> — Timestamped `encdec.log` system</li>
        <li>📄 <strong>File Auto-Viewer</strong> — Handles both terminal & browser-based content</li>
        <li>💻 <strong>Zero External Dependencies</strong> — Only core utils: bash, awk, base64, xxd</li>
        <li>📦 <strong>Portable Output</strong> — Minimal `.enc` and `.dec` files</li>
      </ul>
    </section>

    <section class="stack">
      <h2>🔗 Encryption Stack</h2>
      <table>
        <thead>
          <tr><th>Layer</th><th>Name</th><th>Description</th></tr>
        </thead>
        <tbody>
          <tr><td>1️⃣</td><td>ASCII Byte Shift</td><td>Permission-based rotation of ASCII values</td></tr>
          <tr><td>2️⃣</td><td>Hex Reverse + Rotate</td><td>In-place hex string mangling</td></tr>
          <tr><td>3️⃣</td><td>NXR4 – Nibble Swap</td><td>Custom nibble reversal encryption</td></tr>
          <tr><td>4️⃣</td><td>Base64 + Block Shuffling</td><td>Final obfuscation via encode & reorder</td></tr>
        </tbody>
      </table>
    </section>

    <section class="usage">
      <h2>📦 Usage</h2>
      <pre><code>git clone https://github.com/likhil-pidugu/ED4.git
cd ED4
chmod +x ed4.sh
./ed4.sh</code></pre>
      <p><strong>Menu:</strong></p>
      <ul>
        <li>🔐 Encrypt File</li>
        <li>🔑 Decrypt File</li>
        <li>📄 View File</li>
        <li>🔍 View Logs</li>
        <li>❌ Exit</li>
      </ul>
    </section>

    <section class="demo">
      <h2>🧪 Live Demo (Terminal)</h2>
      <pre><code>$ ./ed4.sh
Choose option 1: 🔐 Encrypt
Enter file path: <em>secret.pdf</em>
✅ Output: secret.pdf.enc

Choose option 2: 🔑 Decrypt
Enter file path: <em>secret.pdf.enc</em>
✅ Output: secret.pdf.dec</code></pre>
      <img src="https://raw.githubusercontent.com/likhil-pidugu/ED4/main/screenshots/demo.png" alt="Live Demo Screenshot" class="screenshot" />
    </section>

    <section class="stack">
      <h2>📊 Real-Time Stats</h2>
      <img src="https://komarev.com/ghpvc/?username=likhil-pidugu&label=Visitors" />
      <img src="https://img.shields.io/tokei/lines/github/likhil-pidugu/ED4" />
      <img src="https://img.shields.io/github/languages/top/likhil-pidugu/ED4" />
    </section>

    <section class="features">
      <h2>🧠 Philosophy</h2>
      <p><em>"Encrypt not just bytes, but behaviors. ED4 evolves based on permissions, so every file is uniquely protected."</em></p>
      <p>— <strong>LIKHIL & CO</strong></p>
    </section>

    <section class="features">
      <h2>📜 License</h2>
      <p>Licensed under the <a href="LICENSE" style="color:#0ff;">MIT License</a>. Fork, contribute, or enhance freely.</p>
    </section>

    <section class="features">
      <h2>🙌 Credits</h2>
      <ul>
        <li>Developed with ❤️ by <strong>LIKHIL & CO</strong></li>
        <li>Readme animations inspired by modern AI UI/UX patterns</li>
      </ul>
    </section>

  </div>
</body>
</html>
