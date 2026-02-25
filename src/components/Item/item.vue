<template>
  <div class="itemContainer">
    <i>
      <slot class="icon"></slot>
    </i>
    <div class="details">
      <h3>
        <slot class="heading"></slot>
      </h3>
      <slot></slot>
    </div>
  </div>
</template>
<style scoped>
.itemContainer {
  margin-top: 2rem;
  display: flex;
  position: relative;
}

.details {
  flex: 1;
  margin-left: 1rem;
}

i {
  display: flex;
  place-items: center;
  place-content: center;
  width: 2rem;
  height: 2rem;

  color: var(--color-text);
}
h3 {
  font-size: 1.2rem;
  font-weight: 500;
  margin-bottom: 0.4rem;
  color: var(--color-heading);
}
@media (min-width: 64rem) {
  .itemContainer {
    margin-top: 0;
    padding: 0.4rem 0 1rem calc(var(--section-gap) / 2);
  }
  i {
    top: calc(50% - 1.563rem);
    left: -1.625rem;
    position: absolute;
    border: 0.63rem solid var(--color-border);
    border-radius: 0.8rem;
    width: 3.125rem;
    height: 3.125rem;
  }

  .itemContainer:before {
    content: "";
    border-left: 0.63rem soli var(--color-border);
    position: absolute;
    left: 0;
    bottom: calc(50% + 1.563rem);
    height: calcl(50% - 1.563rem);
  }

  .itemContainer:after {
    content: "";
    border-left: 1px solid var(--color-border);
    position: absolute;
    left: 0;
    bottom: calc(50% + 1.563rem);
    height: calc(50% - 1.563rem);
  }

  .itemContainer:first-of-type:before {
    display: none;
  }

  .itemContainer:last-of-type:after {
    display: none;
  }
}
</style>
