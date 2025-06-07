<QA Check List ✅>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>QA Checklist</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: url('https://images.unsplash.com/photo-1600585154340-be6161a56a0c?auto=format&fit=crop&w=1500&q=80') no-repeat center center fixed;
      background-size: cover;
      padding: 30px;
      margin: 0;
    }
    .container {
      max-width: 700px;
      margin: auto;
      background: rgba(255, 255, 255, 0.95); /* light white overlay */
      padding: 25px;
      border-radius: 10px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.2);
    }
    h1, h2 {
      color: #333;
    }
    label {
      display: block;
      margin: 8px 0;
      cursor: pointer;
    }
    button {
      margin-top: 20px;
      padding: 12px 20px;
      background: #007bff;
      border: none;
      color: white;
      font-size: 16px;
      border-radius: 6px;
      cursor: pointer;
    }
    button:hover {
      background: #0056b3;
    }
    #thanks {
      margin-top: 20px;
      color: green;
      font-weight: bold;
      display: none;
    }
  </style>
</head>
<body>

<div class="container">
  <h1>✅ QA Checklist</h1>

  <form id="qaForm" onsubmit="submitChecklist(event)">

    <h2>🔍 Opening & Verification</h2>
    <label><input type="checkbox" /> open the call &lt;10 seconds from receipt of interaction</label>
    <label><input type="checkbox" /> Confirms/updates CPC when not required (other user)</label>
    <label><input type="checkbox" /> Run STAT Tool</label>

    <h2>🎨 Call Handling</h2>
    <label><input type="checkbox" /> Confirms the reason customer is contacting us</label>
