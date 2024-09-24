<template>
  <div class="about">
    <h2 class="heading">Experience</h2>
        <div id="experience-timeline">
            <div data-date="September 2015 – September 2016">
                <h3>Employer Name</h3>
                <h4>Job Title</h4>
                <p>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur in iaculis ex. Etiam volutpat laoreet urna. Morbi ut tortor nec nulla commodo malesuada sit amet vel lacus. Fusce eget efficitur libero. Morbi dapibus porta quam laoreet placerat.
                </p>
            </div>

            <div data-date="September 2015 – September 2016">
                <h3>Employer Name</h3>
                <h4>Job Title</h4>
                <p>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur in iaculis ex. Etiam volutpat laoreet urna. Morbi ut tortor nec nulla commodo malesuada sit amet vel lacus. Fusce eget efficitur libero. Morbi dapibus porta quam laoreet placerat.
                </p>
            </div>

            <div data-date="September 2015 – September 2016">
                <h3>Employer Name</h3>
                <h4>Job Title</h4>
                <p>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur in iaculis ex. Etiam volutpat laoreet urna. Morbi ut tortor nec nulla commodo malesuada sit amet vel lacus. Fusce eget efficitur libero. Morbi dapibus porta quam laoreet placerat.
                </p>
            </div>
        </div>
  </div>
</template>

<style scoped>
  h2 {
    margin-bottom: 15px;
  }

  p {
    margin-bottom: 15px;
  }

  ul {
    margin-bottom: 15px;
  }

  .images {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 10px;
  }

  .images img:nth-child(2) {
    margin-top: 150px;
  }

  .images img:nth-child(3) {
    margin-top: -150px;
  }

  .images img:hover {
    transform: scale(1.1);
    box-shadow: 0px 4px 20px rgba(255, 255, 255, 0.5);
  }

  img {
    width: 300px;
    height: 250px;
    object-fit: cover;
    
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    margin-bottom: 10px;
  }

  .container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 10px;
    margin-top: 15px;
  }

  .about {
    display: flex;
    flex-direction: column;
    gap: 16px;
    transition: background-image 0.5s ease-in-out;
    background-size: cover;
    background-position: center;
    min-height: 100vh;
    padding: 20px;
  }

  @media (min-width: 1024px) {
    .about {
      min-height: 100vh;
      display: flex;
      align-items: center;
    }
  }
</style>
