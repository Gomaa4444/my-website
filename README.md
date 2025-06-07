<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>QA Checklist</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f9f9f9;
      padding: 30px;
    }
    .container {
      max-width: 700px;
      margin: auto;
      background: white;
      padding: 25px;
      border-radius: 8px;
      box-shadow: 0 3px 10px rgba(0,0,0,0.1);
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

  <form onsubmit="submitChecklist(event)">

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

  <p id="thanks">Thank you! Your QA checklist was submitted (locally).</p>
</div>

<script>
  function submitChecklist(event) {
    event.preventDefault();
    document.getElementById('thanks').style.display = 'block';
  }
</script>

</body>
</html>
