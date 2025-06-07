<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>QA Checklist</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: url('https://www.rrhhdigital.com/wp-content/uploads/2024/05/intelcia-oficinas.jpg') no-repeat center center fixed;
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
    <label><input type="checkbox" /> Confirms call back number in case of lost call​</label>
    <label><input type="checkbox" /> Run STAT Tool</label>

    <h2>🎨 Call Handling</h2>
    <label><input type="checkbox" /> Confirms the reason customer is contacting us</label>
    <label><input type="checkbox" /> Provides assurance to help resolve the issue with confidence</label>
    <label><input type="checkbox" /> Actively listens to what the customer is saying</label>
    <label><input type="checkbox" /> Empathizes to the customer's situation</label>

    <h2>🌐 Call Control</h2>
    <label><input type="checkbox" /> Allow the customer to speak uninterrupted</label>
    <label><input type="checkbox" /> Avoids unnecessary hold and dead air</label>
    <label><input type="checkbox" /> Self Help options</label>

    <h2>⚙️ Tool Utilization</h2>
    <label><input type="checkbox" /> Uses STAT properly and when required</label>
    <label><input type="checkbox" /> Pushes STAT data to Remedy</label>
    <label><input type="checkbox" /> Use IBA, AVA,VAT and light speed</label>

    <h2>📝 Setting expectations</h2>
    <label><input type="checkbox" /> Sets expectations for upcoming activities, when applicable[TC Visit: You can cancel, or reschedule a technician appointment on our website.]</label>
    <label><input type="checkbox" /> Setting the customer's expectations about the balance on the account and the due date for any billing inquiry.</label>
    <label><input type="checkbox" /> Advising the customer with SLA for the Direct ship and the Self help option</label>
    
    <h2>📝 Closing</h2>
    <label><input type="checkbox" /> Asks customer if there's anything else they can help with</label>
    <label><input type="checkbox" /> Sets expectations for upcoming activities, when applicable</label>
    <label><input type="checkbox" /> Upsell (Mobile-Fiber)</label>
    <label><input type="checkbox" /> Introduces customer satisfaction survey</label>
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
```
