<script>
    export let onClose;
  
    function closeComponent() {
      onClose();
    }
  </script>
  
  <section class="recruiting-automation-section">
    <div class="automation-component">
      <div class="hero-section">
        <h2 style="color: darkmagenta;">Recruiting Automation</h2>
        <p>Recruiting automation allows you to focus on the work that matters!</p>
      </div>
        <section class="testimonials-section">
          <table>
          <div class="container">
            <div class="row">
              <div class="col-md-4">
                <div class="feature-card">
                  <i class="fa fa-search"></i>
                  <h3 style="color:purple; font-weight:600;">Save time</h3>
                  <h6>Increase efficiency by creating workflows that automate repetitive and common tasks, save hours each week.</h6>
                </div>
              </div>
              <div class="col-md-4">
                <div class="feature-card">
                  <i class="fa fa-envelope"></i>
                  <h3 style="color:purple; font-weight:600;">Be in control</h3>
                  <h6>Ensure that recruiting standards are enforced automatically, and build a streamlined and an error proof workflow.</h6>
                </div>
              </div>
              <div class="col-md-4">
                <div class="feature-card">
                  <i class="fa fa-users"></i>
                  <h3 style="color:purple; font-weight:600;">Automate everything</h3>
                  <h6>Automate mundane tasks so your team can focus on delivering smooth experience at every step of the recruiting cycle.</h6>
                </div>
              </div>
            
          </div>
        </table>
        </section>
          <button class="close-button" on:click={closeComponent}>Close</button>
      </div>
      
  </section>
  
  <style>
   
   .hero-section {
    text-align: center;
    margin-bottom: 200px;
  }
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
  
