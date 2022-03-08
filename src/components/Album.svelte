<script>
  export let img;
</script>

<article>
  <div class="imagewrapper">
    <img src={`imgs/${String(img).padStart(4, "0")}.jpg`} alt="" />
    <svg
      xmlns="http://www.w3.org/2000/svg"
      width="32"
      height="32"
      fill="currentColor"
      class="bi bi-play-circle-fill"
      viewBox="0 0 16 16"
    >
      <path
        d="M16 8A8 8 0 1 1 0 8a8 8 0 0 1 16 0zM6.79 5.093A.5.5 0 0 0 6 5.5v5a.5.5 0 0 0 .79.407l3.5-2.5a.5.5 0 0 0 0-.814l-3.5-2.5z"
      />
    </svg>
  </div>
  <h3>100</h3>
  <p>Velkommen til den nye DK rap playliste med dansk rap, der...</p>
</article>

<style>
  article {
    background: var(--color-grey-100);
    padding: 1rem;
    color: var(--color-grey-700);
    font-size: 0.7rem;
    transition: all 0.2s;
    cursor: pointer;
    min-width: 200px;
  }
  article:hover {
    background: var(--color-grey-200);
  }
  svg {
    fill: lime;
  }
  .imagewrapper {
    position: relative;
  }
  .imagewrapper svg {
    position: absolute;
    bottom: 10px;
    right: 10px;
    transition: transform 0.2s, opacity 0.3s;
    opacity: 0;
    transform: translateY(10px);
  }
  article:hover svg {
    opacity: 1;
    transform: translateY(0px);
  }
</style>
