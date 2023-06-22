<!-- src/App.svelte -->
<script>
  import { createEventDispatcher } from 'svelte';
  import 'bootstrap/dist/css/bootstrap.min.css';

  const dispatch = createEventDispatcher();
  let showWhyRecruitlyPopup = false;
  let showPricingPopup = false;
  let showOverviewPopup = false;
  function openWhyRecruitlyPopup() {
    showWhyRecruitlyPopup = true;
  }

  function openPricingPopup() {
    showPricingPopup = true;
  }

  function closePopup() {
    showWhyRecruitlyPopup = false;
    showPricingPopup = false;
    showOverviewPopup = false;
  }
  function openOverview() {
    // Add your code here to handle the button click event
    // For example, you can redirect to an overview page or show the overview content
    showOverviewPopup = true;
  }

  
 
</script>

<main>
  <div class="container">
    <h1 class="display-4" style="color:blue;font-weight: 700;" >
      Recruitment CRM System
    </h1>
    
    <p class="card-text">Recruitly® is built to streamline agency recruitment processes and help businesses grow as a result.</p>
  </div>
  <button class="overview-button" on:click={openOverview} >Overview</button>
   </main>

<div class="information">
  <p on:click={openWhyRecruitlyPopup} style="color:blue;">Why Recruitly</p>
  <p style="color:blue;">Automation</p>
  <p on:click={openPricingPopup} style="color:blue;">Pricing</p>
</div>

{#if showWhyRecruitlyPopup}
  <div class="popup" on:click={closePopup}>
    <div class="popup-content">
      <button class="close-button" on:click={closePopup}>&times;</button>
      <div class="popup-section">
        <h3>Email Marketing</h3>
        <p class="custom-paragraph">Engage talent at the right time, promote your business to the right audience.</p>
      </div>
      <div class="popup-section">
        <h3>Applicant Tracking System</h3>
        <p class="custom-paragraph">Candidate sharing, boolean searches, interview scheduling, automation and more.</p>
      </div>
      <div class="popup-section">
        <h3>Website Integration</h3>
        <p class="custom-paragraph">Turn your WordPress website into a fully featured job-board using our FREE plugins.</p>
      </div>
      <div class="popup-section">
        <h3>Job Distribution</h3>
        <p class="custom-paragraph">Get your job in front of millions of candidates, manage applicants in one place.</p>
      </div>
      <div class="popup-section">
        <h3>Search & Import</h3>
        <p class="custom-paragraph">Search and import candidates from CV-Library and TotalJobs with just a few clicks.</p>
      </div>
      <div class="popup-section">
        <h3>Recruiting Automation</h3>
        <p class="custom-paragraph">Boost your team's productivity by creating workflows that automate repetitive and common tasks.</p>
      </div>
   </div>
    </div>
    {/if}
    {#if showPricingPopup}
  <div class="popup">
    <div class="popup-content">
      <button class="close-button" on:click={closePopup}>&times;</button>
      <div class="popup-section">
        <h3>Recruitly Pricing</h3>
        <p class="custom-paragraph">Pricing that allows you to scale on demand.</p>
      </div>
    </div>
  </div>
  
{/if}
{#if showOverviewPopup}
  <div class="popup" on:click={closePopup}>
    <div class="popup-content">
      <button class="close-button" on:click={closePopup}>&times;</button>
      <div class="popup-video-section">
        <iframe class="popup-video" src="https://www.youtube.com/embed/9L0fVJb7zSk" frameborder="0" allowfullscreen></iframe>
      </div>
    </div>
  </div>
{/if}
    


<style>
  /* Add custom styles for your opening page here */
  .container {
    text-align: center;
    margin-top: 200px;
  }
  h1.display-4 {
    font-size: 3.5rem;
    margin-bottom: 0.5rem;
    font-stretch: expanded;
  }
  .font-weight-bold {
    font-weight: bold;
  }

  .header {
    background-color: #f8f9fa;
    padding: 20px;
    text-align: center;
  }

  .information {
    position: absolute;
    top: 50px;
    right: 270px;
    display: flex;
    flex-direction: row;
    align-items: center;
  }

  .information p {
    margin: 0;
    margin-left: 10px;
    cursor: pointer;
  }

  .popup {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.5);
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .popup-content {
    position: relative; /* Added position relative */
    background-color: #fff;
    padding: 20px;
    text-align: center;
    border-radius: 5px;
    width: 80%; /* Increased the width */
    height: 80%; /* Increased the height */
    max-width: 800px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    overflow-y: auto;
  }

  .popup-section {
    width: calc(50% - 20px); /* Divide the width equally among two sections */
    height: 25%; /* Divide the height equally among four sections */
    padding: 10px;
  }

  .custom-paragraph {
    text-align: center; /* Center the paragraph horizontally */
  }

  .popup-content h3 {
    text-align: center;
    color: blue;
  }

  .popup-content p.custom-paragraph {
    width: 100%; /* Set the width for the paragraphs */
    text-align: center; /* Center the paragraph text */
  }

  body {
    background-color: #e2f3fc;
  }
  .close-button {
    position: absolute;
    top: 0px;
    right: 1px;
    font-size: 24px;
    color: #f00f22;
    background: transparent;
    border: none;
    cursor: pointer;
  }
  .overview-button {
    margin-top: 10px;
    padding: 10px 20px;
    background-color: yellow;
    color: black;
    border: none;
    border-radius: 5px;
    font-size: 16px;
    cursor: pointer;
    display: flex;
    align-items: center;
  }
  .popup-video-section {
    width: 100%;
    text-align: center;
  }

  .popup-video {
    width: 100%;
    height: 400px;
  }
</style>
