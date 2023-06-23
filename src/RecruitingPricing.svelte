<script>
    export let onClose;
  
    function closeComponent() {
      onClose();
    }
  </script>
  
  <section class="Recruitly Pricing">
    <div class="automation-component">
      <div class="hero-section">
        <h1 style="color:blue;">Recruitly Pricing</h1>
        <p>Pricing that allows you to scale on demand</p>
      </div>
      <section class="features-section">
        <table>
        <div class="container">
          <div class="row">
            <div class="col-md-4">
              <div class="feature-card">
                <i class="fa fa-search"></i>
                <h3 style="color:purple; font-weight:600;">solo</h3>
                <p>For independent recruiters</p>
                <h3 >$35</h3>
              </div>
            </div>
            <div class="col-md-4">
              <div class="feature-card">
                <i class="fa fa-envelope"></i>
                <h3 style="color:purple; font-weight:600;">Startup</h3>
                <p>For startup agencies</p>
                <h3 >$50</h3>
              </div>
            </div>
            <div class="col-md-4">
              <div class="feature-card">
                <i class="fa fa-users"></i>
                <h3 style="color:purple; font-weight:600;">Professional</h3>
                <p>For established teams</p>
                <h3 >$75</h3>
              </div>
            </div>
          </div>
        </div>
      </table>
      </section>
        
      
        
        
        
        
        
        
        
          <button class="close-button" on:click={closeComponent}>Close</button>
        
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
      background-color: purple;
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
  
