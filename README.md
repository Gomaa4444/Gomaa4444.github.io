<QA Check List ✅>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>QA Checklist</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: url(![intelcia-oficinas](https://github.com/user-attachments/assets/cc736b34-44d0-4283-bceb-1b0ec31ade31)
) no-repeat center center fixed;
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
    <label><input type="checkbox" /> Provides assurance to help resolve the issue with confidence</label>
    <label><input type="checkbox" /> Actively listens to what the customer is saying</label>
    <label><input type="checkbox" /> Empathizes to the customer's situation</label>

    <h2>🌐 Call Control</h2>
    <label><input type="checkbox" /> Allow the customer to speak uninterrupted</label>
    <label><input type="checkbox" /> Avoids unnecessary hold and dead air</label>

    <h2>⚙️ Tool Utilization</h2>
    <label><input type="checkbox" /> Uses STAT properly and when required</label>
    <label><input type="checkbox" /> Pushes STAT data to Remedy</label>
    <label><input type="checkbox" /> Use IBA, AVA and light speed</label>

    <h2>📝 Closing</h2>
    <label><input type="checkbox" /> Asks customer if there's anything else they can help with</label>
    <label><input type="checkbox" /> Sets expectations for upcoming activities, when applicable (TC policy)</label>
    <label><input type="checkbox" /> Introduces customer satisfaction survey</label>
    <label><input type="checkbox" /> Self Help options</label>
    <label><input type="checkbox" /> Closes the call branding Optimum</label>

    <button type="submit">Submit</button>
  </form>

  <p id="thanks">Thank you! Your QA checklist was submitted.</p>
</div>

<script>
  function submitChecklist(event) {
    event.preventDefault();

    // Show thank you message
    document.getElementById('thanks').style.display = 'block';

    // Uncheck all checkboxes
    const checkboxes = document.querySelectorAll('#qaForm input[type="checkbox"]');
    checkboxes.forEach(checkbox => {
      checkbox.checked = false;
    });
  }
</script>

</body>
</html>
