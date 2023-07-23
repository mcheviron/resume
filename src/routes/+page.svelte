<script>
  import home from "$lib/assets/home.jpg";
</script>


<div class="wrapper">
  <div class="left-col">
    <h1>Technophile, engineer, developer.</h1>
    <a href="/about"><div class="about">About me</div></a>
    <a href="/skills"><div class="skills">Skills</div></a>
  </div>
  <div class="right-col">
    <img src={home} alt="monitors with code" />
  </div>
</div>

<style>
  .wrapper {
    display: flex;
    gap: 15.3125rem;
  }
  .left-col {
    display: flex;
    flex-direction: column;
    padding-left: 1.875rem;
  }
  h1 {
    font-size: 2.5rem;
    font-weight: normal;
    margin-bottom: 8.125rem;
    width: 22.5rem;
  }
  a {
    text-decoration: none;
    color: inherit;
    width: 10.9375rem;
    margin-bottom: 1.875rem;
    height: 4.6875rem;
  }
  .about {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    background-color: white;
    color: black;
    border-radius: 3.125rem;
    padding: 1.625rem 3rem;
    font-size: 1.125rem;
    cursor: pointer;
  }
  .about:hover {
    font-weight: bold;
  }
  .skills {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    background-color: #1f2028;
    border: 2px solid #9e9e9e;
    border-radius: 3.125rem;
    padding: 1.625rem 3rem;
    width: 10.9375rem;
    height: 4.6875rem;
    font-size: 1.125rem;
    cursor: pointer;
    transition: 0.3s;
  }

  .skills:hover {
    border: 2px solid #1f2028;
  }

  .left-col {
    width: 50%;
  }

  img {
    object-fit: cover;
    height: 37.5rem;
    width: 100%;
    border-radius: 0.3125rem;
    transition: 0.3s;
    transform: scale(1);
  }
  img:hover {
    transform: scale(1.05);
  }
</style>
