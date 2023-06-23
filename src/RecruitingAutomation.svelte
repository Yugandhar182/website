<script>
    export let onClose;
  
    function closeComponent() {
      onClose();
    }
  </script>
  
  <section class="recruiting-automation-section">
    <div class="automation-component">
        <h2>Recruiting Automation</h2>
        <p>Recruiting automation allows you to focus on the work that matters!</p>
        <p>Automation can be key to recruiting efficiency, but only if done right. It takes time and effort to create the right workflow that is optimal for your business. Our intuitive automation platform allows you to configure the triggers, actions and amend them when necessary with ease.</p>
        <ul>
          <li>Save time</li>
          <li>Increase efficiency by creating workflows that automate repetitive and common tasks, save hours each week.</li>
          <li>Be in control</li>
          <li>Ensure that recruiting standards are enforced automatically, and build a streamlined and an error-proof workflow.</li>
          <li>Automate everything</li>
          <li>Automate mundane tasks so your team can focus on delivering a smooth experience at every step of the recruiting cycle.</li>
          <button class="close-button" on:click={closeComponent}>Close</button>
        </ul>
      </div>
      
  </section>
  
  <style>
   
  
    .recruiting-automation-section h1 {
      color: blue;
      font-weight: bold;
      font-size: 2rem;
    }
  
   
    .close-button {
      margin-top: 20px;
      padding: 10px 20px;
      background-color: red;
      color: white;
      border: none;
      border-radius: 5px;
      font-size: 16px;
      cursor: pointer;
    }
    body {
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
    }

    .automation-component {
      width: 100%;
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      background-color: #f0f0f0;
      padding: 20px;
    }

    

    .automation-component p {
      font-size: 18px;
      margin-bottom: 10px;
    }

    .automation-component ul {
      list-style-type: disc;
      margin-left: 20px;
    }

    .automation-component li {
      font-size: 16px;
      margin-bottom: 5px;
    }
  </style>
  
