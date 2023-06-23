<script>
    export let onClose;
  
    function closeComponent() {
      onClose();
    }
  </script>
  
  <section class="Recruitly Pricing">
    <div class="automation-component">
        <h2>Recruitly Pricing</h2>
        <p>Pricing that allows you to scale on demand </p>
        <section class="testimonials-section">
        <section class="pricing-section">
          <div class="container">
            <div class="row">
              <div class="col-md-4">
                <div class="pricing-card">
                  <h3 class="plan-title">Solo</h3>
                  <div class="price">$35</div>
                  <div class="price-details">/user/month</div>
                 
                </div>
              </div>
              <div class="col-md-4">
                <div class="pricing-card">
                  <h3 class="plan-title">Startup</h3>
                  <div class="price">$50</div>
                  <div class="price-details">/user/month</div>
                
                </div>
              </div>
              <div class="col-md-4">
                <div class="pricing-card">
                  <h3 class="plan-title">Professional</h3>
                  <div class="price">$75</div>
                  <div class="price-details">/user/month</div>
                 
                </div>
              </div>
             
            </div>
          </div>
        </section>
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
  
