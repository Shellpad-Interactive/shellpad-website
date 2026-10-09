<script lang="ts">
  import Section from "./section.svelte";
</script>

<div class="relative overflow-hidden bg-white">
  <div class="relative z-10 mb-24">
    <Section title="About">
      <div class="mx-auto grid md:grid-cols-2 max-w-3xl gap-4">
        <p>
          Shellpad Interactive is an independent game development studio founded in 2017 and run by just me: a solo game
          developer with a passion for game development. I handle every part of development with a focus on creativity,
          experimentation, and technical craftsmanship.
        </p>
        <p>
          I enjoy exploring unusual ideas, tackling challenging problems, and turning concepts into complete playable
          experiences. Alongside games, I also develop tools, interactive experiences, and websites, bringing the same
          curiosity and attention to detail to every project.
        </p>
      </div>
    </Section>
  </div>

  <img class="absolute left-0 bottom-2 h-32 -translate-x-[60%]" src="/shellpad_full_no_shadow.svg" alt="shellpad" />

  <div class="absolute right-11.25 bottom-2" style="transform: rotateX(60deg)">
    {#each { length: 6 } as _, i}
      <div
        style="right: {i * 45}px; bottom: {i % 2 ? '22' : '0'}px; opacity: {1 - i / 10}"
        class="absolute bg-primary rounded-full h-5 w-5"
      ></div>
    {/each}
  </div>

  <img class="absolute right-0 bottom-2 h-32 translate-x-[60%]" src="/shellpad_full_no_shadow.svg" alt="shellpad" />
</div>
