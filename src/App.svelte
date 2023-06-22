{#if showPricingPopup}
  <div class="popup pricing-popup">
    <div class="popup-content">
      <button class="close-button" on:click={closePopup}>&times;</button>
      <div class="popup-section">
        <h3>Recruitly Pricing</h3>
        <div class="pricing-tier">
          <h4>Solo</h4>
          <p class="pricing-details">
            For independent recruiters<br />
            $35/user/month
          </p>
        </div>
        <div class="pricing-tier">
          <h4>Startup</h4>
          <p class="pricing-details">
            For startup agencies<br />
            $50/user/month
          </p>
        </div>
        <div class="pricing-tier">
          <h4>Professional</h4>
          <p class="pricing-details">
            For established teams<br />
            $75/user/month
          </p>
        </div>
        <div class="pricing-tier">
          <h4>Enterprise</h4>
          <p class="pricing-details">
            For large organizations<br />
            $100/user/month
          </p>
        </div>
      </div>
    </div>
  </div>
{/if}
