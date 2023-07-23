<div class="timeline">
  <div class="container">
    <div class="ball">
      <span />
    </div>
    <div class="text-box">
      <p>Graduated as an engineer</p>
      <span class="arrow" />
    </div>
  </div>
  <div class="container">
    <div class="ball right">
      <span />
    </div>
    <div class="text-box">
      <p>Started working at Microsoft as a technology consultant</p>
      <span class="arrow-right" />
    </div>
  </div>
  <div class="container">
    <div class="ball">
      <span />
    </div>
    <div class="text-box">
      <span class="arrow" />
      <p>Became part of the Windows Server team</p>
    </div>
  </div>
  <div class="container">
    <div class="ball right">
      <span />
    </div>
    <div class="text-box">
      <p>
        Became the technical leader for the Windows networking and active
        directory teams
      </p>
      <span class="arrow-right" />
    </div>
  </div>
  <div class="container">
    <div class="ball">
      <span />
    </div>
    <div class="text-box">
      <p>
        Arrived in France and became a fulltime husband and discovered my
        passion for code
      </p>
      <span class="arrow" />
    </div>
  </div>
</div>

<style>
  .timeline {
    position: relative;
    max-width: 845px;
    margin: 6.25rem auto;
    margin-bottom: 0;
  }
  .timeline::after {
    content: "";
    position: absolute;
    width: 0.25rem;
    height: 100%;
    background-color: white;
    top: 0;
    left: 50%;
    margin-left: -0.1875rem;
    z-index: -1;
  }

  .container {
    position: relative;
    padding: 10px 50px;
    width: 50%;
  }
  .container:nth-child(odd) {
    left: 0;
  }
  .container:nth-child(even) {
    left: 50%;
  }
  .ball {
    position: absolute;
    width: 1.25rem;
    height: 1.25rem;
    background-color: white;
    border-radius: 50%;
    right: -0.5625rem;
    top: 1.25rem;
    z-index: 10;
  }
  .ball span {
    position: absolute;
    width: 100%;
    height: 100%;
    background-color: inherit;
    border-radius: inherit;
    opacity: 0.8;
    animation: pulseAnimation 1s ease-out infinite;
  }
  @keyframes pulseAnimation {
    100% {
      opacity: 0;
      transform: scale(2);
    }
  }
  .ball.right {
    left: -0.6875rem;
  }
  .arrow {
    position: absolute;
    height: 0;
    width: 0;
    top: 0.625rem;
    z-index: 1;
    border-top: 0.9375rem solid transparent;
    border-bottom: 0.9375rem solid transparent;
    border-left: 0.9375rem solid white;
    right: -0.625rem;
  }
  .arrow-right {
    position: absolute;
    height: 0;
    width: 0;
    top: 0.625rem;
    z-index: 1;
    border-top: 0.9375rem solid transparent;
    border-bottom: 0.9375rem solid transparent;
    border-right: 0.9375rem solid white;
    left: -0.625rem;
  }
  .text-box {
    padding: 1.25rem 1.875rem;
    background-color: white;
    position: relative;
    border-radius: 0.375rem;
  }
  p {
    color: black;
    font-size: 1.375rem;
  }
</style>
