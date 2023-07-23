<script>
  import knowledge from "$lib/assets/about.jpg";
  import Timeline from "$lib/components/Timeline.svelte";
</script>

<div class="wrapper">
  <div class="left-col">
    <h1>
      Hi, I'm Mostafa Elataby-Cheviron, I'm a software engineer and a fullstack
      developer. I love technology in all its forms and the general sciences. I
      don’t care if it’s OS internals or UI/UX design.
    </h1>
    <h2>Knowledge shouldn’t have gate keepers.</h2>
    <div class="scroll-down">
      <div class="button">
        <svg
          width="21"
          height="24"
          viewBox="0 0 21 24"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M0.295607 14.33L9.95561 23.94L19.6156 14.33C19.7296 14.2432 19.8236 14.1329 19.8912 14.0067C19.9589 13.8804 19.9986 13.7411 20.0077 13.5981C20.0169 13.4551 19.9952 13.3119 19.9441 13.178C19.893 13.0442 19.8138 12.9228 19.7118 12.8223C19.6098 12.7217 19.4873 12.6442 19.3528 12.5951C19.2182 12.5459 19.0747 12.5263 18.9318 12.5375C18.789 12.5486 18.6503 12.5903 18.525 12.6598C18.3997 12.7292 18.2908 12.8248 18.2056 12.94L10.9556 20.13L10.9556 1C10.9556 0.734785 10.8503 0.480433 10.6627 0.292896C10.4752 0.10536 10.2208 1.90735e-06 9.95561 1.90735e-06C9.69039 1.90735e-06 9.43604 0.10536 9.2485 0.292896C9.06096 0.480433 8.95561 0.734785 8.95561 1L8.95561 20.13L1.70561 12.94C1.5173 12.753 1.26243 12.6485 0.99707 12.6494C0.731707 12.6504 0.477583 12.7567 0.290606 12.945C0.103628 13.1333 -0.000888824 13.3882 4.95911e-05 13.6535C0.000988007 13.9189 0.107304 14.173 0.295607 14.36V14.33Z"
            fill="white"
          />
        </svg>
      </div>
      <p>Know more about me</p>
    </div>
  </div>
  <div class="right-col">
    <img src={knowledge} alt="knwoledge" />
  </div>
</div>
<Timeline />
<h2>Code</h2>
<div class="footer">
  <p>Other interests that have nothing to do with business:</p>
  <ul>
    <li>I was a swimming champion and played it for over 15 years</li>
    <li>I was a fencer as well but played it much less than swimming</li>
    <li>I am an avid reader, especially non-fiction, history and philosophy</li>
    <li>I have a cat and she’s our daughter</li>
    <li>
      I speak four languages fluently and others with a lower degree of fluency
    </li>
  </ul>
</div>

<style>
  .wrapper {
    display: flex;
    padding: 2.9375rem;
    gap: 14.8125rem;
  }
  h2 {
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 2.5rem;
    font-weight: normal;
    margin-top: 4.6875rem;
  }
  .footer {
    display: flex;
    flex-direction: column;
    gap: 0.8125rem;
    margin: 12.5rem 0;
  }
  .footer p {
    font-size: 2.5rem;
    font-weight: normal;
    width: 750px;
  }

  li {
    margin: 20px 0;
    font-size: 1.875rem;
    font-weight: normal;
  }
  ul {
    margin: 0 1.25rem;
  }

  .left-col h1,
  .left-col h2 {
    font-size: 2.5rem;
    font-weight: normal;
  }
  .left-col h2 {
    color: #a9adc1;
    margin-top: 1.125rem;
  }

  .scroll-down {
    margin-top: 5.9375rem;
    display: flex;
    gap: 1.875rem;
    align-items: center;
  }
  .button {
    display: flex;
    align-items: center;
    justify-content: center;
    border: 0.0625rem solid #9e9e9e;
    width: 44px;
    height: 44px;
    border-radius: 50%;
    animation: upDown 0.5s ease-in-out infinite alternate;
  }
  @keyframes upDown {
    0% {
      transform: translateY(-0.3125rem);
    }
    100% {
      transform: translateY(0.3125rem);
    }
  }
  .scroll-down p {
    font-size: 1.375rem;
  }

  img {
    object-fit: cover;
    height: 37.5rem;
    border-radius: 0.3125rem;
    transition: 0.3s;
    transform: scale(1);
  }
  img:hover {
    transform: scale(1.05);
  }
</style>
